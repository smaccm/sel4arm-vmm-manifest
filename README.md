sel4arm-vmm-manifest
====================

Top level repo for ARM based seL4 VMM.

To build and then run Linux in a virtual machine on seL4 on the ARM-based Odroid-XU, do the following:

## Prerequisites

Please make sure you have the seL4 prerequisites as described in http://sel4.systems/Download.

## Checkout
    mkdir sel4arm-vmm
    cd sel4arm-vmm
    repo init -u ssh://github.com/smaccm/sel4arm-vmm-manifest.git
    repo sync

## Compile
    make odroidxu_vm_linux_defconfig
    make

## Run

See instructions in [HARDWARE.md](https://github.com/smaccm/camkes-smaccm-manifest/blob/master/HARDWARE.md) to run on an Odroid-XU

Once the system boots into Linux, you can log in using either:

    user: odroid
    password: odroid

Or

    user: root
    password: root


