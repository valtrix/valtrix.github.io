---
layout: post
title:  "Valtrix Blog"
blogtitle: "Valtrix at the 8th RISC-V Workshop Barcelona May 2018"
date:   2018-04-17 12:00:00
author: Shubhodeep Roy Choudhury
---

[Valtrix][valtrix_link] will participate in the [8th RISC-V workshop][rv_ws_link] at Barcelona, Spain in May 2018. Co-hosted by the Barcelona Supercomputing Center (BSC) and Universitat Politècnica de Catalunya (UPC) and sponsored by NXP and Western Digital, this event will<!--more--> bring together the [RISC-V][riscv_link] community to share RISC-V activities underway around the globe, and build consensus on the future evolution of the instruction set.

Two poster presentations on design verification of RISC-V implementations using [STING][sting_link] will be featured in the RISC-V workshop. The complete agenda of the workshop can be found [here][rv_ws_agenda_link].

The high level details of the two Valtrix poster presentations are given below -

**Title: Verifying PULPino RISCY Core for a Google Accelerator with STING**

*Authors: Shubhodeep Roy Choudhury and Shajid Thiruvathodi from Valtrix Technologies Pvt. Ltd. and Vaidyanathan Seetharaman, Matt Cockrell, Jon Michelson and Jason Redgrave from Google Inc.*

>Google uses the PULPino RISC-V core RISCY as a job scheduling and dispatch mechanism for a hardware accelerator (similar to a GPU controller). This requires full compliance with the RISC- V RV32I base integer instruction set, standard extensions for integer multiplication and division (‘M’) and compressed instructions (‘C’), and capability to handle interrupts from multiple sources. We used STING, a software-driven verification solution for RISC-V based CPU/SoC implementations, to verify the architectural compliance and functionality of the RISCY core. This verification effort helped uncover 30 RTL, documentation, and toolchain issues in the relatively mature RISCY implementation.

**Title: STING - A Complete RISC-V Functional Verification Solution**

*Authors: Shubhodeep Roy Choudhury and Shajid Thiruvathodi from Valtrix Technologies Pvt. Ltd.*

>The concept of open-source instruction set architecture introduced by RISC-V allows large scale customizations in CPU and SoC designs. With this flexibility comes an even larger challenge and dependency on verifying architectural compliance and functional correctness. Since SoC designs nowadays have to compete in a world of significantly increased complexity, multi-million dollar development and manufacturing costs, tight time-to-market constraints, and aggressive competition, the cost and business impact of non production-worthy silicon is extremely high and can be very damaging, even to established major SoC companies. Functional issues at the system level can result into silicon re-spins affecting profitability and time-to-market. In order to counter that, engineering teams need to adopt techniques and tools for verification that scale across the complexity and life-cycle of design. We will here describe STING, a state-of-the-art verification tool for RISC-V based implementations. It embodies a software driven test generation methodology which allows portability of intelligent, self-checking, and architecturally correct test stimulus throughout the life cycle of a design, enabling SoC and IP vendors to achieve their design verification goals quickly and efficiently across pre-silicon, emulation, FPGA and post-silicon phases of development.

Please email [contact@valtrix.in](mailto:contact@valtrix.in) to set up a meeting at the RISC-V Workshop Barcelona, or to learn more about the verification offerings from Valtrix for RISC-V implementations.

[valtrix_link]: http://valtrix.in
[rv_ws_link]: https://tmt.knect365.com/risc-v-workshop-barcelona/
[riscv_link]: http://riscv.org
[sting_link]: http://valtrix.in/sting/
[rv_ws_agenda_link]: https://tmt.knect365.com/risc-v-workshop-barcelona/agenda/2
