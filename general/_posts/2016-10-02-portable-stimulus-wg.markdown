---
layout: post
title:  "Valtrix Blog"
blogtitle: "Support for Accellera's Portable Stimulus Specification in STING"
date:   2016-10-02 09:45:00
author: Shubhodeep Roy Choudhury
---

I went to the 2016 edition of [DVCON India][dvcon_ind_link] last month. Since Valtrix is also working in the area of reusable and portable stimulus, I attended the Accellera update on PSWG. You can read more about Accellera's Portable Stimulus Working Group [here][pswg_link] in case you are not aware of the ongoing effort. Speakers from Mentor Graphics,<!--more--> Cadence, Breker, Synopsys and Vayavya presented the latest status on the progress made with the specification. 

Portable stimulus specification certainly is a very valuable proposition aimed at removing a broad range of redundancies from design verification. The specification will provide mechanisms for verification engineers to target any scenario to be tested. Once the intent is expressed with the syntax supported by the portable stimulus specification, it can be converted into test stimulus using tools (or the secret sauce as the Accellera foil mentions below :wink: ) provided by the EDA vendors. 

The test stimulus generated would seamlessly run across all the verification environments. As a result, once the test intent is captured, it can be reused throughout the life cycle of design and across multiple projects.

![PswgVision](/assets/img/Pswg-Vision.png)

The foil has been taken from the slides on PSWG update presented in DVCON US 2016 posted [here][pswg_dvcon_us_update] at Accellera's website.

In STING, we support a very elaborate input specification scheme to support different paradigms of functional verification for SoC/IP implementations. Once the portable stimulus model is available, we will evaluate how the syntax and semantics can be mapped to our specification scheme and release our version of "secret sauce". We will also be exploring how our proprietary test applications can be expressed in form of portable stimulus IP for better compatibility.

To conclude the blog, Valtrix is fully committed to the PSWG vision and looking forward to the first release of the specification!

[dvcon_ind_link]: https://dvcon-india.org/
[pswg_link]: http://accellera.org/activities/working-groups/portable-stimulus/
[pswg_dvcon_us_update]: http://www.accellera.org/images/activities/working-groups/portable-stimulus/PortableStimulusUpdateDVConUS_2016.pdf
[sting_link]: http://valtrix.in/sting/
