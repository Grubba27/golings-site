---
title: "Structs"
date: 2023-04-23T21:21:24-03:00
draft: false
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/structs"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/structs.md"
---

# Reading material

A Tour of Go: [Structs](https://go.dev/tour/moretypes/2). 
Go by Example: [Structs](https://gobyexample.com/structs), [Struc Embedding](https://gobyexample.com/struct-embedding).

---


## First exercise

```go

// structs1
// Make me compile!
//
// I AM NOT DONE
package main

import "fmt"

type Person struct {

}

func main() {
	fmt.Printf("Person %s and age %d", person.name, person.age)
}
```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/structs/structs1/main.go)
- [Playground](https://go.dev/play/p/28nP__rGMi2)
- [Solved](https://go.dev/play/p/KZSQgHNhbdF)

## Second exercise

```go
// structs2
// Make me compile!
//
// I AM NOT DONE
package main

import "fmt"

type Person struct {
	// don't just create the phone field here. embed a new struct
	name string
	age int
}

func main() {
	// contactDetails := ContactDetails{}
	person := Person{name: "John", age: 32}
	fmt.Printf("%s is %d years old and his phone is %s\n", person.name, person.age, person.phone)
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/structs/structs2/main.go)
- [Playground](https://go.dev/play/p/X2_qpQjgFwK)
- [Solved](https://go.dev/play/p/n5hPSw7qwRi)


## Third exercise

```go

// structs3
// Make me compile!
//
// I AM NOT DONE
package main

import "fmt"

type Person struct {
	firstName string
	lastName  string
}

func main() {
	person := Person{firstName: "Maurício", lastName: "Antunes"}
	fmt.Printf("Person full name is: %s\n", person.FullName()) // here it must output Person full name is: Maurício Antunes
}

```

- [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/structs/structs3/main.go)
- [Playground](https://go.dev/play/p/2v9TNGglQB8)
- [Solved](https://go.dev/play/p/hXUIB-Qpn8w)
