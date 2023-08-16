---
title: "The highlights of the past week"
date: 2023-06-21
---

Although it’s already the vacation season, quite a few interesting news has emerged over the past two weeks.

💣 A month has passed since Red Hat limited access to its Red Hat Enterprise Linux (RHEL) source code and the initial anger to that decision has grown into real clone wars.
First it was Oracle who trash-talked Red Hat and presented itself as an open-source Linux champion compared to them, while still committing to maintain RHEL compatibility for Oracle Linux.
Then Suse dropped the bomb announcing that it is forking RHEL, trying to create a new enterprise Linux standard - an alternative to what RHEL has been for years.
One of the most popular RHEL clones, Rocky Linux, said that although they will continue to maintain RHEL compatibility they will support Suse’s efforts.
Only Alma Linux decided not to join the war and it will stop being an exact binary copy of RHEL.

🤖 Bard, the chatbot Google developed to rival OpenAI's ChatGPT, finally got released in Europe after being public in other parts of the world for a couple of months.
Having an alternative is important, especially now that researchers from Stanford University and UC Berkeley demonstrated a significant decline in ChatGPT’s response quality in recent times.

💥 InfluxDB Cloud customers in Belgium and Australia were surprised to find that their data had been permanently deleted without a backup.
It turns out that operations in the AWS Sydney and GCP Belgium regions were discontinued following a plan announced in February.
However, many customers were only contacted via emails which they never received. While some of the customer data was recovered,
this incident comes as a lesson on maintaining customers trust in handling their data and the importance of employing effective communication strategies, such as "scream tests",
to ensure that important messages reach everyone.

🎉 GitHub announced the public availability of merge queues, a feature designed to prevent your default branch from breaking when multiple people want to commit conflicting changes.
Using merge queues, when a new PR is added to the queue, a temporary branch is automatically created including all the changes from all the PRs in the queue.
Then a PR will only be merged if all the required status checks pass for it.

**Bonus #Golang tip:** The Go security team released version v1.0.0 of the official vulnerability scanning command-line tool, govulncheck.
Now that the tool and its APIs are stable, you can safely start using it in your CI pipelines to tap into its many advantages - tailor-made for Go,
using the Go vulnerability database, and also reducing noise by prioritising vulnerabilities in functions that your code is actually calling.

For more information on these news stories, check:

RHEL clone wars: [https://www.zdnet.com/article/almalinux-is-dropping-out-of-the-rhel-clone-wars/](https://www.zdnet.com/article/almalinux-is-dropping-out-of-the-rhel-clone-wars/)\
Google Bard: [https://bard.google.com/](https://bard.google.com/)\
ChatGPT quality deteriorating: [https://www.zdnet.com/article/gpt-4-is-getting-significantly-dumber-over-time-according-to-a-study/](https://www.zdnet.com/article/gpt-4-is-getting-significantly-dumber-over-time-according-to-a-study/)\
InfluxDB Cloud incident: [https://www.theregister.com/2023/07/11/influxdata_apologizes_for_ending_services/](https://www.theregister.com/2023/07/11/influxdata_apologizes_for_ending_services/)\
GitHub merge queues announcement: [https://github.blog/2023-07-12-github-merge-queue-is-generally-available/](https://github.blog/2023-07-12-github-merge-queue-is-generally-available/)\
Govulncheck v1.0.0 release: [https://go.dev/blog/govulncheck](https://go.dev/blog/govulncheck)
