# Thoughts on Wasm3 Verification

This code is pretty nice and well organized overall. Envisioning a large project, the wasm spec
is so simple and well-defined that it would make a great top-level specification. A smaller
project might involve reasoning about some of the memory mangagement, or individual instructions.

I'd be curious what the correctness concerns might be, and how likely any bugs are to exist in this codebase.

Stack managment looks like it would maybe be a simple foothold to start proving. There seem
to be some simple invariants that need to hold about it.

Probably similar goes for code page management.

While the compilation-continuation approach results in good
performance, I'm nervous about how that might abstract from what we'd want to prove at
the end of the day. I think everything was doable, but I was definitely expecting a "deeper" embedding
when I first envisioned a verification effort. It seems likely that compilation and execution would need to be reasoned about separately and then stitched together somehow for an end-to-end story... Ideally parsing gets added in as well.

Overall, this is definitely a code-base that's amenible to verification, although some of the
complexities make me nervous to tackle it on less than a medium-sized project.


