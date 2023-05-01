---
title: "The highlights of the past week"
date: 2023-02-25
---

Here are the most educating things for me this week:

An interesting overview of some of the approaches to automatic instrumentation in #Golang was posted on the #CNCF blog
describing the Helios team’s approach for their #OpenTelemetry Go SDK:
[https://www.cncf.io/blog/2023/02/22/helping-go-teams-implement-opentelemetry-a-new-approach/](https://www.cncf.io/blog/2023/02/22/helping-go-teams-implement-opentelemetry-a-new-approach/)

I found this very useful project which emulates the #GCP Google Cloud Storage API.
It can be used as a #Golang library or as a standalone binary/Docker image, and I've already used it in my unit tests:
[https://github.com/fsouza/fake-gcs-server](https://github.com/fsouza/fake-gcs-server)

#AWS shared on their Open Source Blog a really useful #OpenTelemetry config validator CLI and GUI tool developed by Lightstep:
[https://aws.amazon.com/blogs/opensource/validating-opentelemetry-configuration-files-with-the-otel-config-validator/](https://aws.amazon.com/blogs/opensource/validating-opentelemetry-configuration-files-with-the-otel-config-validator/)

Did you know that... you can tell GitHub to ignore the whitespace in PR diffs making it way easier to see the differences
when the changes involve a lot of indentation modifications:
[https://github.blog/2018-05-01-ignore-white-space-in-code-review/](https://github.blog/2018-05-01-ignore-white-space-in-code-review/)

I knew previously about SSH tunneling but until this week I didn't know one can use the popular "gcloud compute ssh" command
to create a tunnel via a private #GCP VM instance (jump server) to access resources in a private network (or with IP access restrictions)
from the local machine. Just execute the following command and then you can connect to the remote service on "local-port" on localhost:

```shell
gcloud compute ssh vm-instance-name --project=your-project --zone=vm-instance-gcp-zone -- -NL local-port:remote-host:remote-port
```
