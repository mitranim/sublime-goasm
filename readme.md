## Overview

Syntax definition for Go assembly for Sublime Text. Work in progress.

## Why

Go has its own meta-assembly. Other assembly plugins for ST can't handle its idiosyncratic syntax.

Reading assembly is helpful when profiling, and teaches you more about how the language works and what your program actually does.

## Installation

Clone this repository into ST's Packages folder. On MacOS, this is usually `"/Users/<user>/Library/Application Support/Sublime Text 3/Packages"`. Find it using Sublime's menu → Preferences → Browse Packages.

It will automatically pick up `*.s` and `*.goasm` files. The latter is made-up as a way to disambiguate assembly formats.

Related: since you're using Sublime Text with Go, consider a better Go syntax: https://github.com/Mitranim/sublime-gox. Also consider this syntax definition for `go.mod` files: https://github.com/Mitranim/sublime-gomod.

## Getting Started

Read this documentation on Go assembly: https://golang.org/doc/asm.

Output assembly for a program:

```sh
go build -gcflags -S
```

For syntactic support, output the assembly to a file:

```go
go build -gcflags -S 2> asm.goasm
```

## Misc

License: https://en.wikipedia.org/wiki/WTFPL

I'm receptive to suggestions. If this package _almost_ satisfies you but needs changes, open an issue or chat me up. Contacts: https://mitranim.com/#contacts
