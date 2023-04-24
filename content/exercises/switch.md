---
title: "Switch"
date: 2023-04-23T21:38:53-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/structs"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/structs.md"
---

# Reading material

A Tour of Go: [Switch](https://go.dev/tour/flowcontrol/9). 
Go by Example: [Switch](https://gobyexample.com/switch).

---


## First exercise

```go

// switch1
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	status := "open"
	switch {
	case "open":
		fmt.Println("status is open")
	case "closed":
		fmt.Println("status is closed")
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/switch/switch1/main.go)
- [Playground](https://go.dev/play/p/CtVz7cmhfEZ)
- [Solved](https://go.dev/play/p/ChJbi9Vxjns)

## Second exercise

```go

// switch2
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	switch {
	case 0 > 1:
		fmt.Println("zero is greater than one")
	case:
		fmt.Println("one is greater than zero")
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/switch/switch2/main.go)
- [Playground](https://go.dev/play/p/iqwaMerA5pb)
- [Solved](https://go.dev/play/p/82cMH-DXDpE)

## Third exercise

```go

// switch3
// Make me compile!

// I AM NOT DONE
package main

import "testing"

func weekDay(day int) string {
	// Return the day of the week based on the
	// integer. Use a switch case to satisfy all test cases below
	return "Sunday"
}

func TestWeekDay(t *testing.T) {
	tests := []struct {
		input int
		want  string
	}{
		{input: 0, want: "Sunday"},
		{input: 1, want: "Monday"},
		{input: 2, want: "Tuesday"},
		{input: 3, want: "Wednesday"},
		{input: 4, want: "Thursday"},
		{input: 5, want: "Friday"},
		{input: 6, want: "Saturday"},
	}

	for _, tc := range tests {
		day := weekDay(tc.input)
		if day != tc.want {
			t.Errorf("expected %s but got %s", tc.want, day)
		}
	}
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/switch/switch3/main.go)
- [Playground](hhttps://go.dev/play/p/U6XXrvIAVj4)
- [Solved](https://go.dev/play/p/EZI3ki7uBaP)