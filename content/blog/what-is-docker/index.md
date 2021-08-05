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

**Docker** also allows cross-platform applications to be installed on different infrastructures without the need to adapt them to the specific configuration of the hardware and software systems of each host system. It uses _images_ as portable copies of the container software.

These contain the applications together with all libraries, binary and configuration files required during the execution of the encapsulated application processes. For this reason, they require hardly anything from the host system, which makes it easy to move a container-application between different operating systems without any adjustments.

## Images & Engine

As stated before, Docker is made up of two main components, [Docker images](https://docs.docker.com/engine/reference/commandline/image/) & [Docker engine](https://docs.docker.com/engine/).

### Images

Docker containers are based on images, which are read-only templates with all the instructions needed by the engine to create a container. As a portable copy of a container, a Docker image is described in the form of a text file (Dockerfile). A container can be considered as a running process of an image.

### Engine

The heart of any Docker development project is the Docker engine, i.e. an open source client-server application available to all users in the current version on all established platforms.

The components that make up the basic architecture of this engine are: a daemon with server functions, a programming interface (API) based on REST (Representational State Transfer) and the operating system terminal (Command-Line Interface, CLI) as the user interface (client).

Docker allows you to start, stop or manage software containers directly from the console. With the `docker` command and commands such as `build`, `pull` or `run`, it is possible to communicate with the daemon, allowing both client and server to be on the same system.
