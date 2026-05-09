---
title: "How Zapier uses KEDA"
url: "https://keda.sh/blog/2022-03-10-how-zapier-uses-keda/"
date: "2022-03-10"
author: ""
feed_url: "https://keda.sh/blog/index.xml"
---
RabbitMQ is at the heart of Zap processing at Zapier. We enqueue messages to RabbitMQ for each step in a Zap. These messages get consumed by our backend workers, which run on Kubernetes. To keep up with the varying task loads in Zapier we need to scale our workers with our message backlog. For a long time, we scaled with CPU-based autoscaling using Kubernetes native Horizontal Pod Autoscale (HPA), where more tasks led to more processing, increasing CPU usage, and triggering our workers’ autoscaling. It seemed to work pretty well, except for certain edge cases.
