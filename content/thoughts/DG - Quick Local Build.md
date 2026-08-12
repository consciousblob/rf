---
id: T20260806-002
created: 2026-08-06
source:
  - text
related:
  - "[[my-mindware]]"
  - "[[my-mindscape]]"
priority:
status:
publish: true
---
Frequently go through the process of running quartz locally to make updates/modifications before pushing onto the public site, and this involves a (lengthy when repeated as often as TM) process of:
1. Open command prompt
2. Change directory to the folder the quartz stuff is in
3. Type & run `npx quartz build --serve`
4. Click link to `http://localhost:8080/` to open locally built site

Might not seem like much, but annoying, unnecessary friction for an activity performed frequently. So, want to create some kind of automation to perform all this from e.g. 1 command/click.
