---
title: "The highlights of the past week"
date: 2023-04-01
---

No big news this week, yay! Here is what caught my attention though:

💻 The proposal for adding structured logging in the #Golang standard library was recently accepted
( [https://github.com/golang/go/issues/56345#issuecomment-1470506816](https://github.com/golang/go/issues/56345#issuecomment-1470506816) ).
You can check the implementation in the experimental package, although it may undergo some changes before it lands in the standard library:
[https://pkg.go.dev/golang.org/x/exp/slog](https://pkg.go.dev/golang.org/x/exp/slog)

💡 While looking at the Golang experimental packages, I was surprised to find that there is an "event" package
( [https://pkg.go.dev/golang.org/x/exp/event](https://pkg.go.dev/golang.org/x/exp/event) ),
which reminded me of this very interesting talk on having observability without logs:
[https://www.infoq.com/presentations/event-tracing-monitoring/](https://www.infoq.com/presentations/event-tracing-monitoring/)

I recently found out about Dragonfly - a drop-in replacement for the Redis in-memory datastore
which boasts greater performance, scalability and operational ease.
You may want to check it at [https://dragonflydb.io/](https://dragonflydb.io/)

📈 Grafana Labs announced the schedule for the upcoming GrafanaCON 2023.
You can check it at [https://grafana.com/about/events/grafanacon/2023/](https://grafana.com/about/events/grafanacon/2023/)
