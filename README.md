# awesome-lib

[![CI](https://github.com/mikejoh/awesome-lib/actions/workflows/go.yml/badge.svg)](https://github.com/mikejoh/awesome-lib/actions/workflows/go.yml)
[![License](https://img.shields.io/github/license/mikejoh/awesome-lib)](https://github.com/mikejoh/awesome-lib/blob/main/LICENSE)

A tiny Go library used to try out tooling.

`awesome-lib` is a minimal Go module with a couple of small, self-contained functions — one that logs and returns a greeting via [`logrus`](https://github.com/sirupsen/logrus), and one that returns a static string from a sub-package. It's primarily used as a sandbox for exercising Go module tooling (CI, dependency updates, linting, etc.) rather than for any real-world functionality.

## Install

```
go get github.com/mikejoh/awesome-lib
```

## Usage

```go
package main

import (
	"fmt"

	awesome "github.com/mikejoh/awesome-lib"
	"github.com/mikejoh/awesome-lib/pkg/text"
)

func main() {
	fmt.Println(awesome.Awesome())
	fmt.Println(text.Text())
}
```
