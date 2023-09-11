---
title: Config Reference
description: ''
position: 32
category: 'Kyverno Plugin'
---

# Config Reference

Configuration file reference with all possible options.

```yaml
kubeconfig: '~/.kube/config' 

api:
  port: 8080
  # HTTP Basic Authentication for APIs and metrics endpoints
  basicAuth:
    username: ""
    password: ""
    secretRef: ""

rest:
  enabled: false

metrics:
  enabled: false

blockReports:
  enabled: false
  eventNamespace: default
  results: 
    maxPerReport: 200
    keepOnlyLatest: false
  source: "Kyverno Event"

leaderElection:
  enabled: false
  releaseOnCancel: true
  leaseDuration: 15
  renewDeadline: 10
  retryPeriod: 2
```
