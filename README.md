Before start, there is another good Sass compilers written in !!PURE!! Go.
Star them not here:

* [github.com/c9s/c6](https://github.com/c9s/c6)
* [github.com/yosssi/gcss](https://github.com/yosssi/gcss)

Or you can go to another up to date libsass binding projct:

* [github.com/wellington/go-libsass](https://github.com/wellington/go-libsass)


# About sass

It's Go binding for [libsass][4] which written in cpp by [hcailin][5].
It compile [Sass][3] file (.scss) to CSS.

> This is no more an experimental _cgo_ project to find best practice to
> guide people to download and install third party c library.

# Documentation

## Prerequisites

[Install Go][1]

## Installation

    $ go get github.com/suapapa/go_sass

If you don't have libsass in your system, run;

    $ cd $GOROOT/src/pkg/github.com/suapapa/go_sass
    $ install_libsass.sh

I'll ask admin password to install the libsass system widely.

## General Documentation

Use `go doc` to vew the documentation for sass

    go doc github.com/suapapa/go_sass

Or alternatively, refer [go.pkgdoc.org][2]

## Example

Compile Sass folder into CSS:

    package main

    import (
            "github.com/suapapa/go_sass"
    )

    func main() {
            var sc sass.Compiler
            sc.CompileFolder("_scss", "css")
    }

# Author

Homin Lee &lt;homin.lee@suapapa.net&gt;

# Copyright & License

Copyright (c) 2012, Homin Lee.
All rights reserved.
Use of this source code is governed by a BSD-style license that can be
found in the LICENSE file.

[1]: http://golang.org/doc/install
[2]: http://go.pkgdoc.org/github.com/suapapa/go_sass
[3]: http://sass-lang.com/
[4]: https://github.com/hcatlin/libsass
[5]: https://github.com/hcatlin
