---
title: "Functions"
date: 2023-04-20T01:08:08-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/functions"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/functions.md"
---

# Reading material:

Go by example: [Functions](https://gobyexample.com/functions)

A Tour of Go: [Functions](https://go.dev/tour/basics/4)

---

## First exercise:

```go

// functions1
// Make me compile!

// I AM NOT DONE
package main

func main() {
	call_me()
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/functions/functions1/main.go)
- [Playground](https://go.dev/play/p/v_lC8LDSs05)
- [Solved](https://go.dev/play/p/no2gWFrkAg4)

## Second exercise:

```go
// functions2
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	call_me(10)
}

func call_me(num) {
	for n := 0; n <= num; n++ {
		fmt.Printf("Num is %d\n", n)
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/functions/functions2/main.go)
- [Playground](https://go.dev/play/p/dCT1Vfaa9aB)
- [Solved](https://go.dev/play/p/m793kd_CdTn)

## Third exercise:

```go
// functions3
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	call_me()
}

func call_me(num int) {
	for n := 0; n <= num; n++ {
		fmt.Printf("Num is %d\n", n)
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/functions/functions3/main.go)
- [Playground](https://go.dev/play/p/dRe45O4Pj6X)
- [Solved](https://go.dev/play/p/ZOF9DMH_PUl)

## Fourth exercise:

```go
// functions4
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	fmt.Println("1 + 2 is: ", add_numbers(1, 2)) // don't change this line
}

func add_numbers(a int, b int) {
	return a + b
}

```
- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/functions/functions4/main.go)
- [Playground](https://go.dev/play/p/sSZuhGw2J8y)
- [Solved](https://go.dev/play/p/ChxSPGyk5CZ)
