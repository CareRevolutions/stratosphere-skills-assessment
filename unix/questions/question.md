1. You have a “protected” subnet (perhaps in AWS) which has no route to the internet. You also have a public (NATted) subnet. You’d like to update the OS on a machine running your favorite flavor of Linux in the protected subnet. You have another machine with two network cards, each attached to one of the subnets. Show all commands (ensure kernel is capable) involved in setting up and using for example a ‘proxy’ on the second machine (or some other mechanism of your choice) that will allow the first machine to update its packages. The device on the 1st machine is eth0 10.10.0.3 netmask 255.255.252.0, and 2nd machine are eth0 10.10.0.4 netmask 255.255.252.0 and eth1 10.10.4.5 netmask 255.255.252.0 default gateway 10.10.4.1. BONUS How would you do this more simply in AWS if both subnets were in the same AZ (as above provide shell (including AWSCLI) commands)?
2. Provide a configuration (shell script -- use here docs and/or sed for config files) that affords you the following for a filesystem on an AWS instance
   requirements:

    1. Initial size of 500GB, with ability to add more storage (but not necessarily unlimited) and grow filesystem while it’s mounted
    2. Read bandwidth in excess of 1.5 Gigabyte/second
    3. Durable in the sense that it will survive at least termination of the instance or failure of one device
    4. Cost of the storage is less than $.16/GB/month