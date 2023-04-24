---
title: "Slices"
date: 2023-04-23T21:08:04-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/slices"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/slices.md"
---

# Reading material

A Tour of Go: [Slices](https://go.dev/tour/moretypes/7). 
Go by Example: [Slices](https://gobyexample.com/slices).

---


## First exercise

```go

// slices1
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	a := make(, 3, 10) // play with length and capacity
	fmt.Println("length of 'a':", len(a))
	fmt.Println("capacity of 'a':", cap(a))
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/slices/slices1/main.go)
- [Playground](https://go.dev/play/p/m-b99owCcJ3)
- [Solved](https://go.dev/play/p/Hsybut_8sU1)


## Second exercise

```go

// slices2
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	names := [4]string{"John", "Maria", "Carl", "Peter"}
	lastTwoNames := names[] // after figuring out the answer, try with other low/high bounds
	fmt.Println(lastTwoNames)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/slices/slices2/main.go)
- [Playground](https://go.dev/play/p/tgA7c5Y65Lx)
- [Solved](https://go.dev/play/p/mNbjp_u0FPk)


## Third exercise

```go

// slices3
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	names := []string{"John", "Maria", "Carl", "Peter"}
	names = append()
	fmt.Println(names)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/slices/slices3/main.go)
- [Playground](https://go.dev/play/p/tgA7c5Y65Lx)
- [Solved](https://go.dev/play/p/o6RI80q6WGf)

## Fourth exercise

```go

// slices4
// Make me compile!

// I AM NOT DONE
package main_test

import (
	"reflect"
	"testing"
)

func TestGetOnlyFirstName(t *testing.T) {
	names := []string{"John", "Maria", "Carl", "Peter"}
	firstName := names[3]

	if firstName != "John" {
		t.Errorf("firstName value must be John")
	}
}

func TestGetFirstTwoNames(t *testing.T) {
	names := []string{"John", "Maria", "Carl", "Peter"}
	firstTwoNames := names[5:10]
	expectedFirstTwoNames := []string{"John", "Maria"}

	if !reflect.DeepEqual(firstTwoNames, expectedFirstTwoNames) {
		t.Errorf("firstTwoNames should be %v, but got %v", expectedFirstTwoNames, firstTwoNames)
	}
}

func TestGetLastTwoNames(t *testing.T) {
	names := []string{"John", "Maria", "Carl", "Peter"}
	lastTwoNames := names[5:10]
	expectedLastTwoNames := []string{"Carl", "Peter"}

	if !reflect.DeepEqual(lastTwoNames, expectedLastTwoNames) {
		t.Errorf("firstTwoNames should be %v, but got %v", expectedLastTwoNames, lastTwoNames)
	}
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/slices/slices4/main.go)
- [Playground](https://go.dev/play/p/RXpsHW9X48W)
- [Solved](https://go.dev/play/p/MEug95GtlT4)