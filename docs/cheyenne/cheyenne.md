# Cheyenne supercomputer

Cheyenne is a 5.34-petaflops, high-performance computer built for NCAR by SGI. The system was released for production work on January 12, 2017.

![cheyenne](https://kb.ucar.edu/download/attachments/embedded-page/RC/Cheyenne%20supercomputer/Cheyenne-450.jpg?api=v2)

An SGI ICE XA Cluster, the Cheyenne supercomputer features 145,152 Intel Xeon processor cores in 4,032 dual-socket nodes (36 cores/node) and 313 TB of total memory.

Cheyenne's login nodes give users access to the GLADE shared-disk resource and other storage systems.

Data storage components provided by DataDirect Networks (DDN) give the GLADE system a total usable capacity of 38 PB. The DDN system transfers data at the rate of 200 GBps, more than twice as fast as the previous file system’s rate of 90 GBps.


!!! tip
    "Go to "Quick start on Cheyenne". 

## Logging in
To log in, start your terminal or Secure Shell client and run an `ssh` command as shown here:
```
ssh -X username@system_name.ucar.edu
```
OR 
```
ssh -X username@system_name.ucar.edu
```

Some users (particularly on Macs) need to use `-Y` instead of `-X` when calling `ssh` to enable `X11 forwarding`.

You can use this shorter command if your username for the system is the same as your username on your local computer:
```
ssh -X system_name.ucar.edu 
```
OR 
```
ssh -X system_name.ucar.edu
```
After running the ssh command, you will be asked to authenticate to finish logging in.


## Estimating core-hours needed
Cheyenne allocations are made in core-hours. The recommended method for estimating your resource needs for an allocation request is to perform benchmark runs. Some guidance is provided here.

The core-hours used for a job are calculated by multiplying the number of processor cores used by the wall-clock duration in hours. Cheyenne core-hour calculations should assume that all jobs will run in the regular queue and that they are charged for use of all 36 cores on each node.


```
