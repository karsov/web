---
title: "The highlights of the past week"
date: 2023-03-11
---

Here are my highlights of the week - a couple of new announcements and a few older but very education resources:

Amazon Web Services (AWS) announced the general availability of their AWS Application Composer – a visual builder for serverless applications.
And it looks like a great tool not only for quick prototyping but also for generating diagrams or simply learning about serverless applications:
[https://aws.amazon.com/blogs/aws/aws-application-composer-now-generally-available-visually-build-serverless-applications-quickly/](https://aws.amazon.com/blogs/aws/aws-application-composer-now-generally-available-visually-build-serverless-applications-quickly/)

Cloudflare shared an excellent blog post describing not only how they handle high cardinality in Prometheus
but also going in depth on what metrics and time series are and how #Prometheus handles them internally:
[https://blog.cloudflare.com/how-cloudflare-runs-prometheus-at-scale/](https://blog.cloudflare.com/how-cloudflare-runs-prometheus-at-scale/)

🙁 The #Kubernetes Project announced that a tool I found very useful while I was starting with K8s, the free Katacoda Kubernetes tutorials,
is shutting down at the end of March:
[https://kubernetes.io/blog/2023/02/14/kubernetes-katacoda-tutorials-stop-from-2023-03-31/](https://kubernetes.io/blog/2023/02/14/kubernetes-katacoda-tutorials-stop-from-2023-03-31/)

If you've never heard of container checkpointing, it allows you to write to a file on the disk the state of a running container (including memory!)
in order for it to be restored or analysed later. Sysdig has a great article going into further details on what was added in Kubernetes 1.25
along with a lot of other useful resources:
[https://sysdig.com/blog/forensic-container-checkpointing-dfir-kubernetes/](https://sysdig.com/blog/forensic-container-checkpointing-dfir-kubernetes/)

🤓 I found this interesting read on something #Golang devs don't usually think a lot, the goroutines size:
[https://tpaschalis.me/goroutines-size/](https://tpaschalis.me/goroutines-size/)
