---
layout: post
title:  "Valtrix Blog"
blogtitle: "Running STING on PULPino Platform"
date:   2017-12-18 12:30:15
author: Shubhodeep Roy Choudhury
---

[PULPino][pulp_link] is a competitive, state-of-the-art 32-bit processor based on the RISC-V architecture, with a rich set of peripherals, and full debug support developed at ETH Zurich and Università di Bologna. PULPino is based on optimized 32-bit RISC-V cores (known as RI5CY and Zero-riscy) with complete support for the RV32I base integer instruction<!--more--> set and extensions for compressed and integer multiplication/division instructions. The core also implements several other custom extensions such as - hardware loops, post incrementing load and store instructions, ALU and MAC operations. A very small subset of privileged specification and CSR (control and status registers) has been implemented to keep the footprint of the core as small as possible. More information on the implementation can be found in the PULPino [documentation][pulp_docs].
<br/>
<br/>

#### Enabling STING on PULPino

We recently enabled [STING][sting_link] on the open source test bench of PULPino available in the project's [github repository][pulp_git_link]. The code base has been [forked][valtrix_pulp_git_link] so that STING specific customizations can be added as required. The steps to setup the test bench and run STING binaries are documented in a README file which can be found [here][valtrix_pulp_git_readme] (snapshot below).

<br/>
![STINGPulpReadme](/assets/img/STING_Readme_PULP.png)

<br/>
Minor modifications to the test bench were made (e.g. relocating ROM, combining instruction and data memory into a single memory block) to get STING up and running on the platform. The size of the RAM was also increased to ensure that more number of tests could be packed in a single STING binary.

On the tool side, support for some of the custom extensions (hardware loops) and PULPino peripherals (timer, UART, event unit etc.) was added to support the design verification needs of the platform.
<br/>
<br/>

#### Running STING on PULPino Simulations

The steps to run the STING test can be found in the README file. A STING binary has been copied to the following path - sw/apps/sting/images in the forked repository. It can be used to run and evaluate a test comprising of random stimulus on the PULPino simulations.

<br/>
![STINGPulpModelsim](/assets/img/STING_ModelSim_PULP.png)


<br/>
Once the test is run, the waves and core trace are dumped in - sw/build/apps/sting. Snapshot of the core trace from the STING test is given below.

<br/>
![STINGPulpCoreTrace](/assets/img/STING_CoreTrace_PULP.png)

<br/>

#### Conclusion

STING has been successfully ported to the specifications of the PULPino platform and can be extended further to meet the verification needs of any SoC/IP design based on it.

We have plans to run STING extensively on PULPino and make sure that the design is compliant with the RISC-V specification. The test stimulus will be a random mix of instructions supported by the PULPino core, the bias for which can be controlled using configuration files. In addition to the random test content, a large number of focused and corner-case scenarios are also covered using snippets of directed code. The timer, UART and event unit devices are also programmed for concurrency and to allow generation of interrupts at regular intervals during the test execution. The results from test execution on PULPino simulations are compared with the results obtained from running the same test on SPIKE (the RISC-V CPU model) to ensure functionally correct behavior.

If this interests you, write to [contact@valtrix.in][mailto:contact@valtrix.in] to know how STING can help meet your RISC-V verification goals quickly and efficiently.
<br/>

<br/>

[sting_link]: https://valtrix.in/sting/
[riscv_link]: https://riscv.org
[pulp_link]: https://www.pulp-platform.org/
[pulp_docs]: https://www.pulp-platform.org/documentation/
[pulp_git_link]: https://github.com/pulp-platform/pulpino
[valtrix_pulp_git_link]: https://github.com/valtrix/pulpino/tree/pulpino_05f0dbe
[valtrix_pulp_git_readme]: https://github.com/valtrix/pulpino/blob/pulpino_05f0dbe/STING_README.md
