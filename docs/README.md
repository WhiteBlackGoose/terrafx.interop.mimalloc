# TerraFX.Interop.Mimalloc

Interop bindings for mimalloc.

![ci](https://github.com/terrafx/terrafx.interop.mimalloc/workflows/ci/badge.svg?branch=main&event=push)
[![Discord](https://img.shields.io/discord/593547387457372212.svg?label=Discord&style=plastic)](https://discord.terrafx.dev/)

Packages are available at: https://github.com/orgs/terrafx/packages or via the NuGet Feed URL: https://pkgs.terrafx.dev/index.json

## Table of Contents

* [Code of Conduct](#code-of-conduct)
* [License](#license)
* [Contributing](#contributing)
* [Goals](#goals)
* [Languages and Frameworks](#languages-and-frameworks)
* [Benchmarks](#benchmarks)

### Code of Conduct

TerraFX and everyone contributing (this includes issues, pull requests, the
wiki, etc) must abide by the [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md).
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting the project team at admin@terrafx.dev.

### License

Copyright © Tanner Gooding and Contributors. Licensed under the MIT License
(MIT). See [LICENSE](../LICENSE.md) in the repository root for more information.

### Contributing

If you are looking to contribute you should read our
[Contributing](CONTRIBUTING.md) documentation.

### Goals

TerraFX is aiming to be a cross-platform framework for developing multimedia-
based applications.

* We plan on primarily supporting Linux and Windows and are looking at the
  possibility of supporting MacOS as well.
* We plan on providing an API that abstracts over the various lower-level
  graphics, audio, and windowing libraries APIs and makes them easy to use.

### Languages and Frameworks

TerraFX uses C# as its primary development language and .NET Core as our primary
target framework.

### Benchmarks

`Mimalloc.mi_malloc` takes **20%**-**50%** less time than `NativeMemory.Alloc` and
`Marshal.AllocHGlobal` methods (allocation + deallocation).

See more detailed benchmarks: [**raw**](./../docs/benchmarks/BenchmarkResultsRaw.md),
[**interpreted**](./../docs/benchmarks/BenchmarkResultsInterpreted.md).
