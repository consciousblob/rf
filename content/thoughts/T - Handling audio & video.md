---
id: T20260808-001
created: 2026-08-08
source:
  - text
related:
  - "[[technical]]"
priority:
status:
publish: false
---

Derived from Claude: [Removing computer noise from video audio - Claude](https://claude.ai/chat/68f05fe5-f07f-4970-976b-4aa0276ccf4b)
and
[Audio editing in Audacity - Claude](https://claude.ai/chat/f4dc18b2-1f42-4382-a15e-2c3f4f3ed737)

---
Extract audio with ffmpeg:
`ffmpeg -y -i video.mp4 -vn -af "aresample=async=1:first_pts=0" -acodec pcm_s16le -ar 44100 audio.wav`

Check duration (make sure same as video duration):
`ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1 audio.wav`

Audacity - select a bit of audio w/o talking, but with the background noise (click & drag), then
Effects -> Noise reduction
Click the "Get Noise Profile" button. This teaches Audacity what to strip away.

Select a small segment *with* speaking, go back to Noise Reduction, do these settings:
![[Pasted image 20260808210219.png]]
and click Preview.

If good, cross this off, select all audio, do the same, press OK.

Export the audio as `audio.wav` (to work with the copied/pasted commands).

Replace the audio in the video:
`ffmpeg -i video.mp4 -i audio.wav -map 0:v:0 -map 1:a:0 -c:v copy -c:a aac -b:a 192k final_video.mp4`

---
## Equalise/Amplify Volume
To amplify volume in Audacity,
select all audio then
Effect -> Amplify
and apply the recommended amplification.

**Alternatively** if some segments are quieter:
1. Select segments of different volumes
2. Effect -> Volume & Compression -> Loudness Normalisation
3. I think -23 is max so if you want a bit quieter, try anything up to -16


## Cut part of video w/o encoding

Cut part of video without re-exporting:
`ffmpeg -i input.mp4 -ss 00:01:30 -to 00:04:00 -c copy output.mp4`

Or for just cutting from some point til the end:
`ffmpeg -i input.mp4 -ss 00:01:30 -c copy output.mp4`

