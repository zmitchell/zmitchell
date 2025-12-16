# Zach Mitchell (`@zmitchell`)

Hey, I'm Zach. I'm a software engineer and a professional curler[^1]. I'm also a [CPython contributor](https://github.com/python/cpython/pull/6964/commits/0cc74ee9467974d6aad44a7476c68291d4f9ba26)[^2].

## Background

My background is physics, but that's not what I do anymore because lasers don't have unit tests or version control. I did a PhD building various kinds of laser spectrometers to study how energy moves between molecules (specifically inside proteins involved in photosynthesis). The lasers I built spit out pulses of light as short as 20 femtoseconds (femto = 10^-15), and sometimes they even worked! I also did quantum mechanics simulations. If you call me "doctor" I'll simultaneously feel extremely uncomfortable and proud. Do with that what you will.

I developed an interest in systems programming during my PhD, and now I spend my free time doing things like building eBPF-based profilers (like everyone else). I feel at home in Rust and Zig, but I spent several years knee-deep in Python. I have a healthy fear of C++, and C macros scare me a little bit. It's my professional opinion as a doctor that header files should be illegal.

I spent about 9 months on the [Nix](https://nixos.org) documentation team (if you've seen the documentation you'll understand why). I don't do that anymore, but I do still use Nix to configure all of my machines (yes, even my macOS laptop). You can see my Nix configurations here: [zmitchell/nixos-configs](https://github.com/zmitchell/nixos-configs). I'm the program chair for the [Nix conference](https://planetnix.com) that takes place in North America every year.

## Work

I work at [Flox](https://flox.dev) building something that's hard to do justice in a single sentence. I work on both the CLI and the backend server. The CLI is open source and can be found here: [flox/flox](https://github.com/flox/flox).

Flox is a tool for creating reproducible "environments". If you use it during development, it's a developer environment. If you use it in CI, it's a CI environment. If you use it in production, it's a production environment. It's a way of getting the same set of software everywhere that you use it. macOS or Linux. x86_64 or Arm.

For developers, the idea is that onboarding to an existing project looks like this:

```
$ git clone
$ flox activate
```

I truly believe it's the current local maximum for developer environments, bringing Nix-powered reproducibility together with an intuitive and familiar CLI.

I can't help myself, so I've developed several tools and projects related to Flox:

- **flox-debugger** - A "debugger" for the `flox activate` command
  - [zmitchell/flox-debugger](https://github.com/zmitchell/flox-debugger)
  - The `flox activate` command does the complex, heavy lifting of setting up a shell with a reproducible set of dependencies, carefully handled process parentage, etc. It's the magic that makes Flox work, and it's simultaneously the hardest part to get correct.
- **release-flox (internal)** - The (internal) tool we use to cut and upload Flox CLI releases
- **flox-ci (private)** - A proof of concept CI system based around Flox environments
  - This uses `systemd-nspawn` containers and ZFS copy-on-write clones to make starting jobs substantially faster when there are jobs on a given host that use the same Flox environment.

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
