# [Go Official Tutorials](https://go.dev/doc/tutorial.html)


## Tutorial 1. Hello, World!

``` go
package main

import (
	"fmt"
)

func main() {
	fmt.Println("Hello, World!")
}
```

<details>
<summary>mod init</summary>

``` PowerShell
hello> go mod init hello
go: creating new go.mod: module hello
go: to add module requirements and sums:
        go mod tidy
```

</details>

<details>
<summary>run</summary>

``` PowerShell
hello> go run .
Hello, World!
```

</details>

Import module: quote

``` go
package main

import (
	"fmt"
	"rsc.io/quote"
)

func main() {
	fmt.Println("Hello, World!")
	fmt.Println(quote.Go())
}
```

<details>
<summary>mod tidy</summary>

``` PowerShell
hello> go mod tidy
go: finding module for package rsc.io/quote
go: downloading rsc.io/quote v1.5.2
go: found rsc.io/quote in rsc.io/quote v1.5.2
go: downloading rsc.io/sampler v1.3.0
go: downloading golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c
```

</details>

<details>
<summary>run</summary>

``` PowerShell
hello> go run .
Hello, World!
Don't communicate by sharing memory, share memory by communicating.
```

</details>
