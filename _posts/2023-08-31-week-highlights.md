---
title: "The highlights of the past week"
date: 2023-08-31
---

As promised, due to the significant number of recent #Golang news, I am thrilled to present you a special Go-themed post.

🚀 Go 1.21 was released! 🎉🎉🎉 This version comes with an incredible amount of new features - improvements in the tooling, language additions,
support for WASI and the addition of four highly anticipated packages to the standard library, alongside numerous other minor improvements.

Here are the highlights:
* The introduction of “min” and “max” built-in functions that work for ordered types, and a “clear” built-in function for maps and slices.
* A new package “log/slog” - finally we have a structured logging package in the standard library. This is one of the largest additions to the standard library since Go 1 was released in 2012! 
* A new package “slices” - for various useful functions on slices of any type. Plus, it includes a faster sort function for slices of “ordered” types.
* A new package “maps” - for common maps functions that you previously had to write on your own.
* A new package “cmp” - for types and functions facilitating ordered values comparison.
* An anticipated addition is the port to WASI, the WebAssembly System Interface for non-browser WebAssembly runtimes.
* Improved backwards compatibility by expanding and formalising the use of the GODEBUG environment variable. This aims to make the latest version of Go be the best possible implementation of older versions of Go.
* Improved forward compatibility by making the Go version defined in the go.mod file a minimum required Go toolchain version, while previously it was an unenforced suggestion, and by the introduction of toolchain management in the “go” command. Now you are not only able to use different Go toolchain versions for different modules but also the “go” command will automatically download them if they are not present on the machine. Thus, once you’ve installed Go 1.21, you’ll never have to manually download and install a Go toolchain again!

🤔 In another announcement, the Go team presented “gonew”, an experimental tool for instantiating new projects in Go from predefined templates.
A template can be any Go module, so currently “gonew” is simply a shorthand for “git clone --depth=1”, remove the ".git” folder, and
replace all references of the original module name with the new project’s name. While similar tools exist, it is interesting to see how “gonew” will evolve.

🔥 Google officially stopped supporting the standard Go mocking framework "github.com/golang/mock" and its repo was recently archived after not being updated for quite some time.
While there are some popular alternatives like "github.com/vektra/mockery", they are not as lightweight and introduce additional dependencies.
So I'm happy that the Uber Go team decided to fork the repo and invest in its maintenance. The initial version is an exact copy of the old library,
so to switch to it you simply have to run “go install go.uber.org/mock/mockgen@latest”, regenerate your mocks and replace all “github.com/golang/mock” references in your code
with “go.uber.org/mock”.

🤓 To conclude this dedicated Go post on an educational note, I want to share Eli Bendersky’s great article on common mistakes people make when using Go’s benchmarking tool.
From evaluating the speed of the wrong thing and forgetting to stop the timer around auxiliary code, to the compiler optimising away and even emptying the benchmark loop,
the article not only outlines the possible issues but also suggests solutions for fixing them. Find the link in the resources below to read the full write-up.

---

To learn more about the topics discussed in this post, check these resources:

Go 1.21 release notes:
[https://tip.golang.org/doc/go1.21](https://tip.golang.org/doc/go1.21)\
Introduction of the new structured logging package:
[https://go.dev/blog/slog](https://go.dev/blog/slog)\
Go’s backward compatibility:
[https://go.dev/blog/compat](https://go.dev/blog/compat)\
Go’s forward compatibility:
[https://go.dev/blog/toolchain](https://go.dev/blog/toolchain)

Uber’s fork of the standard Go mocking framework:
[https://github.com/uber-go/mock](https://github.com/uber-go/mock)

Introduction of the gonew tool:
[https://go.dev/blog/gonew](https://go.dev/blog/gonew)

Common pitfalls in Go benchmarking:
[https://eli.thegreenplace.net/2023/common-pitfalls-in-go-benchmarking/](https://eli.thegreenplace.net/2023/common-pitfalls-in-go-benchmarking/)
