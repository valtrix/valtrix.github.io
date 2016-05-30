---
layout: post
title:  "STING for RISC-V"
blogtitle: "Announcing support for RISC-V based systems in STING"
date:   2016-05-30 10:30:00
author: Shajid T
---

<b>Valtrix Systems</b> is happy to announce the availability of STING for RISC-V
based systems. This is a *beta* version of STING and we are working on hardening
it.

<br/>

#### Features
---

 * Based on User Level spec 2.0
 * Priv spec 1.7
 * Supports all integer instructions and "M" instructions
 * Supports machine,supervisor and user mode
 * Support for Sv48: 48 bit Virtual-Memory system
 * Support for following modes:
   * Machine only
   * Machine and User mode
   * Machine, Supervisor and User modes
 * Support for non contiguous RAM
 * Supports once CPU, but will support multi processor shortly.
 * Support for htif based console
 * Support for generic UART


We have tested these features on spike, risc-v qemu and rocket core "C++"
simulator.(Note: Not all the features have been tested on all the models)

<br/>

#### Upcoming Features
---

We will be adding support for the following soon.

 * Single and Double precision floating point instructions
 * Sv39 and Sv32 Virtual-Memory system

We are very excited about the RISC-V architecture and the potential it holds as
an open architecture. 


If you need more information about STING or need a demo, please drop an email to
contact@valtrix.in


