---
title: "The highlights of the past week"
date: 2023-07-08
---

Despite that the summer is heating up and the tech world is slowing down, there have been a couple of significant news items in the past two weeks that I'd like to share.
Keep reading to learn more and check the comments for a bonus #Golang tip.

💥 The Linux open-source community was angered by Red Hat's decision to limit access to the Red Hat Enterprise Linux (RHEL) source code,
making it available only through their customer portal. This change not only hinders the creation of RHEL-compatible distributions like AlmaLinux and Rocky Linux
but also poses challenges for individual app developers supporting RHEL. Many even believe that Red Hat is violating the GPLv2 licence.
Learn more about the matter in this excellent ZDNET article:
[https://www.zdnet.com/article/red-hats-new-rule-open-source-betrayal/](https://www.zdnet.com/article/red-hats-new-rule-open-source-betrayal/)

🎉 In a surprising turn of events, Squarespace announced that they are acquiring Google Domains, the third largest domain registrar.
This unexpected news has triggered a wave of transfers to other registrars by Google Domains' customers. To find out more, read the in-depth analysis on Gergely Orosz’s blog:
[https://blog.pragmaticengineer.com/google-domains-to-shut-down/](https://blog.pragmaticengineer.com/google-domains-to-shut-down/)

💡 37signals, the inventors of Ruby on Rails and makers of Basecamp and HEY, shared an interesting achievement - they've now completed their cloud exit.
This comes at a time when the world is increasingly embracing cloud technologies. They estimate that their entire infrastructure on self-owned hardware in two data centres
saves them $1.5 million per year compared to their previous AWS bills, all without expanding their operations team. Discover more about it here:
[https://world.hey.com/dhh/we-have-left-the-cloud-251760fb](https://world.hey.com/dhh/we-have-left-the-cloud-251760fb)

📈 And finishing up with #observability, the next LTS (Long-Term Support) release of Prometheus, version 2.45, is out! It comes with a bunch of incremental improvements and
guarantees at least 12 months of fixes and support. Explore the release notes for more details:
[https://github.com/prometheus/prometheus/releases/tag/v2.45.0](https://github.com/prometheus/prometheus/releases/tag/v2.45.0)

**Bonus #Golang tip:** Sometimes you may need to perform additional setup or teardown tasks when running all your tests.
In Go, you can put that auxiliary code in a TestMain function defined for every package that needs the extra functionality.
Great examples for using the TestMain functionality are tasks like creating and cleaning up the Docker containers on which your tests depend on,
or checking for leaked goroutines in your code.
