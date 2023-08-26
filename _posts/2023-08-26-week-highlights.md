---
title: "The highlights of the past week"
date: 2023-08-26
---

It's remarkable how many significant tech events affecting countless individuals and companies have occurred since my last post.
From #Terraform to #Vim, and #AWS pricing changes - there's a lot to catch up on. Even #Golang has seen so many interesting recent developments that
I'll publish a dedicated Go post in the coming days.

💥 HashiCorp changing overnight the licence for all its products, including #Terraform, #Vault, #Consul, #Nomad, from the open-source MPL v2 to the competition restricting BSL v1.1
is definitely the biggest thing these days. This shift has sparked big discussions, particularly around Terraform, one of the standard tools for infrastructure as code.
While some support HashiCorp in their right to do so, for others this is not right because the tool has definitely gained popularity from being open source.
Therefore, a group of companies led by Gruntwork and Spacelift published the OpenTF manifesto - a plan and pledge to keep Terraform open source forever and
first asked HashCorp to revert the licence change. Since the day the manifesto was published, HashiCorp hasn’t given any signs for reversal,
so the #OpenTF initiative just announced yesterday that it is forking Terraform!

🕯 Another thing that may soon affect millions, is the passing away of the creator and benevolent dictator of #Vim, one of the most popular text editors of all time.
Vim can be found on practically all operating systems and is loved and hated by many people, a source of many memes, and is certainly my favourite editor.
The ownership of the Vim project is already transferred to other people, so it will continue its life, but we are yet to see where the new maintainers will steer it.

💰 #AWS also announced a change that will influence many companies’ and individuals’ bills. Starting February 1, 2024, charges will be applied to all public IPv4 addresses
assigned to AWS resources. With IPv4 addresses becoming increasingly scarce and expensive in recent years, this change is yet another encouragement to adopt IPv6
as a modernization and cost-cutting measure.

🤓 The #Python Steering Council posted a notice about their intention to accept a proposal for making the global interpreter lock optional in CPython,
the default and most widely used implementation of the Python language. This change will allow CPU-bound multi-threaded applications to really execute in parallel on multi-core processors,
thus increasing their performance greatly. The improvement promises to be so significant that even Meta already committed to support it in the form of three engineer-years.

🎉 #Kubernetes version 1.28 has been released. Among many others, the most notable changes seem to be the increase of the supported skew between control plane and worker node versions
to 3 minor versions, and the alpha release of a restartPolicy field for init containers which is used to indicate when an init container is also a sidecar container,
thus introducing a mode similar to a background container.

🎂 Celebrating a significant milestone, #Debian, one of the most popular Linux distributions, recently turned 30 years old!
It’s nice to see that one of the first Linux flavours I tried about 20 years ago is still going strong.

🤖 Wrapping up with a touch of #observability, Datadog joined the generative AI train by introducing their own DevOps copilot, “Bits AI”.
The tool provides a conversational interface that not only can help you investigate issues more efficiently by correlating data from across the Datadog platform,
but can also suggest automated code fixes, synthetic tests, and relevant Datadog workflows.

---

If you are interested in reading more about the topics I shared here, check these resources:

HashiCorp licence change announcement:
[https://www.hashicorp.com/blog/hashicorp-adopts-business-source-license](https://www.hashicorp.com/blog/hashicorp-adopts-business-source-license)\
Gruntwork’s reasoning behind creating the OpenTF initiative:
[https://blog.gruntwork.io/the-future-of-terraform-must-be-open-ab0b9ba65bca](https://blog.gruntwork.io/the-future-of-terraform-must-be-open-ab0b9ba65bca)\
The OpenTF Manifesto: [https://opentf.org/](https://opentf.org/)\
Announcement for OpenTF forking Terraform: [https://opentf.org/announcement](https://opentf.org/announcement)\
AWS IPv4 pricing change:
[https://aws.amazon.com/blogs/aws/new-aws-public-ipv4-address-charge-public-ip-insights/](https://aws.amazon.com/blogs/aws/new-aws-public-ipv4-address-charge-public-ip-insights/)\
Python Steering Council's decision:
[https://discuss.python.org/t/a-steering-council-notice-about-pep-703-making-the-global-interpreter-lock-optional-in-cpython/30474](https://discuss.python.org/t/a-steering-council-notice-about-pep-703-making-the-global-interpreter-lock-optional-in-cpython/30474)\
Meta’s commitment to the GIL change:
[https://discuss.python.org/t/a-fast-free-threading-python/27903/99](https://discuss.python.org/t/a-fast-free-threading-python/27903/99)\
The Kubernetes 1.28 release:
[https://kubernetes.io/blog/2023/08/15/kubernetes-v1-28-release/](https://kubernetes.io/blog/2023/08/15/kubernetes-v1-28-release/)\
Buoyant’s in-depth analysis on the k8s 1.28 sidecar containers enhancement:
[https://buoyant.io/blog/kubernetes-1-28-revenge-of-the-sidecars](https://buoyant.io/blog/kubernetes-1-28-revenge-of-the-sidecars)\
Debian's anniversary:
[https://bits.debian.org/2023/08/debian-turns-30.html](https://bits.debian.org/2023/08/debian-turns-30.html)\
DataDog's Bits AI press release:
[https://www.datadoghq.com/blog/datadog-bits-generative-ai/](https://www.datadoghq.com/blog/datadog-bits-generative-ai/)
