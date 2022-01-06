# Ziglings

Welcome to Ziglings! This project contains a series of tiny broken programs.
By fixing them, you'll learn how to read and write
[Zig](https://ziglang.org/)
code.

![ziglings](https://user-images.githubusercontent.com/1458409/109398392-c1069500-790a-11eb-8ed4-7d7d74d32666.jpg)

Those tiny broken programs need your help! (You'll also save the planet from
evil aliens and help some friendly elephants stick together, which is very
sweet of you.)

Each exercise is self-contained and self-explained. However, you're encouraged
to also check out these Zig language resources for more detail:

* https://ziglearn.org/
* https://ziglang.org/documentation/master/

Also, the [Zig community](https://github.com/ziglang/zig/wiki/Community) is incredibly friendly and helpful!

## Getting Started

Install a [development build](https://ziglang.org/download/) of the Zig compiler.
(See the "master" section of the downloads page.)

Verify the installation and build number of `zig` like so:

```bash
$ zig version
0.9.0-dev.2025+xxxxxxxxx
```

Clone this repository with Git:

```bash
$ git clone https://github.com/ratfactor/ziglings
$ cd ziglings
```

Then run `zig build` and follow the instructions to begin!

```bash
$ zig build
```

## A Note About Versions

The Zig language is under very active development. In order to be current,
Ziglings tracks **development** builds of the Zig compiler rather than
versioned **release** builds. The last stable release was `0.8.1`, but Ziglings
needs a dev build with pre-release version "0.9.0" and a build number at least
as high as that shown in the example version check above.

It is likely that you'll download a build that is _greater_ than the minimum.

Once you have a build of the Zig compiler that works with Ziglings, they'll
continue to work together. But keep in mind that if you update one, you may
also need to update the other.

## Advanced Usage

It can be handy to check just a single exercise or _start_ from a single
exercise:

```bash
zig build 19
zig build 19_start
```

You can also run without checking for correctness:

```bash
zig build 19_test
```

Or skip the build system entirely and interact directly with the compiler
if you're into that sort of thing:

```bash
zig run exercises/001_hello.zig
```

Calling all wizards: To prepare an executable for debugging, install it
to zig-cache/bin with:

```bash
zig build 19_install
```
