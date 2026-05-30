# Zach Mitchell (`@zmitchell`)

Hey, I'm Zach. I'm a software engineer and a professional curler[^1]. I'm also a [CPython contributor](https://github.com/python/cpython/pull/6964/commits/0cc74ee9467974d6aad44a7476c68291d4f9ba26)[^2].

## Background

My background is physics, but that's not what I do anymore because lasers don't have unit tests or version control. I did a PhD building various kinds of laser spectrometers to study how energy moves between molecules (specifically inside proteins involved in photosynthesis). The lasers I built spit out pulses of light as short as 20 femtoseconds (femto = 10^-15), and sometimes they even worked! I also did quantum mechanics simulations. If you call me "doctor" I'll simultaneously feel extremely uncomfortable and proud. Do with that what you will.

I developed an interest in systems programming during my PhD, and now I spend my free time doing things like building eBPF-based profilers (like everyone else). I feel at home in Rust and Zig, but I spent several years knee-deep in Python. I have a healthy fear of C++, and C macros scare me a little bit. It's my professional opinion as a doctor that header files should be illegal.

I spent about 9 months on the [Nix](https://nixos.org) documentation team (if you've seen the documentation you'll understand why). I don't do that anymore, but I do still use Nix to configure all of my machines (yes, even my macOS laptop). You can see my Nix configurations here: [zmitchell/nixos-configs](https://github.com/zmitchell/nixos-configs). For a few years I was the program chair for the [Planet Nix](https://planetnix.com) conference.

## Interests

I'm particularly interested in systems software of various kinds. I constantly have an itch to build tools that other developers can use because I see so many of our tools as suboptimal.

Lately I've been on a build system kick. Nix gets close to what I want, but falls short on a few fronts. I ended up working at [Flox](https://flox.dev) for a few years, which is a big leap forward in user experience, but a step backwards in flexibility and interoperability.

If you want to be my best fried in the whole world, please write a tool for local code review that (1) doesn't suck, (2) is `jujutsu`-compatible, and (3) isn't written by vibe coders for vibe coders.

Most of my personal projects these days are written in Zig, but I'd like an excuse to use Gleam for something.

## Writing

I write infrequently, but I enjoy doing it when I have something to teach. Much of the documentation at [flox.dev/docs](https://flox.dev/docs) was written by me (especially the Concepts section).

A few highlights:

- [Speeding up a quantum mechanics simulation by 250x](https://tinkering.xyz/fmo-optimization-story/)
- [A writeup of a Flox feature I designed](https://tinkering.xyz/flox-composition/)

## Talks

I'm genetically incapable of shutting up, and being on stage temporarily quenches my thirst for power, so I frequently find myself speaking at conferences or working booths.

The full list of my appearences is here: https://tinkering.xyz/talks/

The highlights:

- NixCon 2025 — “You can't spell ‘devshell’ without ‘hell’”
  - https://media.ccc.de/v/nixcon2025-56410-you-cant-spell-devshell
- RustConf 2023 — “Async Building Blocks: A Streaming Data Drama in Three Acts”
  - https://youtu.be/hU-lKbAdOUg

[^1]: In the sense that I somehow convinced my employer to sponsor my curling team. I'm not kidding: https://flox.dev/blog/flox-named-exclusive-media-sponsor-of-the-rock-bottom-curling-clubs-2025-season/
[^2]: Look, someone had to do it. Also, no one else volunteered to be an accomplice in my Python [crime](https://tinkering.xyz/abusing-type-annotations/).
