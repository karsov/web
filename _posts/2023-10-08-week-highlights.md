---
title: "The highlights of the past week"
date: 2023-10-08
---

Some big news was announced in the tech world lately, from big changes for Splunk, to new AI-related developments.
Keep reading to stay up-to-date with the latest in tech, and don't miss my bonus #Golang tip.

🚀 Cisco is acquiring Splunk for a whopping $28 billion! This is Cisco's biggest acquisition to date and possibly the largest in the #observability space.
While the deal will certainly expand Splunk’s security and observability solutions reach, it will be interesting to see how the merger of these two giants comes along and
what other changes it will bring.

☁️ Cloudflare presented several new AI offerings: Workers AI is a serverless AI inference as a service platform, allowing you to run AI models really easy
on Cloudflare’s global network of GPUs, Vectorize - a vector databases designed to work seamlessly with Workers AI, and an “AI gateway” adds features like
caching, rate-limiting, analytics and logging.

🗣 OpenAI is introducing image input and voice conversations to #ChatGPT. This brings it into direct competition with existing popular tools like Apple’s Siri and Google’s voice assistant,
and as we all know - the more competition there is the better it is for consumers.

🤖 Anthropic, the creators of the popular AI assistant Claude, secured a $4 billion investment by Amazon. The deal comes with a point that
Amazon Web Services (AWS) will become Anthropic’s primary cloud provider, which may come as a surprise to some since earlier this year they shared their choice of
Google Cloud as a cloud provider.

🤓 And to end on an educational note, in a new blog post Adriano Caloiaro raises a good point about choosing “boring” technologies (like #PostgreSQL or #MariaDB)
for your queue implementation. While the post is specifically for Postgres, in my team we’ve been using MariaDB’s “SELECT ... FOR UPDATE SKIP LOCKED” since it was added 2 years ago
and it's a relief not having to manage yet another tech for our job queues.

Bonus Golang tip: Did you know that since Go 1.16 there is an “embed” package in the standard library? It allows you to embed files in your binaries during compilation and
later access them via a simple standard interface.

---

If you want to read more about these week’s topics check the following links:

Splunk’s acquisition:
[https://www.reuters.com/markets/deals/cisco-acquire-splunk-28-billion-2023-09-21/](https://www.reuters.com/markets/deals/cisco-acquire-splunk-28-billion-2023-09-21/)\
Cloudflare’s new AI additions:
[https://www.cloudflare.com/en-gb/press-releases/2023/cloudflare-launches-workers-ai-deploy-ai-inference/](https://www.cloudflare.com/en-gb/press-releases/2023/cloudflare-launches-workers-ai-deploy-ai-inference/)\
Open AI adds image input and voice conversations:
[https://openai.com/blog/chatgpt-can-now-see-hear-and-speak](https://openai.com/blog/chatgpt-can-now-see-hear-and-speak)\
Amazon invests in Anthropic:
[https://www.anthropic.com/index/anthropic-amazon](https://www.anthropic.com/index/anthropic-amazon)\
Adriano Caloiaro: Choose Postgres queue technology:
[https://adriano.fyi/posts/2023-09-24-choose-postgres-queue-technology/](https://adriano.fyi/posts/2023-09-24-choose-postgres-queue-technology/)\
The Go “embed” package:
[https://pkg.go.dev/embed](https://pkg.go.dev/embed)
