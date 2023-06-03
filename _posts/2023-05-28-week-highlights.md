---
title: "The highlights of the past week"
date: 2023-05-28
---

This week I’ve gathered some exciting updates on container tooling and #observability. Keep reading to learn more about it, along with the bonus #Golang tip in the comments.

First up, Red Hat released Podman Desktop, a user-friendly UI desktop application that provides an alternative to Docker Desktop and Rancher Desktop
for building, pushing, and pulling images, running containers, and working with Kubernetes on your local machine. Read more about it in the official release post:
[https://developers.redhat.com/articles/2023/05/23/podman-desktop-now-generally-available](https://developers.redhat.com/articles/2023/05/23/podman-desktop-now-generally-available)

Continuing with containers, The New Stack published an excellent article on enhancing your Docker images by using Dockerfile linting,
image security audit and image size minimisation tools. Dive into the details here:
[https://thenewstack.io/four-ways-to-enhance-your-dockerfiles/](https://thenewstack.io/four-ways-to-enhance-your-dockerfiles/)

Shifting the focus to observability, Julius Volz released a great video introduction to the PromQL basics.
Make sure you have the foundations right by checking out the video here:
[https://www.youtube.com/watch?v=xIAEEQwUBXQ](https://www.youtube.com/watch?v=xIAEEQwUBXQ)

In a significant strategic move Timescale, the company behind TimescaleDB, the time-series-optimised SQL database packaged as a PostgreSQL extension,
announced a transition from a database company with a cloud product to a cloud company with a database product.
They will now concentrate their development focus on their cloud offering adding only part of its new features to the PostreSQL extension.
Discover more about their new branding and development focus in their blog post:
[https://www.timescale.com/blog/announcing-the-new-timescale/](https://www.timescale.com/blog/announcing-the-new-timescale/)

And to finish the week with a bit of AI, honeycomb.io recently introduced an experimental AI query assistant to their observability platform,
allowing you to write queries in plain English instead of learning yet another domain-specific language. Find out more in their announcement here:
[https://www.honeycomb.io/blog/introducing-query-assistant](https://www.honeycomb.io/blog/introducing-query-assistant)


**Bonus #Golang tip:** Using containers for external dependencies during testing can enhance application compatibility, integration and end-to-end tests.
While you can prepare the test setup with Docker Compose, this complicates your job by adding yet another step to the processes.
Testcontainers is a library that solves this by allowing you to start the containers within your tests, making “go test” the only tool you need. Learn how to use it at:
[https://golang.testcontainers.org/quickstart/](https://golang.testcontainers.org/quickstart/)
