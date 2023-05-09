---
title: "The highlights of the past week"
date: 2023-05-09
---

Last week I had an interesting mixture of news and educational resources that I want to share with you.
Read on for more information, and make sure to check the #Golang tip in the comments about an easy to miss memory leak.

🎉 A big milestone for the OpenTelelemetry project and the whole #observability space was reached with the announcement of feature parity with OpenCensus and sunsetting the latter.
As a result, 4 years after the merger of OpenTracing and OpenCensus into OpenTelemetry, all OpenCensus GitHub repositories will be archived on July 31st, 2023.
Learn more about it at:
[https://opentelemetry.io/blog/2023/sunsetting-opencensus/](https://opentelemetry.io/blog/2023/sunsetting-opencensus/)

🔐 In other news, Google declared the beginning of the end of passwords by rolling out support for passkeys across Google Accounts.
Passkeys allow you to sign in to apps and websites using a fingerprint, a face scan or a screen lock PIN on your mobile device.
While this new way of authentication is generally easier to use and more secure, some users have expressed concerns about losing access to their accounts
by losing the mobile device or authentication handler blocking them out of their important accounts. Check out the Google announcement here:
[https://blog.google/technology/safety-security/the-beginning-of-the-end-of-the-password/](https://blog.google/technology/safety-security/the-beginning-of-the-end-of-the-password/)

📺 Moving on to the educational resources, the video recordings from KubeCon + CloudNativeCon Europe 2023 have just been released!
You can find the playlist for the main track here:
[https://www.youtube.com/playlist?list=PLj6h78yzYM2PyrvCoOii4rAopBswfz1p7](https://www.youtube.com/playlist?list=PLj6h78yzYM2PyrvCoOii4rAopBswfz1p7)
and for Observability Day Europe 2023 here:
[https://www.youtube.com/playlist?list=PLj6h78yzYM2ORxwcjTn4RLAOQOYjvQ2A3](https://www.youtube.com/playlist?list=PLj6h78yzYM2ORxwcjTn4RLAOQOYjvQ2A3)

💡 I came across an insightful post by Vadim Kravcenko on rules of thumb for software development estimations.
If you want to learn more about this important aspect of software development, check it out here:
[https://vadimkravcenko.com/shorts/project-estimates/](https://vadimkravcenko.com/shorts/project-estimates/)

🤔 Finally, I was amused to discover that #PostgreSQL has a dedicated page describing to its users which of its numerous features they shouldn’t use!
You can find it here:
[https://wiki.postgresql.org/wiki/Don%27t_Do_This](https://wiki.postgresql.org/wiki/Don%27t_Do_This)


**Bonus #Golang tip:** Timers and tickers from the Golang standard library are the most common way to execute actions at specific times.
However, make sure to double-check the docs so that they are used correctly and recovered by the garbage collector to prevent memory leaks.
ArangoDB learned this the hard way:
[https://www.arangodb.com/2020/09/a-story-of-a-memory-leak-in-go-how-to-properly-use-time-after/](https://www.arangodb.com/2020/09/a-story-of-a-memory-leak-in-go-how-to-properly-use-time-after/)
