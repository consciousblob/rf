---
id: T20260722-005
created: 2026-07-22
source:
  - text
related:
  - "[[mindscaping]]"
priority:
status: "0"
publish: true
title: M - appending numbers to objects
---
This is just an idea for how to approach version control for thoughts/views in a worldview representation in a mindscape / independent thought space / individual wiki / digital garden.

For example, I want to share thoughts on a particular object - say, the object I conceive as "consciousness". Obviously, thoughts might develop *a lot* over time. So, need some way to track this development. Might start a note "consciousness", but it quickly becomes unwieldy, and is eventually full of fluff in form of e.g. outdated thoughts/beliefs (views) about it. Then, want to abandon that note and "start afresh" BUT that original note contained the seeds of the new version - it tells the story of any subsequent conceptions of "consciousness". So, need/want some way of storing these note versions pertaining to same object, serially/chronologically.

Currently think this might be the best approach in terms of labelling (for ease of reference & viewing):
- The "current canonical" representative note for the object "consciousness" could be `0-consciouness`
- Then, once this becomes outdated, rename to `1-consciousness` and develop the new thoughts in the canonical `0-consciousness`
- Then, once *this* becomes outdated, rename it to `2-consciousness` and as before, start a fresh `0-consciousness`
- Keep developing versions, incrementing the prepend with each newly archived version.

But what about just a `consciousness` object? What could this represent?
Maybe it could be considered/used as a container of all versions.

Obviously, "consciousness" could be replaced with anything; this mini-discussion is supposed to delineate a general approach to updating thoughts & their containers.

[[Mon 10-08-2026]]
Lately, have started transitioning to the similar but kind of opposite convention of *appending* rather than *prepending* the number - so, `consciousness-0` instead of `0-consciousness`. Several reasons for this, but mainly because it makes opening/searching for notes easier. A drawback is that I can't search all the roots at once (e.g., when opening a note, type "0-" and see a list of all notes beginning with that), but there are ways around this, like using the Dataview plugin or something similar to pull all notes of that type into a table.

Also, I'm thinking it might be good to reserve one name convention for private, as opposed to public -facing versions of notes. Currently, I'm thinking either:
1. Reserve `root-0` for the latest private iteration, and `root-1` for the latest public iteration - then, when I publicise the `root-0`, rename it to `root-1` and the previous (public) `root-1` becomes `root-n` where `n` is the lowest non-taken (by previous public iterations) integer.
2. Reserve `root` for the latest public (or private) iteration and reserve `root-0` for the latest private (or public) iteration.

I was thinking that `root-n` works well at representing "this `root-n` note is `n - 1` iterations away from the latest public version, `root-1`, and `n` iterations away from the latest private version, `root-0`". BUT to actually implement this representation, would need to rename all previous iterations (to increment them) and I think this could make it more confusing to reference iterations and mentally track them (though it would make more sense digitally perhaps), so I'll abandon this idea for now and stick with the principle of: "once an iteration is no longer the latest (public or private) version, whatever label is assigned to it should remain with it (should be fixed) unless major overhaul of conventions occurs".