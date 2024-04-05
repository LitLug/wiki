# Linux 发行版

**Linux 发行版**（英语：Linux distribution 或 distro，也被叫做 **GNU/Linux 发行版**），为一般用户预先集成好的 Linux 操作系统及各种应用软件。一般用户不需要重新编译，在直接安装之后，只需要小幅度更改设置就可以使用，通常以软件包管理系统来进行应用软件的管理。Linux 发行版通常包含了包括桌面环境、办公包、媒体播放器、数据库等应用软件。这些操作系统通常由 Linux 内核、以及来自 GNU 计划的大量的函式库，和基于 X Window 或者 Wayland 的图形界面。有些发行版考虑到容量大小而没有预装 X Window，而使用更加轻量级的软件，如：BusyBox、musl 或 uClibc-ng。现在有超过 300 个 Linux 发行版（Linux 发行版列表）。大部分都正处于活跃的开发中，不断地改进。

由于大多数软件包是自由软件和开源软件，所以 Linux 发行版的形式多种多样——从功能齐全的桌面系统以及服务器系统到小型系统（通常在嵌入式设备，或者启动软盘）。除了一些定制软件（如安装和配置工具），发行版通常只是将特定的应用软件安装在一堆函式库和内核上，以满足特定用户的需求。

这些发行版可以分为商业发行版，比如 **Ubuntu**（Canonical 公司）、**Red Hat Enterprise Linux**、**SUSE Linux Enterpise**；和社区发行版，它们由自由软件社区提供支持，如 **Debian**、**Fedora**、**Arch**、**openSUSE** 和 **Gentoo**。

### 发行版们 {#distros}

一个典型的 Linux 发行版除了 Linux 内核以外，通常还会包括一系列 GNU 工具和库、一些附带的软件、说明文档、一个桌面系统、一个窗口管理器和一个桌面环境。不同的发行版之间除了 Linux 内核以外的其它部分都有可能不一样，因此有的时候我们对比某两种发行版的时候会觉得它们看起来像是完全不一样的操作系统，然而实质上它们却拥有着相同的核心，即 Linux 内核。

这里给读者介绍若干桌面和服务器环境中主流的发行版分支：

#### Debian 分支 {#debian-branch}

Debian 是一个完全由自由软件构成的类 UNIX 操作系统，第一个版本发布于 1993 年 9 月 15 日，迄今仍在维护，是最早的发行版之一。其以坚持自由软件精神和生态环境优良而出名，拥有庞大的用户群体，甚至自己也成为了一个主流的子框架，称为“Debian GNU/Linux”。

![](images/Debian-Logo.png)

Debian 图标
{: .caption }

Debian GNU/Linux 也派生了很多发行版，其中最为著名的便是 Ubuntu（官方译名“友邦拓”）。Ubuntu 由英国的 Canonical 公司主导创立，是一个主打桌面应用的操作系统。其为一般用户提供了一个时新且稳定的由自由软件构成的操作系统，且拥有庞大的社群力量和资源，十分适合普通用户使用。

![](images/Ubuntu-Logo.png)

Ubuntu 图标
{: .caption }

#### Red Hat 分支 {#red-hat-branch}

Red Hat Linux 是美国的 Red Hat 公司发行的一个发行版，第一个版本发布于 1994 年 11 月 3 日，也是一个历史悠久的发行版。它曾经也广为使用，但在 2003 年 Red Hat 公司停止了对它的维护，转而将精力都投身于其企业版 Red Hat Enterprise Linux（简称 RHEL）上，Red Hat Linux 自此完结，而商业市场导向的 RHEL 维护至今。

![](images/Red-Hat-Logo.png)

Red Hat 公司商标，RHEL 是其旗下产品
{: .caption }

在 Red Hat Linux 在停止官方更新后，由社群启动的 Fedora 项目接管了其源代码并构筑了自己的更新，演变成了如今的 Fedora 发行版。Fedora 是一套功能完备且更新迅速的系统，且本身计划也受到了 Red Hat 公司的赞助，成为了公司测试新技术的平台。

![](images/Fedora-Logo.png)

Fedora 图标
{: .caption }

虽然 RHEL 是一个收费的、商业化的系统，但是其遵循 GNU 通用公共许可证，因此会开放源代码。编译这些源代码可以重新得到一个可以使用的操作系统，即一个新的发行版：CentOS（Community Enterprise Operating System，社区版企业操作系统）。因为 CentOS 几乎完全编译自 RHEL 的代码，所以其也像 RHEL 一样具有企业级别的稳定性，适合在要求高度稳定的服务器上运行。

2020 年 12 月，CentOS 社区在其博客中[宣布未来的重点转向 CentOS Stream](https://www.redhat.com/en/blog/centos-stream-building-innovative-future-enterprise-linux)，这是一个全新的滚动发行版。在此之前，RHEL 的上游为 Fedora，而 CentOS 的上游为 RHEL；在推出 CentOS Stream 之后，它就成为了 RHEL 的上游发行版。与此同时，CentOS 8 的支持期限被缩短至 2021 年底，且不再推出新的非 Stream 的 CentOS 版本。不满于该决定的人们也组织了新的社区，推出了诸如 [AlmaLinux](https://almalinux.org/)、[Rocky Linux](https://rockylinux.org/) 等发行版。

![](images/CentOS-Logo.png)

CentOS 图标
{: .caption }

#### Arch Linux 分支 {#arch-linux-branch}

Arch Linux 是一个基于 x86-64 架构的 Linux 发行版，不过因为其内核默认就包含了部分非自由的模块，所以其未受到 GNU 计划的官方支持。即便如此，Arch Linux 也因其“简单、现代、实在、人本、万能”的宗旨赢得了 Linux 中坚用户的广泛青睐。不过，Arch Linux 对这个宗旨的定义和其它发行版有所区别。通常的操作系统为了方便用户快速上手，都是尽可能隐藏底层细节，从而避免用户了解操作系统的运行知识即可直接使用。但是 Arch Linux 则是重在构建优雅、极简的代码结构，这方便了使用者去理解系统，但不可避免地要求使用者自身愿意去了解操作系统的运作方式。某种程度上说，它的“简单”和“人本”注重的是方便用户通过了解而去最大化地利用它，而不是采取屏蔽工作原理的方式来降低使用门槛。因此，本书不建议初学者直接上手 Arch Linux，但十分推荐在读者对 Linux 有进一步了解之后去探索它。

![](images/Arch-Linux-Logo.png)

Arch Linux 图标
{: .caption }

Arch Linux 拥有强大的功能，但因其特殊的理念使得用户不易使用。为了能让一般用户也能用上 Arch Linux 的强大功能，它的变种 Manjaro 发行版于 2011 年问世。Manjaro 发行版基于 Arch Linux，但更注重易用，因而更适合一般用户。

![](images/Manjaro-Logo.png)

Manjaro 图标
{: .caption }

以上是若干个常见的 Linux 发行版系列，其他的常用发行版有 openSUSE、Gentoo 等。

Linux 的发行版非常丰富，不同的发行版有其各自的特性，因而可以面向不同的用户满足独特的需求。对于新手来说，一个拥有丰富的图形界面的发行版更加适合初步探索和后续使用。
