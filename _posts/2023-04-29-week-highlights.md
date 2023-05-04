---
title: "The highlights of the past week"
date: 2023-04-29
---

This week was full of news and updates, ranging from cloud outages to new educational resources and AI tools.
Check out my summary below for the highlights, and don't miss the bonus #Golang tip in the comments.

💥 Probably the biggest event was the whole Google Cloud Paris region going down on Wednesday morning local time,
due to a “water intrusion” (and a fire!) in a single data centre. The outage lasted more than 24 hours, serving as a serious reminder
of the importance of multi-region operational resilience for any critical cloud application. This is especially true for GCP,
where they don’t have such strict region definitions as AWS (the Paris region seems to be located in a single data centre,
while in AWS a region consists of a minimum of three AZs, “physically separate by a meaningful distance, many kilometers, from any other AZ”).
Read more about the outage and its implications at:
[https://thenewstack.io/paris-is-drowning-gcps-region-failure-in-age-of-operational-resilience/](https://thenewstack.io/paris-is-drowning-gcps-region-failure-in-age-of-operational-resilience/)

🎉 On the bright side for Google Cloud, just a day before the Paris incident, they reported their first profit, 15 years after launching:
[https://www.theregister.com/2023/04/26/alphabet_q1_2023/](https://www.theregister.com/2023/04/26/alphabet_q1_2023/)

🤓 The most significant event in the #observability space was the release of version 1 of the Prometheus remote-write specification
(check Bartłomiej Płotka’s announcement here:
[https://groups.google.com/g/prometheus-announce/c/6xnGh7rcZKU](https://groups.google.com/g/prometheus-announce/c/6xnGh7rcZKU)).
Currently there are many remote-write implementations, so the specification aims to ensure that any sender or receiver
who claims Prometheus compatibility follows the same rules and best practices (for example, some sender may forget to send stale markers
when a time series will no longer be appended to, leading to increased memory usage for the receiver). Check the specification here:
[https://prometheus.io/docs/concepts/remote_write_spec/](https://prometheus.io/docs/concepts/remote_write_spec/)

🤖 Moving on to AI, this week I learned that people have started using large language models to save time on fixing #k8s issues.
For example, the “k8sgpt” tool ( [https://github.com/k8sgpt-ai/k8sgpt](https://github.com/k8sgpt-ai/k8sgpt) ),
combines the expertise of its creators in collecting the important information for your Kubernetes clusters, and leaves to the AI model
diagnosing and suggesting solutions to the found issues in plain English. Similarly, a KubeVela Workflow use of ChatGPT
as a k8s diagnostics & security audit tool and as s quality gate was demonstrated in a #CNCF blog post:
[https://www.cncf.io/blog/2023/04/25/promptops-in-application-delivery-empowering-your-workflow-with-chatgpt/](https://www.cncf.io/blog/2023/04/25/promptops-in-application-delivery-empowering-your-workflow-with-chatgpt/)

📖 Lastly, for anyone interested in databases, a new “Build Your Own Database” book was released last week.
Part I, dedicated to persistent KV stores and with code samples in #Golang, is freely available online. Check it out here:
[https://build-your-own.org/blog/20230420_byodb_done/](https://build-your-own.org/blog/20230420_byodb_done/)


**Bonus #Golang tip:** Don’t forget to use the built-in data race detector to catch difficult-to-debug memory corruption issues and inconsistent application behaviours. To enable it in your tests, simply add the “-race” flag to the “go test” command. You can catch even more issues if you build your binaries with enabled race detection. However, running in this mode significantly increases the memory usage and slows down the application execution, so you may not want to do this in production. To learn more about the race detector, check the Go docs:
[https://go.dev/doc/articles/race_detector](https://go.dev/doc/articles/race_detector)
