---
title: "Anonymous functions"
date: 2023-04-16T21:46:07-03:00
draft: false
---


Hey this is the first lesson:

you can check it out [here](https://github.com/mauricioabreu/golings/blob/main/exercises/anonymous_functions/anonymous_functions1/main.go) 
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