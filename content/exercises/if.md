---
title: "If"
date: 2023-04-23T19:13:15-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/if"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/if.md"
---

# Reading material:

Go by example: [If/Else](https://gobyexample.com/if-else)

A Tour of Go: [If and Else](https://go.dev/tour/flowcontrol/7),  
[If](https://go.dev/tour/flowcontrol/5), [If with a short statement](https://go.dev/tour/flowcontrol/6)

---

## First exercise

```go

// if1
// Make me compile!

// I AM NOT DONE
package main

import "testing"

func bigger(a int, b int) int {
	// Complete this function to return the bigger number
	// Use only if statements
	if a > b {
		return a
	} else {
		return b
	}
}

func TestTwoIsBiggerThanOne(t *testing.T) {
	if bigger(2, 1) != 2 {
		t.Errorf("2 is bigger than 1")
	}
}

func TestTenIsBiggerThanFive(t *testing.T) {
	if bigger(5, 10) != 10 {
		t.Errorf("10 is bigger than 5")
	}
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/if/if1/main_test.go)
- [Playground](https://go.dev/play/p/316919AjuJq)
- [Solved](https://go.dev/play/p/rsrMpTBDy1L)

## Second exercise

```go
// if2
// Make me compile!

// I AM NOT DONE
package main

import "testing"

func fooIfFizz(fizzish string) string {
	if fizzish == "fizz" {
		return "foo"
	} else {
		return "complete me"
	}
}

func TestFooForFizz(t *testing.T) {
	result := fooIfFizz("fizz")
	if result != "foo" {
		t.Errorf("should be 'foo' but got %s", result)
	}
}

func TestBarForFuzz(t *testing.T) {
	result := fooIfFizz("fuzz")
	if result != "bar" {
		t.Errorf("should be 'bar' but got %s", result)
	}
}

func TestDefaultForBazz(t *testing.T) {
	result := fooIfFizz("random stuff")
	if result != "baz" {
		t.Errorf("should be 'baz' but got %s", result)
	}
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/if/if2/main_test.go)
- [Playground](https://go.dev/play/p/fvoSLE_pPqs)
- [Solved](https://go.dev/play/p/xMWmKJz1QeqL)