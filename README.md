<h1 align="center">Non-Official Machinekit-HAL</h1>

<h3 align="center">Goal with this fork is to make it compiling on any distro.</h3>

<div align="center"><img alt="Machinekit demo" src="media/machinekit-hal.svg" width="450px" /></div>

<h4 align="center">Universal <i>framework</i> for machine control.</h4>

<p align="center">
<a href="https://machinekit.io/">Website</a>
|
<a href="https://machinekit.io/docs">Docs</a>
|
<a href="http://www.machinekit.io/about">About</a>
</p>

**Machinekit-HAL** is a powerful software for _real-time_ control of machinery based on _**H**ardware **A**bstraction **L**ayer_ principle. With tools and libraries making development of new _components_ and _drivers_ easy. Integrators can choose to control **industrial robotic arm**, **single purpose machine** or **CNC mill** or **lathe** with additional software package.

Supporting _RT PREEMPT_ and _Xenomai 2_ real-time Linux kernel patches. **APT** packages available for Debian 9 _Stretch_, Debian 10 _Buster_, Ubuntu 18.04 _Bionic_ LTS and Ubuntu 20.04 _Focal_ LTS.

<div align="center"><img alt="Machinekit demo" src="https://raw.githubusercontent.com/cerna/machinekit-hal/various-bugfixes/media/machinekit_hal_ethercat_demo.gif" width="650px" /></div>

## Getting started

You can build locally on your machine in _**R**un-**I**n-**P**lace_ mode. The briefest sequence of commands would be from cloned folder.:

```sh
bootstrap.sh
mk-build-deps -irs sudo
cd src
./autogen.sh
./configure
make
sudo make setuid
```

More information about building can be glanced from [documentation](http://www.machinekit.io/docs/developing/machinekit-developing).

|![Warning](https://img.icons8.com/ios-filled/50/000000/warning-shield.png)| Be advised that currently there is no support for Linux distributions other than Debian derivatives. |
|:---:|---|

## History

**Machinekit-HAL** was created by separating the core functionality from now deprecated [Machinekit](https://github.com/machinekit/machinekit) repository into own repository.

It all started in the early nineties when NIST created the Enhanced Machine Controller Architecture in Public Domain as a _vendor-neutral_ software implementation for numerical control of machining operations. From that in 2003 open community of developers created a project called **EMC2** or _Enhanced Machine Controller 2_. (Or on the side of commercial software, EMC was developed into popular software _Mach3_ for Microsoft Windows.) _EMC2_ was renamed in 2011 as a **LinuxCNC**. In 2014, [**Machinekit**](https://machinekit.io) was forked from [LinuxCNC](https://linuxcnc.org) to facilitate deeper changes in _low level_ functionality. In 2020, the original _Machinekit_ repository was _archived_ and development is fully continuing in the **Machinekit-HAL** repository.

|![Warning](https://img.icons8.com/ios-filled/50/000000/warning-shield.png)| The _CNC_ part of original repository was separated into the [_Machinekit-CNC_](https://github.com/machinekit/machinekit-cnc) repository in the same move. |
|:---:|---|

## Getting involved

**Machinekit-HAL** like all projects in the **Machinekit** organization is volunteer based governed by the [**C**ollective **C**ode **C**onstruction **C**ontract ](http://www.machinekit.io/community/c4), generally known as a C4 originally from the [ZeroMQ](https://rfc.zeromq.org/spec/22) project.

The original source code is hosted publicly on [GitHUB](https://github.com/machinekit/machinekit-hal), where majority of programming discussion about further development happens. In lower measures, Machinekit-HAL is also discussed on [_Machinekit forum_](https://groups.google.com/forum/#!forum/machinekit) and in [_Machinekit Matrix Room_](https://matrix.to/#/#machinekit:matrix.org), which are used more to the point of support platforms and for general chat.

|![Counselling](https://img.icons8.com/ios-filled/50/000000/counselor.png)| It's always encouraged to create a new _issue_ in GitHub tracker first. Discuss the proposed changes there and then based on the output implement the changes and create a new _pull request_. |
|:---:|---|

## Licence

This software is released under the **GPLv2**, with some parts under the **LGPL**. See the file COPYING for more details.

|![Warning](https://img.icons8.com/ios-filled/50/000000/warning-shield.png)| For more detailed information consult specific files with source code implementing given functionality. There should be explicit licensing. |
|:---:|---|
