---
title: "Anonymous Functions"
date: 2023-04-16T21:46:07-03:00
draft: false
descripiton: "TODO"
exercises: "https://github.com/mauricioabreu/golings/tree/main/exercises/anonymous_functions"
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/exercises/anonymous_functions.md"
---


# Reading material:

Go by example: [Closures](https://gobyexample.com/closures)

A Tour of Go: [Closures](https://go.dev/tour/moretypes/25)

---


##  First exercise

```go
// anonymous functions1
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {

	func(name string) {
		fmt.Printf("Hello %s", name)
	}()

}
```
 - [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/anonymous_functions/anonymous_functions1/main.go) 
 - [Playground](https://go.dev/play/p/YmZRqjE3Cvo) 
 - [Solved](https://go.dev/play/p/ggJXZybLVom)


 ##  Second exercise

```go
// anonymous functions2
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func main() {
	var sayBye func(name string)

	sayBye = func() {
		fmt.Printf("Bye %s", n)
	}
}
```
 - [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/anonymous_functions/anonymous_functions2/main.go) 
 - [Playground](https://go.dev/play/p/7kLSnWwN4DJ) 
 - [Solved](https://go.dev/play/p/bBqoyklXiSn)


  ##  Third exercise

```go
// anonymous functions3
// Make me compile!

// I AM NOT DONE
package main

import "fmt"

func updateStatus() func() string {
	var index int
	orderStatus := map[int]string{
		1: "TO DO",
		2: "DOING",
		3: "DONE",
	}

	return func() string {
		index++
		return "What should I return?"
	}
}

func main() {
	anonymous_func := updateStatus()
	var status string

	status = anonymous_func()
	status = anonymous_func()

	if status == "DONE" {
		fmt.Println("Good Job!")
	} else {
		panic("To complete the challenge the status must be DONE")
	}
}
```
 - [Source code](https://github.com/mauricioabreu/golings/blob/main/exercises/anonymous_functions/anonymous_functions3/main.go) 
 - [Playground](https://go.dev/play/p/XQgkjjWqhwD) 
 - [Solved](https://go.dev/play/p/tuRE2AJu5vO)