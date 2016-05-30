---
layout: post
title:  "Valtrix Blog"
blogtitle: "Announcing Support for RISC-V in STING"
date:   2016-05-30 10:30:00
author: Shajid T
---

<b>Valtrix Systems</b> is happy to announce the availability of [STING][sting_link] for [RISC-V][riscv_link] architecture. RISC-V is an open-source instruction set architecture (ISA) based on reduced instruction set computing (RISC) fundamentals. It has been designed to support extensive customization and specialization across multiple classes<!--more--> of processors. Please note that this is a *beta* version of STING and we are working on testing and hardening it further. In the sections below, you can find the list of features that are currently implemented in STING and the ones that are going to be supported soon.
<br/>
<br/>

#### Features

The following features are tested and supported in STING at present. These features have been tested on Spike simulator, QEMU model for RISC-V and Rocket core "C++" simulator. (NOTE: Not all the features have been tested on all the models)

 * Based on user level v2.0 and privilege level v1.7 specifications
 * Supports RV32I/RV64I base integer instruction set and RV32M/RV64M standard extensions
 * Supports machine, supervisor and user mode
 * Support for Sv48: 48 bit virtual-memory system
 * Support for following modes:
   * Machine only
   * Machine and user mode
   * Machine, supervisor and user modes
 * Support for non contiguous RAM
 * Uniprocessor mode is well-tested and supported. Testing of multi processor mode of execution in progress.
 * Support for HTIF based console
 * Support for generic UART
 * Support for STING's focused test development framework
 * Support for C++ based test algorithms/applications in STING
<br/>
<br/>

#### Upcoming Features

Support for the following features are going to be added very soon -

 * Support for standard extensions for atomic, single and double precision floating point instructions
 * Sv39 and Sv32 virtual-memory system
<br/>
<br/>

We are very excited about the RISC-V architecture and the potential it holds as an open-source ISA. If you need more information about STING or need a demo, please drop an email to contact@valtrix.in


[sting_link]: http://valtrix.in/sting/
[riscv_link]: http://riscv.org/
