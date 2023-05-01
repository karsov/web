---
title: "The highlights of the past week"
date: 2023-03-04
---

A couple of new announcements and old but useful Go resources captured my attention last week.

Fly.io released for free a series of distributed systems programming challenges:
[https://fly.io/blog/gossip-glomers/](https://fly.io/blog/gossip-glomers/)

A #Kubernetes SIG (special interest group) backed by Apple introduced KWOK (Kubernetes WithOut Kubelet),
a tool for testing, development or simply learning, which simulates K8s using a fraction of the resources needed by existing tools:
[https://www.kubernetes.dev/blog/2023/03/01/introducing-kwok/](https://www.kubernetes.dev/blog/2023/03/01/introducing-kwok/)

A really good talk from QCon Plus was released publicly along with a transcript about API gateways,
sidecars and API documentation in the K8s microservices world:
[https://www.infoq.com/presentations/api-design-implement-document/](https://www.infoq.com/presentations/api-design-implement-document/)

I found an interesting blog post from a CockroachDB engineer going over their investigation on why #Golang executables can become large:
[https://dr-knz.net/go-executable-size-visualization-with-d3.html](https://dr-knz.net/go-executable-size-visualization-with-d3.html)

Did you know that... regular expressions in #Golang standard library are really slow.
Most probably you already know that but maybe you didn't know that there are libraries which can change the picture.
You can find them within Benchamarks game's comparison of multiple languages' regex performance comparison:
[https://benchmarksgame-team.pages.debian.net/benchmarksgame/performance/regexredux.html](https://benchmarksgame-team.pages.debian.net/benchmarksgame/performance/regexredux.html)
