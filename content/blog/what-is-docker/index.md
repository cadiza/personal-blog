---
title: What is Docker?
date: "2021-07-26T19:00:42.268Z"
description: develop, send and execute applications everywhere
---

With the slogan "Build, Ship and Run Any App, Anywhere", the open source container platform **Docker** defines its main function: to develop, ship and run any application on any system, making it a flexible and resource-saving alternative to virtual machine (VM)-based emulation of hardware components.

While _traditional hardware virtualisation_ is based on starting different guest operating systems on the same host computer, with **Docker apps** are run as isolated processes within a single system by means of so-called containers. This is called container-based virtualisation and therefore also virtualisation at the operating system level.

Although both technologies allow system administrators and developers to install different applications with different requirements in parallel on the same physical system, their most notable differences are based on resource utilisation and portability.

## Containers

In order to encapsulate applications with classic virtualisation hardware, an element known as a _Hypervisor_ is required, which functions as an abstraction layer between the host system and the virtual guest systems. Each guest system emulates a complete machine with a separate operating system kernel, to which the hypervisor allocates the host hardware components:

> - CPU
> - Memory
> - HDD space
> - Available hardware peripherals

in a proportional manner.

In comparison, in container-based virtualisation, a comprehensive guest system is not built, but applications are started in containers which, while sharing the same kernel, i.e. that of the host system, run as isolated processes in user space.

The key feature of container-based virtualisation is that applications with different requirements can run in isolation from each other while avoiding the overhead of a separate host system. For this purpose, container technology takes advantage of two basic functions of the Linux kernel: control groups (Cgroups) and Kernel namespaces.

## Portable and highly scalable

**Docker** also allows cross-platform applications to be installed on different infrastructures without the need to adapt them to the specific configuration of the hardware and software systems of each host system.
