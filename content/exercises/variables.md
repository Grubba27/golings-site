---
title: "Variables"
date: 2023-04-23T22:05:44-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/variables"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/variables.md"
---

# Reading material

A Tour of Go: [Variables](https://go.dev/tour/basics/8), [Variables with initializers](https://go.dev/tour/basics/9), [Short variable declarations](https://go.dev/tour/basics/10).
Go by Example: [Variables](https://gobyexample.com/variables), [Constants](https://gobyexample.com/constants).

---

## First exercise

```go
// variables1
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	var = 5
	fmt.Printf("x has the value %d", x)
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/variables/variables1/main.go)
- [Playground](https://go.dev/play/p/IIGsUORIOO6)
- [Solved](https://go.dev/play/p/YgBPsTSOp3m)

## Second exercise

```go

// variables2
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	x = 5
	fmt.Printf("x has the value %d", x)
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/variables/variables2/main.go)
- [Playground](https://go.dev/play/p/CBo29RhYw25)
- [Solved](https://go.dev/play/p/0nThlXamg9y)

## Third exercise

```go

// variables3
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	var x
	fmt.Printf("x has the value %d", x)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/variables/variables3/main.go)
- [Playground](https://go.dev/play/p/IyZcTYSsi5W)
- [Solved](https://go.dev/play/p/zQF1fDemmfP)

## Fourth exercise

```go

// variables4
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	x := "TEN" // Don't change this line
	fmt.Printf("x has the value %s", x)

	if true {
		x = 1
		fmt.Println(x + 1)
	}

	fmt.Println(x)
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/variables/variables4/main.go)
- [Playground](https://go.dev/play/p/J0uYR5HgSpe)
- [Solved](https://go.dev/play/p/rewoAn2zpZ_J)

## Fifth exercise

```go
// variables5
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

const Pi

func main() {
	fmt.Println(Pi)
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/variables/variables5/main.go)
- [Playground](https://go.dev/play/p/WRRzCi4TUHX)
- [Solved](https://go.dev/play/p/MjALSjMD8zA)

## Sixth exercise

```go

// variables6
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

const x = 10

func main() {
	fmt.Println(x)

	x = x + 1
	fmt.Println(x)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/variables/variables6/main.go)
- [Playground](https://go.dev/play/p/WRRzCi4TUHX)
- [Solved](https://go.dev/play/p/BtjU-UcdgxL)