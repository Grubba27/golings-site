---
title: "Range"
date: 2023-04-23T20:53:40-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/range"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/range.md"
---

# Reading material

A Tour of Go: [Range](https://go.dev/tour/moretypes/16). 
Go by Example: [Range](https://gobyexample.com/range).

---


## First exercise

```go

// range1
// Make me compile!
//
// I AM NOT DONE
package main

import "fmt"

func main() {
	evenNumbers := []int{2, 4, 6, 8, 10}

	for _, v := {
		fmt.Printf("%d is even\n", v)
	}
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/range/range1/main.go)
- [Playground](https://go.dev/play/p/kVA2YU0_Qx0)
- [Solved](https://go.dev/play/p/8Qyn0OxxZZe)


## Second exercise

```go

// range2
// Make me compile!
//
// I AM NOT DONE
package main

import "fmt"

func main() {
	phoneBook := map[string]string{
		"Ana":  "+01 101 102",
		"John": "+01 333 666",
	}

	for name, phone := range phoneBook {
		fmt.Printf("%s has the %s phone\n", name, phone)
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/range/range2/main.go)
- [Playground](https://go.dev/play/p/1SfT5Uu7kEy)
- [Solved](https://go.dev/play/p/D7qkpG6sKn-)


## Third exercise

```go

// range3
// Make me compile!
//
// I AM NOT DONE
package main_test

import (
	"reflect"
	"testing"
)

func TestFilterEvenNumbers(t *testing.T) {
	numbers := []int{1, 2, 3, 4, 5, 6, 7, 8, 9, 10}

	evenNumbers := []int{} // use range to filter even numbers

	for range numbers {
	}

	if !reflect.DeepEqual(evenNumbers, []int{2, 4, 6, 8, 10}) {
		t.Errorf("evenNumbers does not contain all the required even numbers, got %v", evenNumbers)
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/range/range2/main.go)
- [Playground](https://go.dev/play/p/AvGKPx8otle)
- [Solved](https://go.dev/play/p/_HvzntOQOKY)