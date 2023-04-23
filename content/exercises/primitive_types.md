---
title: "Primitive Types"
date: 2023-04-23T19:53:27-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/primitive_types"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/primitive_types.md"
---

# Reading material

A Tour of Go: [Basic types](https://go.dev/tour/basics/11).

---


## First exercise

```go

// primitive_types1
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	storeIsOpen := true
	if storeIsOpen {
		fmt.Println("The store is open, let's buy some clothes!")
	}

	storeIsOpen
	if !storeIsOpen {
		fmt.Println("Oh no, let's buy some clothes online!")
	}
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/primitive_types/primitive_types1/main.go)
- [Playground](https://go.dev/play/p/wXWu2pHkxjb)
- [Solved](https://go.dev/play/p/EhWIOpZKGuN)

## Second exercise

```go

// primitive_types2
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	fmt.Printf("Hello, %s\n", who) // '%s' is used to format strings
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/primitive_types/primitive_types2/main.go)
- [Playground](https://go.dev/play/p/MLaNjfsr_19)
- [Solved](https://go.dev/play/p/ZtUn1xV-b3b)


## Third exercise

```go

// primitive_types3
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {

	fmt.Printf("Hello, I am %s and live in %s\n", who, country)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/primitive_types/primitive_types3/main.go)
- [Playground](https://go.dev/play/p/4gNhPL5yHMH)
- [Solved](https://go.dev/play/p/ItgHb9FCH2I)


## Fourth exercise

```go

// primitive_types4
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	var b1 byte = 110
	fmt.Println("byte value for b1:", b1)

	var b2 byte = ''
	fmt.Println("representation for b2:", b2)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/primitive_types/primitive_types4/main.go)
- [Playground](https://go.dev/play/p/eup5Cg1sgA7)
- [Solved](https://go.dev/play/p/p-SdkTWESaM)

## Fifth exercise

```go

// primitive_types5
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	var n1 integer = 101
	if n1 > 100 {
		fmt.Println("It is a big number")
	} else {
		fmt.Println("Not a big number at all")
	}

	var n2 float = 0.99
	fmt.Println(n2)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/primitive_types/primitive_types5/main.go)
- [Playground](https://go.dev/play/p/Vez4Pet1qVf)
- [Solved](https://go.dev/play/p/ly1S3xCOrpK)