---
id: T20260722-002
created: 2026-07-22
source:
  - text
related:
  - "[[DG - Technical, Practical]]"
priority:
status:
publish: true
title: DG - Line breaks
---

Singular line breaks don't seem to automatically render with Quartz. If you want line breaks, add to the file `quartz\styles\custom.scss`:

```
p {
  white-space: pre-line;
}
```

Seemed to work.