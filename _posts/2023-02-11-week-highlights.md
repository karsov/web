---
title: "The highlights of the past week"
date: 2023-02-11
---

It seems that last week was mostly about #Observability for me. A couple of things grabbed my attention:


**AWS Observability Best Practices**

I just stumbled upon this excellent guide on observability best practices by AWS:
[https://aws-observability.github.io/observability-best-practices/](https://aws-observability.github.io/observability-best-practices/)
It has a lot of useful both generic and AWS specific information.


**Big migrations**

Gergely Orosz does a thorough review of Khan Academy’s 3.5 year migration from Python monolith to multiple Go services:
[https://newsletter.pragmaticengineer.com/p/real-world-eng-8](https://newsletter.pragmaticengineer.com/p/real-world-eng-8)


**Fun fact**

Did you know that in Go strings are internally structs?
[https://go101.org/article/string.html](https://go101.org/article/string.html)


**Dynamic logging**

Dynamic logging is the ability to add log lines at runtime.
While there are already some professional solutions for interpreted languages (Lightrun, Rookout Live Logger),
for compiled languages like #Golang the functionality is just starting to appear thanks to eBPF:
[https://docs.pixielabs.ai/tutorials/custom-data/dynamic-go-logging/](https://docs.pixielabs.ai/tutorials/custom-data/dynamic-go-logging/)


**Distributed tracing**

#CNCF shared on their blog and excellent article by Tyk on distributed tracing and OpenTelemetry
[https://www.cncf.io/blog/2023/02/07/migrating-from-opentracing-to-opentelemetry/](https://www.cncf.io/blog/2023/02/07/migrating-from-opentracing-to-opentelemetry/) 
