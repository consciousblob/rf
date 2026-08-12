---
id: T20260806-003
created: 2026-08-06
source:
  - text
related:
  - "[[my-mindscape]]"
priority:
status:
publish: true
---
This note is to capture anything related to this RF site and any related mindscaping endeavours, that comprise the creation/cultivation of TM's own independent thought space.

Possibly a lot of overlap with [[my-mindware]] but this my-mindscape note is more for my personal digital thought space, whereas my-mindware is more for my contributions to apps/tool things that could be use by/between any mindscape(s), including the collective mindscape (i.e., the synthesis of and communication between different independent though spaces).

A lot of notes are for TM's benefit (so, interpretability for other minds is not prioritised), but publicised in case helpful to other minds in their personal mindscaping endeavours. A lot of more "technical" stuff is generated/supplemented by GenAI.

---

## Terminology
Since very much noob at web-devy stuff, will list all terms here to maintain an overview of everything TM learning.

- **Building** = **compiling**
	- `npx quartz build`
	- Quartz transforms raw Markdown files into HTML/CSS/JS files.
- **Serving**
	- `npx quartz build --serve`
	- Runs small local web server so browser can view the built files.
	- Automatically builds, but serves as well (on e.g. localhost:8000) and rebuilds automatically after modifications.
- **Deploying**
	- Pushing the built site to a **static web host** (such as Cloudflare Pages, GitHub Pages, Netlify, Vercel).

## Technical
A current attempted summary/overview of how TM's mindscape exists (how it came into existence, and what tools/infrastructure allows it to exist/persist). Emboldened/italicised words are for TM's benefit.

- Notes are written in markdown in **Obsidian** (a kind of glorified text editor, but that doesn't really do it justice).
- **Quartz** is a *static site generator* (built in Node.js) that converts the Obsidian markdown files into HTML/CSS/JS and creates a website from them.
- **GirHub** stores the Quartz project (code + public notes) as a repository, and acts as the trigger point for publishing.
- **Cloudflare Pages** is a hosting service that watches the GitHub repo; whenever changes pushed, it runs the Quartz build itself and puts the resulting website live at the domain.


## Misc
Little technical/practical things TM thinks useful to share.

- [[DG - Line breaks]]
	- How to render line breaks in a Quartz site.
- 
