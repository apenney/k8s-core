# Demo

This repository contains the ability to manage core components of both AWS and
GCP clusters, appropriately overlaying the right configuration in the right
context.

## Usage

Just point flux at an appropriate branch to match your cluster version:

## ConfigMap

We rely on having the following configmap:

```
apiVersion: v1
kind: ConfigMap
metadata:
  name: release
  namespace: kube-system
data:
  cluster_name: "ashley"
```

This must exist!

## Branches

* 1.18
