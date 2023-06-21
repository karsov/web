---
title: "The highlights of the past week"
date: 2023-06-03
---

This week, I’ve gathered a combination of exciting news, educational articles and new handy tools. Read on to discover more and don’t miss the #Golang tip in the comments.

🎉 Starting off with big news from the company I’m working for, MariaDB announced a new era with the appointments of new CEO & CTO and an ambitious growth plan.
Check out the official press release here:
[https://mariadb.com/newsroom/press-releases/mariadb-announces-new-management-appointments/](https://mariadb.com/newsroom/press-releases/mariadb-announces-new-management-appointments/)

🧙‍♂️ A great find for me was the #mirrord tool. While I’ve previously used #telepresence to run and debug applications on my local maching as if they are running in #Kubernetes,
it needs some tinkering to make it work as desired. mirrord, on the other hand, works like magic - you run a single CLI command (you can use VS Code or IntelliJ too) and that’s it.
All you need is kubectl access to your cluster. Check its quick start guide for details:
[https://mirrord.dev/docs/overview/quick-start/](https://mirrord.dev/docs/overview/quick-start/)

🤓 In an educational article, Nicholas Ray shared how small JavaScript changes significantly reduced Wikipedia's total blocking time. Read all about it on his blog:
[https://www.nray.dev/blog/300ms-faster-reducing-wikipedias-total-blocking-time/](https://www.nray.dev/blog/300ms-faster-reducing-wikipedias-total-blocking-time/)

💡 Aviator, a developer workflow automation tools provider, demonstrated an interesting application of the #Cortex Query Frontend. They used it as a #Prometheus query cache,
and not as a part of the standard Cortex installation. Learn how you can do it at (it might work with #Thanos Query Frontend too):
[https://www.aviator.co/blog/improve-query-performance-cortex-query-frontend/](https://www.aviator.co/blog/improve-query-performance-cortex-query-frontend/)

📈 And finally, I stumbled upon a valuable collection of #observability tools at https://o11y.tools/ . It contains a PromQL parser, /metrics linter, and many more,
making your life working with Prometheus metrics easier.


**Bonus #Golang tip**: There are many ways to selectively run Go tests. You can use regular expressions to match specific test names with `go test -run regexp`,
or skip them with `go test -skip regexp`. In the code, you can use `t.Skip()` to skip a test. Additionally, you can check if `go test -short` was run by calling `testing.Short()`,
allowing you shorten the testing. And if you don’t want to modify your tests’ code, you can place your slow integration tests in a separate file with a build flag defined in the beginning.
Thus, these tests will be only execute if the build flag is explicitly mentioned, for example: `go test -tags=integration`.
