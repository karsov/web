---
title: "The highlights of the past week"
date: 2023-09-21
---

This week I’ve collected some major developments in the world of #observability, a big addition to #Neo4j, and an important change for #Golang on #AWS.

🎉 But first, the biggest news around is that #OpenTF, the recently announced #Terraform fork, just joined The Linux Foundation under a new name: OpenTofu.
It may come as a surprise that this happens only a few weeks after HashiCorp changed Terraform’s licence to limit competition,
but the energy behind the new project seems to make it poised for success.

🚀 Switching to a topic I’m really fond of, databases, Neo4j, the leading name in the graph DB space, added native vector search.
This feature comes at a time of surge in adoption of vector databases caused by the explosion of large language models (LLMs) popularity,
because they facilitate the integration of LLM responses with factual data.

📈 Moving on to observability, the next #Prometheus version, 2.47, was released with the addition of an OpenTelemetry ingestion endpoint, among many other improvements.
And don’t forget, the biggest Prometheus event #PromCon EU is coming next week (Sep 28-29) so book the time on your calendar and check the schedule in the comments below.

📊 Still on observability, Grafana Labs unveiled a public preview of Grafana Beyla, a new tool able to auto-instrument your application with HTTP request metrics and trace spans.
And because it’s using #eBPF all of that is done without any code changes and for a wide range of programming languages.
And there’s more - Grafana Pyroscope, their continuous profiling solution, reached version 1. This means that its integration into the Grafana ecosystem is now complete
after its acquisition in March. Now, the team boasts it is “the most efficient and scalable open source profiling database”.

💥 Finishing this week's post with Golang, if you are using AWS lambda with the “go1.x” runtime and missed the news, Amazon Web Services (AWS) is deprecating it by the end of the year
along with the Amazon Linux AMI’s end-of-life. While the new “provided.al2” runtime may offer better performance, it requires modifications on your end.
Find in the comments a nice InfoQ article summarising the community’s reaction to the deprecation.

---

Check these resources to discover more about the topics discussed above:

Linux Foundation announces OpenTofu:
[https://www.linuxfoundation.org/press/announcing-opentofu](https://www.linuxfoundation.org/press/announcing-opentofu)\
Neo4j adds vector search:
[https://neo4j.com/blog/vector-search-deeper-insights/](https://neo4j.com/blog/vector-search-deeper-insights/)\
Prometheus 2.47 release notes:
[https://github.com/prometheus/prometheus/releases/tag/v2.47.0](https://github.com/prometheus/prometheus/releases/tag/v2.47.0)\
PromCon EU 2023 schedule:
[https://prometheus.io/blog/2023/09/01/promcon2023-schedule/](https://prometheus.io/blog/2023/09/01/promcon2023-schedule/)\
Grafana Beyla announcement:
[https://grafana.com/blog/2023/09/13/grafana-beyla-open-source-ebpf-auto-instrumentation/](https://grafana.com/blog/2023/09/13/grafana-beyla-open-source-ebpf-auto-instrumentation/)\
Grafana Pyroscope reaches version 1:
[https://grafana.com/blog/2023/08/29/grafana-pyroscope-1.0-release-continuous-profiling/](https://grafana.com/blog/2023/08/29/grafana-pyroscope-1.0-release-continuous-profiling/)\
AWS lambda Go runtime deprecation:
[https://www.infoq.com/news/2023/09/aws-lambda-go-deprecation/](https://www.infoq.com/news/2023/09/aws-lambda-go-deprecation/)
