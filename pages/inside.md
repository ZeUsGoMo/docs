# What's On The Device?

The [Resin.io][resin] software running on your device leverages a number of powerful components to provide great functionality at a minimal performance cost:-

## Operating System

![Yocto Project Logo](/img/yocto.png)

The operating system we install on your device is [Yocto][yocto] [Linux][linux]. This is an innovative distribution which comprises components which can be combined together to build a custom Linux system containing only the software you need for any target architecture.

This is perfect for Resin.io - we have built an optimised Linux system for the devices we support and can guarantee the same behaviour on any further devices we support in the future.

## Application Environment

![Docker Logo](/img/docker.png)

We use [Docker][docker] to leverage the power of [containerisation][containerisation] to provide a consistent environment for your software to operate inside at a far smaller performance penalty than virtualisation, as well as giving you the freedom to provide custom [Dockerfiles][Dockerfile] so you have total freedom in what runs on your device.

In addition we leverage containerisation to have our build server build your project without consuming a single CPU cycle on your actual device, then ship a container to it which is guaranteed to run as built without concern for the host operating system running on your device.

## Resin.io Supervisor

![Resin.io Logo](/img/logo_big.svg)

The Resin.io supervisor is a lightweight process which runs on your device, manages your applications and communicates with our servers - downloading new applications and updates to existing applications as you push them, sending logs to your dashboard, as well as updating itself automatically when new releases of the supervisor are pushed out by us.

[resin]:https://resin.io
[yocto]:https://www.yoctoproject.org/
[linux]:http://en.wikipedia.org/wiki/Linux
[docker]:https://www.docker.com/
[containerisation]:http://en.wikipedia.org/wiki/Operating_system%E2%80%93level_virtualization
[Dockerfile]:http://docs.docker.com/reference/builder/