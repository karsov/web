---
title: "The highlights of the past week"
date: 2023-02-04
---

Let me share a couple of topics I found interesting during the week:

**Go 1.20**

Go 1.20 was just released:  https://go.dev/blog/go1.20 
Among the standard performance improvements a few cool things you can now do are added:
- Create code coverage reports of whole running applications: [https://go.dev/testing/coverage/](https://go.dev/testing/coverage/)
- Join multiple errors: [https://pkg.go.dev/errors#Join](https://pkg.go.dev/errors#Join) 
- Cancel a context with a given error: [https://pkg.go.dev/context#WithCancelCause](https://pkg.go.dev/context#WithCancelCause)


**Golang dependencies**

Did you know that you can check what is the source of an indirect dependency with a single command?
It is `go mod why -m the-full-name-of-the-module`
Obviously this command has been available since Go 1.11!


**Golang Workspaces**

Go Workspaces are a way to make your local development in a monorepo easier.
They were introduced in Go 1.18 and here is a nice short introduction:
[https://earthly.dev/blog/go-workspaces/](https://earthly.dev/blog/go-workspaces/)


**Lean coffee**

Lean coffee is an interesting way to organise agendaless meetings.
The participants vote for the topics in the beginning and each topic has limited time.
https://leancoffee.org/ 


**Ngrok**

Have you ever wanted to add a public endpoint for a service running on your local machine (for example for webhook testing)
or an edge device behind many firewalls?
A very nice and simple solution is using Ngrok ( [https://ngrok.com/docs/getting-started/](https://ngrok.com/docs/getting-started/) ) - an agent
running on your machine and creating a tunnel between your machine and the public endpoint.


**Multi-document YQ**

Did you know that “yq” can work with multiple separate documents in a single file (like multiple K8s manifest in deploy.yaml)?
It can even filter on which specific document you want to work on:
[https://mikefarah.gitbook.io/yq/operators/document-index#filter-by-document-index](https://mikefarah.gitbook.io/yq/operators/document-index#filter-by-document-index) 
