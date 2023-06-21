---
title: "The highlights of the past week"
date: 2023-06-21
---

As we head into summer, news seems to become less abundant, and my updates may become less frequent. However, I've gathered some important recent releases, an AWS outage,
and an interesting debugging story for you. Don’t forget to check the comments for the mandatory #Golang bonus tip.

🎉 The MariaDB community server released its next major version 11. It features big improvements to the query optimizer and extensive code cleanup causing breaking changes.
Find all the details in the official announcement:
[https://mariadb.com/resources/blog/announcing-mariadb-community-server-11-0-ga-and-11-1-rc/](https://mariadb.com/resources/blog/announcing-mariadb-community-server-11-0-ga-and-11-1-rc/)

📈 Exciting news from the #OpenTelemetry project as they announced the first stable release of the OpenTelemetry Golang Metrics API with opentelemetry-go v1.16.0.
Now the progress continues with stabilising the Golang Metrics SDK. Check out the release notes for more information:
[https://github.com/open-telemetry/opentelemetry-go/releases/tag/v1.16.0](https://github.com/open-telemetry/opentelemetry-go/releases/tag/v1.16.0)

💥 AWS experienced their first major outage in a while when multiple services in the “us-east-1” region went down on June 13th for around 3 hours.
The incident brought down multiple websites and mobile apps (and even vacuum cleaners), and it sheds light on the importance of that specific region within the global AWS service.
Read more about it here:
[https://www.theverge.com/2023/6/13/23759857/amazon-aws-down-outage-taco-bell-mcdonalds-burger-king](https://www.theverge.com/2023/6/13/23759857/amazon-aws-down-outage-taco-bell-mcdonalds-burger-king)

🤓 Wrapping up with my recommendation for a long read, Chris Sinjakli, an infrastructure engineer at PlanetScale, shared his team’s challenging debugging journey
when a whole PostgreSQL cluster failed. His article not only delves into the specific problems they had to solve but also shares valuable general debugging tips.
Dive into the details here:
[https://www.infoq.com/articles/debugging-beneath-trusted-abstraction/](https://www.infoq.com/articles/debugging-beneath-trusted-abstraction/)


**Bonus #Golang tip:** Experience is the most effective way to enhance your Go programming skills.
However, there is a shortcut to gaining experience - learning from others who already went down that path. Vadym Fedorov recently shared a great resource which may save you months,
if not years, in learning all the good practices and useful tips listed in it. Explore it at:
[https://github.com/cristaloleg/go-advice](https://github.com/cristaloleg/go-advice)
