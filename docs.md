---
id: 6jcokroc8otqv0gh3ufzoz6
title: Cluster
desc: ''
updated: 1668433769622
created: 1668433453255
---

## Monitoring jobs

```bash
squeue
```

Can also use the following to monitor jobs in real-time:

```bash
watch squeue
```

## Getting info about the cluster

The following shows detailed information about all nodes in the cluster:

```bash
scontrol show node
```

The following also show info about the nodes in a more condensed form:

```bash
sinfo --Node --long
sinfo -o "%n %e %m %a %c %C"
```
