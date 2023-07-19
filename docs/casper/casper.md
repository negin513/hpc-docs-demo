# Casper cluster

*Created by BJ Smith, last modified on 2023-02-27*

The Casper cluster is a system of specialized data analysis and visualization resources; large-memory, multi-GPU nodes; and high-throughput computing nodes.

Casper is composed of 100 nodes featuring Intel Skylake or Cascade Lake processors.

- 22 Supermicro SuperWorkstation nodes are used for data analysis and visualization jobs. Each node has 36 cores and up to 384 GB memory.
    - 9 of these nodes also feature an NVIDIA Quadro GP100 GPU.
    - 3 nodes feature a single NVIDIA Ampere A100 GPU.
- 10 nodes feature large-memory, dense GPU configurations to support explorations in machine learning (ML) and deep learning (DL) and general-purpose GPU (GPGPU) computing in atmospheric and related sciences.
    - 4 of these nodes feature 4 NVIDIA Tesla V100 GPUs.
    - 6 of these nodes feature 8 NVIDIA Tesla V100 GPUs.
- 64 high-throughput computing (HTC) nodes for small computing tasks using 1 or 2 CPUs.
    - 62 HTC nodes have 384 GB of available memory.
    - 2 HTC nodes have 1.5 TB of available memory.
- 4 nodes are reserved for Research Data Archive workflows.

Please refer to the hardware summary table below for detailed specifications.

**Operating system: CentOS 7.8**

## Logging in on an NCAR system

To log in, start your terminal or Secure Shell client and run an ssh command as shown here:
```
ssh -X username@system_name.ucar.edu

```
Or
```
ssh -X username@system_name.ucar.edu

```

Some users (particularly on Macs) need to use -Y instead of -X when calling SSH to enable X11 forwarding.

You can use this shorter command if your username for the system is the same as your username on your local computer:
```
ssh -X system_name.ucar.edu 
```
OR 
```
ssh -X system_name.ucar.edu
```

After running the `ssh` command, you will be asked to authenticate to finish logging in.
