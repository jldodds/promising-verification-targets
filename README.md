# Promising Verification Targets

This list is things that I'd like to verify, or that might be easily verifiable.
I'd like to keep the list open-source, and for now it's all C because that's what I'm thinking about, but other contributions and suggestions are more than welcome via PR, email or Twitter!

Right now I've written this with SAW in mind, because that's where my focus is. If other languages/tools show up, it's probably worth adding a column.

Finally, if you're interested in actually _doing_ some verification, please reach out. An important part of what we're workign on now is trying out our tools, and we'd gladly offer some mentoring time to any willing or aspiring ~~victims~~ proof engineers.

## C Programs

| Project | Notes | Suggester (thanks!) |
|---------|----------------------------|---------------------|
| [Wasm3](https://github.com/wasm3/wasm3) | [Link](wasm3.md) | [Frank](https://twitter.com/jedisct1) |
| [LibSodium](https://github.com/jedisct1/libsodium) | optimized x86! | [DKP](https://twitter.com/tweetdkp)
| [Sweet-B](https://github.com/westerndigitalcorporation/sweet-b) | need to examine this code | [Brian Mastenbrook](https://twitter.com/bmastenbrook)
| [Signal C implementation](https://github.com/signalapp/libsignal-protocol-c) |  | [Matthew Fernandez](https://twitter.com/smattrr), [Aaron Tomb](https://galois.com/team/aaron-tomb/)
| [DTach](https://github.com/crigler/dtach) | Pretty small and self-contained, any obvious properties? | [Tikhon Jelvis](https://twitter.com/tikhonjelvis)
| ASN.1 | So many bugs, so much code | [Martin Nyx Brain](@ciphernyx)
| [Azure C SDK](https://github.com/Azure/azure-sdk-for-c) | Memory safety targets, api stuff is harder | Me
| Compression/Image libraries | Probably lots to do, binary formats would be fun. Some specs are very clear | [Tristan Ravitch](https://galois.com/team/tristan-ravitch/)
| [Curl](https://github.com/curl/curl) | So much here, probably some high impact parts | [Tom DuBuisson](https://twitter.com/MDTom)
| [libflint](https://www.flintlib.org/) | |[Tom DuBuisson](https://twitter.com/MDTom)
| sudo (parsing) | | [Tom DuBuisson](https://twitter.com/MDTom)


### Wall of shame
Funny suggestions that fill me with rage or fear (nonexclusive or). Honestly all of these are probably chock-full of bugs and good problems. We'll know we've won the verification game when we can move them up to the "real list".

| Project | Notes | Suggester (no thanks!)
| ------- | ----- | ----------------------
| Doom (memory allocater)    | Bugs might be useful for speedrunners. Seriously there's probably good targets in here, but I'm too scared | [Dominic Orchard](https://twitter.com/dorchard) 
| GMP | Yeah, I'm going to verify a program I can't draw a smiley face in. | [Sebastian Ullrich](https://twitter.com/derKha)
| Red/Black Tree | We're going to need a bigger boat (and a separation logic) | [Martin Nyx Brain](@ciphernyx)