---
title: "The highlights of the past week"
date: 2023-03-18
---

This week was packed with big tech news! From big AI to DockerHub announcement mishaps and an observability scene acquisition.

The biggest thing for me was Docker sending an email to all DockerHub free team organisations that they will be deleted,
if they do not upgrade to a paid team plan within less than 1 month from now!
This obviously affects a lot of open-source projects and their millions of users and after a massive outcry
( you can check Hacker News here: https://news.ycombinator.com/item?id=35154025 and here: https://news.ycombinator.com/item?id=35166317 )
Docker apologised for the "miscommunication" and told that
"public images will only be removed from Docker Hub if their maintainer decides to delete them":
https://www.docker.com/blog/we-apologize-we-did-a-terrible-job-announcing-the-end-of-docker-free-teams/

🤖 You may have seen that OpenAI released this week GPT-4 with even more amazing capabilities ( if not, check here: https://openai.com/research/gpt-4 )
but the big thing for me as a language learning geek is that Duolingo announced
that they've already started using it to provide a better language learning experience: https://blog.duolingo.com/duolingo-max/

📈 And the big news for anyone interested in observability was that Grafana Labs acquired the continuous profiling project Pyroscope
and will be merging it with its own profiling tool Grafana Phlare under a new name - Grafana Pyroscope:
https://grafana.com/blog/2023/03/15/pyroscope-grafana-phlare-join-for-oss-continuous-profiling/

... and that's enough big news for me. Now some educational resources:

🤓 I was reminded this week of this great series of blog posts from Confluent on diagnosing and debugging Apache #Kafka issues:
https://www.confluent.io/blog/debug-apache-kafka-reduced-message-throughput/

💡 ngrok presented a very interesting concept - ingress as a #Golang application library.
With its open-source library you can have a secure public endpoint without having to deploy a separate agent application:
https://ngrok.com/blog-post/ngrok-go
