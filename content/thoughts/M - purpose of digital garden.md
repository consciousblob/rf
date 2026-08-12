---
id: T20260804-001
created: 2026-08-04
source:
  - text
related:
  - "[[mindscaping]]"
  - "[[my-mindscape]]"
priority:
status:
publish: false
---
**Context for LLM**

I have set up a digital garden on a domain I have bought, rootfinding.com, using Obsidian and Quartz. Information about it is below.

Stack:
- Quartz v4.5.2 at `C:\Users\theau\Documents\diggar`
- Public notes folder: `Obsidian Vault\Public` — symlinked to `diggar\content`
- GitHub repo: `github.com/consciousblob/rf` (branch: `v4`)
- Hosted on Cloudflare Pages, live at `rootfinding.com`
- `baseUrl` set to `rootfinding.com`

Workflow:
- Write notes to the Public folder in Obsidian Vault
- Local preview: `npx quartz build --serve` → `localhost:8080`
- Run `npx quartz sync` from an **administrator** Command Prompt
- Cloudflare auto-rebuilds within ~60 seconds of each sync

The purpose of this site is to share my thoughts fluidly, in as many formats as possible. It acts as an "independent thought space" - my own corner of the internet I can customise to best represent and share my thoughts, and have full ownership of my outputs and how they are presented.

My aim is to encourage as many people as possible to do a similar thing - to set up their own digital garden / independent thought space - and for us to create various "mindware modules", which are pieces of hardware and (primarily) software to link these thought spaces, to transition away from traditional monolithic privately owned social media platforms. Ideally, we'd have maximum personalisation and divergence in our own thought spaces (full freedom in what and how we express), along with the possibility of maximum standardisation and convergence (the ability to parse the outputs of others into formats that we prefer to input). For example, suppose mind A shares thoughts in a kind of serial Instagram-style stream of posts (image + short caption), mind B shares thoughts primarily via video, and mind C shares thoughts mostly through long-form essays plus some shorter notes / tweet-style posts. Then, suppose that mind C wishes to receive/input thoughts only in a similar written (long or short -form) format to how they transmit/output. Then ideally, we would have a mindware module that could take the posts of A and videos of B, and parse them into a written format specified by C.

This is the ultimate aim, and my site is just one node in this network / digital ecosystem of minds and their thought spaces.

I want to be able to record thoughts privately, and then publicise a subset of these. My current Obsidian system uses a particular note template, where each note is called a "thought". A thought note has the following properties:
- ID (unique)
- Created (date)
- Title (as the note name will be lowercase with hyphens for HTML standardisation)

I would like to include a property to differentiate between the type/form/format of the thought (text/video/audio/image) and another property to indicate a more specific type (e.g. art, poem, fiction/short story, song, rambling) and/or indicate level of development/coherence (finished/finalised, messy/chaotic, in process, etc.) but I'm not yet sure of the best way to label/differentiate these. I have a mostly unused property called "status" which I could use somehow.

