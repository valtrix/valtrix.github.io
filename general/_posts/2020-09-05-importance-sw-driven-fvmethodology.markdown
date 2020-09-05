---
layout: post
title:  "Valtrix Blog"
blogtitle: "Importance of Software Driven Functional Verification Methodology"
date:   2020-09-05 10:00:00
description: "Importance of Software Driven Functional Verification Methodology"
author: Shubhodeep Roy Choudhury
---

A good functional verification methodology is extremely crucial to the success of any semiconductor design project. Missed or late bugs can massively hurt market share, revenue and brand name even for reputed companies. The complexity of SoC designs along with tight time-to-market constraints demand high levels of efficiency in the verification process.<!--more-->

The approach to verify the functionality and correctness of implementation changes as the design matures. The testing in the initial phase of design is carried out using system verilog/UVM based block or top level tests in design simulations and emulation. The utility of these tests reduce in the later stages of FPGA and silicon, where the focus is on enabling OS and real world applications to verify the use cases which the design supports. These software applications are cumbersome to enable in simulation rendering them ineffective when used as a stimulus for design verification. The logic issues hit by the software applications are very difficult to reproduce and debug in simulations. This results in a disconnect in verification methodology used across the design life cycle.

<br/>
![STING_Portable_Stimulus](/assets/img/STING_Portable_Stimulus.png)
*Figure 1: Advantages of a software-driven functional verification methodology (Image: Valtrix)*
<br/>

With [STING][sting_link], we have developed an approach which utilizes software driven stimulus to address these issues to a large extent. The stimulus has a very low memory and instruction footprint so that they can be effectively used in slow verification environments like simulations and emulation. In case of faster targets like FPGA and silicon, the tool can be programmed to generate the stimulus on-target and run for a longer span of time.

Test stimulus once developed can be reused across the design life cycle and allows consistent execution across multiple verification environments. As a result companies can save on duplicate efforts spent by design verification and system validation teams in maintaining the test stimulus. This approach also enables easy migration of the failures hit on silicon to simulations for faster debug. Early enabling of real-world use-cases also increases the chances of hitting the complex bugs earlier in the project.

[sting_link]: https://valtrix.in/sting/
