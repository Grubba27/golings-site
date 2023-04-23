---
title: "Maps"
date: 2023-04-23T19:24:39-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/maps"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/maps.md"
---

# Reading material:

Go by example: [Maps](https://gobyexample.com/maps).

A Tour of Go: [Maps](https://go.dev/tour/moretypes/19), [Mutating Maps](https://go.dev/tour/moretypes/22), [exercise Maps](https://go.dev/tour/moretypes/23) - [Solved](https://go.dev/play/p/Ps2U2xvkEt5)

---

## First exercise

```go

// maps1
// Make me compile!
//
// I AM NOT DONE
//
package main

import "fmt"

func main() {
	// Map with people names and their ages
	m := make(map)

	m["John"] = 30
	m["Ana"] = 21

	fmt.Printf("John is %d and Ana is %d", m[], m[])
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/maps/maps1/main.go)
- [Playground](https://go.dev/play/p/7piJ4P_s6lj)
- [Solved](https://go.dev/play/p/E-KMlz-BvRC)


## Second exercise

```go

// maps2
// Make me compile!
//
// I AM NOT DONE
package main

import "fmt"

func main() {
	m := map{}
	fmt.Printf("John is %d and Ana is %d", m["John"], m["Ana"])
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/maps/maps2/main.go)
- [Playground](https://go.dev/play/p/oRLlQPrio18)
- [Solved](https://go.dev/play/p/eTCnoWU_-h8)


## Third exercise

```go
// maps3
// Make me compile!
//
// I AM NOT DONE
package main

import "testing"

func TestGetPhone(t *testing.T) {
	phoneBook := map[string]string{
		"Ana":  "+01 101 102",
		"John": "+01 333 666",
	}

	phone, _ := phoneBook["Anna"] // something seems wrong here
	expectedPhone := "+01 101 102"
	if phone != expectedPhone {
		t.Errorf("phone should be %s but got %s", expectedPhone, phone)
	}
}

func TestInsertPhone(t *testing.T) {
	phoneBook := map[string]string{
		"Ana":  "+01 101 102",
		"John": "+01 333 666",
	}

	phone, _ := phoneBook["Laura"] // don't change this line
	expectedPhone := "+11 99 98 97"
	if phone != expectedPhone {
		t.Errorf("phone should be %s but got %s", expectedPhone, phone)
	}
}

func TestDeletePhone(t *testing.T) {
	phoneBook := map[string]string{
		"Ana":  "+01 101 102",
		"John": "+01 333 666",
	} // don't change the original map

	totalPhones := len(phoneBook)
	expectedTotalPhones := 1
	if totalPhones != expectedTotalPhones {
		t.Errorf("phoneBook should have only %d contact, but got %d", expectedTotalPhones, totalPhones)
	}
}

```
- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/maps/maps3/main_test.go)
- [Playground](https://go.dev/play/p/w9bgEPUmWUO)
- [Solved](https://go.dev/play/p/QFzScTRR0BL)