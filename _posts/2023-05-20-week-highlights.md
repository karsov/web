---
title: "The highlights of the past week"
date: 2023-05-20
---

This week, I want to share some recent #observability developments, a bit of architecture, and touch on the topic that seems everywhere these days - AI.
Don't forget to check out the comments for the bonus #Golang tip!

💥 Gergely Orosz published an in-depth analysis of a global outage that lasted a whole day for one of the biggest observability service providers, Datadog, back in March.
While such postmortems are always great learning resources, it is strange that a person outside of the company had to write it in this case.
Interestingly, a few hours after his publication, Datadog finally published their postmortem.\
Check Gergely’s analysis here: [https://newsletter.pragmaticengineer.com/p/inside-the-datadog-outage](https://newsletter.pragmaticengineer.com/p/inside-the-datadog-outage)\
and DataDog’s official post here: [https://www.datadoghq.com/blog/2023-03-08-multiregion-infrastructure-connectivity-issue/](https://www.datadoghq.com/blog/2023-03-08-multiregion-infrastructure-connectivity-issue/)

📈 The world’s first generative AI assistant for observability (according to the official announcement), New Relic Grok, was released for early access.
New Relic, Inc. claims that if you are using their platform for all your monitoring data this new assistant can identify the root cause for an issue and
even suggest a code fix for the bug that caused it, all by plain human language queries. Check out the announcement here:
[https://newrelic.com/blog/nerdlog/new-relic-grok](https://newrelic.com/blog/nerdlog/new-relic-grok)

🤖 While on the AI topic, I came across another great use of generative AI - video summarisation.
The idea is that a model can produce a single paragraph summary from an hour-long video saving you loads of time. While there are several applications doing this already,
I’ve tried only [https://www.summarize.tech/](https://www.summarize.tech/) because it can do the most for free and without requiring an account.
Other popular tools are [https://kagi.com/summarizer/](https://kagi.com/summarizer/) and [https://www.you-tldr.com/](https://www.you-tldr.com/)

🤔 In a recent blog post, the Amazon Prime video engineering team fueled the microservices vs monolith debate by sharing how they reduced costs and
improved scalability by moving to a monolith architecture for a specific feature. While some may argue that this proves monoliths are superior,
I see it as an excellent example that the architecture should be flexible and not set in stone. Sometimes monoliths are better, and other times - microservices;
it depends on your requirements. It is normal for your architecture to evolve as requirements change. Read about the Prime Video team's learnings here:
[https://www.primevideotech.com/video-streaming/scaling-up-the-prime-video-audio-video-monitoring-service-and-reducing-costs-by-90](https://www.primevideotech.com/video-streaming/scaling-up-the-prime-video-audio-video-monitoring-service-and-reducing-costs-by-90)

💸 Confluent, the company founded by the original creators of Apache Kafka and now providing an enterprise-grade, zero-ops cloud-native platform for Kafka, issued a challenge.
They claim to offer a lower price compared to running open-source Kafka on your own (or $100 on them). Check out the challenge here:
[https://www.confluent.io/blog/understanding-and-optimizing-your-kafka-costs-part-4-savings-challenge/](https://www.confluent.io/blog/understanding-and-optimizing-your-kafka-costs-part-4-savings-challenge/)


**Bonus #Golang tip:** The “go test” tool usually executes the tests in different packages concurrently to save you time and CI bill.
You can force parallel execution within a single package too by calling “t.Parallel()” in your tests. However, sometimes executing tests in parallel can lead to unexpected errors.
If you want to ensure serial execution of packages, use the “-p 1” CLI argument. For serial execution within a package, use “-parallel 1”.
