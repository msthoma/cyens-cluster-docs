# Cluster docs

## Running jobs

### Starting jobs

```bash
sbatch run_script.sh
```

### Monitoring jobs

```bash
squeue
```

Can also use the following to monitor jobs in real-time:

```bash
watch squeue
```

### Job efficiency

After a job finishes, details such as CPU utilisation & efficiency, memory utilisation & efficiency, etc., can be queried with:

```bash
seff <SLURM_JOB_ID>
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

## Storage

### Disk quotas

Home directories (at `/trinity/home/<USER>`) have a disk quota of 20GB. Information about the current state of a user's home directory can be retrieved using:

```bash
quota -s
```
