# Read the branch, not the names

Function names, comments, strings, and encoded payloads can be clues. They do not
establish what a program does. Trace the actual calls and the conditions that reach
them. A function with a frightening name may be a decoy; a blandly named function may
read credentials or send data elsewhere.

For each branch, record the guard, the operations it reaches, and the data those
operations touch. Keep ordinary browser behavior separate from code gated on a Node
environment or an environment variable. A conditional path is still part of the
program's behavior, even if it does not run in a browser.

## Source case

In [veritas's write-up](https://nullpt.rs/fingerprinting-bioweapons), the browser
fingerprinting behavior and the Node-only path are distinct. The former collects
browser signals. The latter contains operations aimed at local files, a downloaded
binary, and persistence. Describing the whole script as harmless because its browser
path fingerprints visitors would miss the conditional path. Calling every alarming
identifier proof of a working biological capability would also misread the code.

Static analysis is enough to identify those operations. Do not run the sample to
resolve uncertainty. If reachability, successful execution, or intent is unknown, say
so.
