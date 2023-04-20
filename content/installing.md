---
title: "Installing"
date: 2023-04-20T01:39:18-03:00
draft: false
pageSource: "https://github.com/Grubba27/golings-site/blob/main/content/installing.md"
---

> This is the installing section from the [GitHub repo](https://github.com/mauricioabreu/golings/blob/main/README.md).

First, you need to have `go` installed. You can install it by visiting the [Go downloads page](https://go.dev/dl/)

There are two ways to install `golings`

### go install

```sh
go install github.com/mauricioabreu/golings/golings@latest
```

### Binaries

Go to the [releases page](https://github.com/mauricioabreu/golings/releases) and choose the option that best fits your environment.

## Doing exercises

All the exercises can be found in the directory `golings/exercises/<topic>`. For every topic there is an additional README file with some resources to get you started on the topic. We really recommend that you have a look at them before you start.

Now you have the task to fix all the programs. Some of them don't compile, and you need to fix them. Some of them compile, but have tests and you need to write some code to have them all green (these are the `compile` and `test` modes).

#### Clone the repository:

```sh
git clone git@github.com:mauricioabreu/golings.git
```

#### To run the next pending exercise:

```sh
golings run next
```

#### If you want to run a single exercise:

```sh
golings run variables1
```

#### In case you are stuck and need a hint:

```sh
golings hint variables1
```

#### To list all exercise while checking your progress:

```sh
golings list
```

#### To compile and run all the exercises:

```sh
golings verify
```

#### If you need help with CLI commands:

```sh
golings --help
```


## Learning resources

1. [Golang official tutorial](https://go.dev/doc/tutorial/)
2. [Go by example](https://gobyexample.com)
3. [Aprenda Go](https://www.youtube.com/playlist?list=PLCKpcjBB_VlBsxJ9IseNxFllf-UFEXOdg)

## Other 'lings

1. [rustlings](https://github.com/rust-lang/rustlings)
2. [ziglings](https://github.com/ratfactor/ziglings)