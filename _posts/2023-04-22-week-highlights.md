---
title: "The highlights of the past week"
date: 2023-04-22
---

While I was busy watching as many sessions as possible from KubeCon + CloudNativeCon Europe 2023 in Amsterdam this week
(thankfully, recordings are available), I also came across other noteworthy news.
Check out the highlights below, plus (in the comments) a bonus #Golang tip that could have prevented a production issue for my team this week!

📣 The biggest news from #KubeCon for me was the convergence of Elastic Common Schema and OpenTelemetry Semantic Convention into a single open schema.
Once completed, having one single standard will help boost the #observability ecosystem and make working with telemetry data easier.
Check out the official announcement here:
[https://opentelemetry.io/blog/2023/ecs-otel-semconv-convergence/](https://opentelemetry.io/blog/2023/ecs-otel-semconv-convergence/)

🎉 In other news, Cortex - the #CNCF project providing horizontally scalable long term storage for Prometheus metrics, released version 1.15,
which comes with out-of-order samples ingestion and many other improvements. You can find all the changes in the release notes here:
[https://github.com/cortexproject/cortex/releases/tag/v1.15.0](https://github.com/cortexproject/cortex/releases/tag/v1.15.0)

💡 For those interested in system design, Slack engineering shared a blog post on the architecture of their platform
serving real-time messages across the world. You can read it all here:
[https://slack.engineering/real-time-messaging/](https://slack.engineering/real-time-messaging/)

💻 And finally, if you are looking into expanding your Apache Kafka knowledge, I just found out that Confluent created a 100 Days Of Code program
to help anyone ramp up their skills in the area. Check it out here:
[https://developer.confluent.io/100-days-of-code/](https://developer.confluent.io/100-days-of-code/)


**Bonus #Golang tip:** Always run linters before releasing your code! You can do that as a Git hook or in your CI pipeline (best - in both places).
Linters can save you from a lot of common errors that cause panics, memory leaks, etc. golangci-lint is probably the best tool for the purpose.
You can see how to use it here: [https://golangci-lint.run/](https://golangci-lint.run/)
