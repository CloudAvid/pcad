# Introduction
**_pcad_**, part of PVM-Prototype, is wrapper of [pvmctl](https://github.com/cloudavid/pvmctl/) for cluster environment.

**_pcad_** is part of PVM-prototype, our early try to write special hypervisor based on KVM named **_PVM_**. 

Read [pvmctl wiki](https://github.com/cloudavid/pvmctl/wiki) for more information.

# Installation

You should first install **_pvmctl_**, then run **_install-pcad_** for pcad installation:
```shell
$ ./install-pcad
```

NOTE: **_pcad_** developed based on **_cman + rgmanager_**. So to use pcad, you should first install & configure cman.

# Documentation

Complete tutorial located at [pvmctl wiki](https://github.com/cloudavid/pvmctl/wiki).

See also **_pcad help_**:
```shell
pcad is a management and control script for KVM-based virtual machines in the cluster.

Usage:  pcad start    host [server]   - start the named VM on local machine or on the named server if given
        pcad stop     host            - stop  the named VM
        pcad restart  host [server]   - restart named "VM", it will be restarted on the named server if given

        pcad status                   - show the status of the cluster
        pcad status   host            - show full details for the named VM in the cluster

        pcad show-log #n              - show the cluster activity log (use CTRL+^C to exit)

        pcad uptime                   - show uptime server

        pcad mkimg    host image_name image_size  - create a disk image in the host directory
        pcad rmimg    host image_name             - remove disk image of the host
        pcad rnimg    host image_name new_name    - rename disk image of the host

        pcad new      host_name [sid]             - Create A virtual machine
        pcad create   template host_name [sid]    - Create A virtual machine from template
        pcad clone    host clone_name [new_sid]   - creating a clone from the host

        pcad rmvm     host                        - delete virtual machine
        pcad rename   host new_name               - rename host to new_name
        pcad mvvm     host new_sid                - move virtual machine to new storage

        pcad edit     host                        - Open config file for edit
        pcad info     host                        - print out host information (parameters in config file)

        pcad mktmpl   host  [template_name]       - Create A virtual Template from host
        pcad rmtmpl   template_name               - Remove the Virtual Template
        pcad mkiso    iso_name                    - Create An ISO image from the CD in Local CDROM(local)
        pcad rmiso    iso_name                    - Remove the ISO image

        pcad ls                                   - print out list of virtual machines
        pcad lst                                  - print out list of Virtual Templates
        pcad lscd                                 - print out list of CD Images (ISO files)
        pcad lsid                                 - print out list of Virtual Storages.

        pcad help                                 - show this usage

```

# Contributing Code
If you are capable of contributing code changes, we encourage you to do so. You can help us in different fields:
* Develop new features
* Improve Documentation
* ... 

# Bugs
 Please use github [issues](https://github.com/cloudavid/pcad/issues) to report bugs. 
# About
Copyright 2010-2020 [CloudAvid](http://www.cloudavid.com).
