# Symposium of Formal Methods - Formal Verification of IoT Software with Frama-C

October 7-11, 2019

Porto, Portugal

The tutorial will take place on 10th of October in the morning.

[Registration](https://bit.ly/2JfdBjO)

The Virtual Machine is available [here](https://drive.google.com/uc?id=1AdTOQu849PKlXGLbiMR0qsT9L8qHgp0S&export=download).

The slides are available [here](https://allan-blanchard.fr/slides/fm-19-tuto.pdf)

# Presenters

- [Allan Blanchard](https://allan-blanchard.fr)
- [Nikolai Kosmatov](https://nikolai-kosmatov.eu/)
- [Frédéric Loulergue](https://frederic.loulergue.eu/)

# Contents

## The Topic

Among distributed systems, connected devices and services, also
referred to as the Internet of Things (IoT), have proliferated very
quickly in the past years. There are now billions of interconnected
devices, and this number is growing. It is anticipated that by 2021,
about 46 billions of devices will be in use. 

Some of these devices are in service in safety and security critical domains, and
even in domains that are not necessarily critical, privacy issues may
arise with devices collecting and transmitting a lot of personal
information. Moreover insufficiently secured devices may be used for
example for massive distributed denial of service attacks.  This
raises important security challenges. Formal methods have been used
successfully for years in highly critical domains, now they can help
to bring security into the IoT field.

While the correctness of an implementation with respect to a formal
functional specification provides the strongest form of guarantee, it
can be very costly to achieve. In practice it is therefore more common
to rely on a combination of formal methods to achieve an appropriate
degree of guarantee: static analyses to guarantee the absence of
runtime errors, deductive verification of functional correctness,
dynamic verification for parts that cannot be proved using deductive
verification.

[Frama-C](https://frama-c.com) is a source code analysis
platform that aims at conducting verification of industrial-size
programs written in ISO C99 source code. Frama-C fully supports the
combination of formal methods approach, by providing to its users with
a collection of plug-ins that perform static and dynamic analysis for
safety and security critical software. Moreover collaborative
verification across cooperating plug-ins is enabled by their
integration on top of a shared kernel, and their compliance to a
common specification language: ACSL.

Recently Frama-C has been applied
\[[1](https://doi.org/10.1007/978-3-319-54876-0_9),
[2](https://dl.acm.org/citation.cfm?id=3234910),
[3](https://doi.org/10.1007/978-3-319-77935-5_3),
[4](https://doi.org/10.1007/978-3-319-92994-1_11),
[5](https://doi.org/10.1145/3297280.3297495),
[6](https://doi.org/10.1007/978-3-030-20652-9_6)\]
to the verification of software in
the context of the Internet of Things, more specifically the
verification of modules of [Contiki](https://github.com/contiki-ng/contiki-ng), an open source
operating system for the IoT. 

## Expected Audience and Learning Outcomes

This tutorial will be of interest for both researchers and practitioners interested in 
software verification in general, and in particular in IoT software, as well as for
students in Software Engineering.  The tutorial only assumes knowledge of the C
programming language.

Participants will learn how to use the different formal analysis techniques and
how to combine them. Several examples and use cases presented during the tutorial will
give them a clear practical vision of possible usages of the underlying static and
dynamic analyses in their everyday work. The presented code fragments are part of
[Contiki](https://github.com/contiki-ng/contiki-ng), a real-world lightweight operating
system for the IoT.

## Material

A (VirtualBox) Virtual Machine containing Frama-C and the examples is available
through [this link](https://drive.google.com/uc?id=1AdTOQu849PKlXGLbiMR0qsT9L8qHgp0S&export=download).

## Summary of the Tutorial Format

The proposed tutorial duration is 180 minutes: about 20 minutes for the
introduction including an overview of Frama-C and Contiki, 50 minutes
for each of the 3 main parts, and 10 minutes for conclusion.

Each part consists of a presentation using slides and live
demonstration, and a session of exercises.  To work on the exercises,
the attendees will be provided a virtual machine image containing all
the tools ready to use.

In more detail, the tutorial will be structured as follows:

1. Introduction
    1. IoT and verification challenges
    2. An overview of Frama-C
    3. The Contiki operating system
2. Verification of absence of runtime errors using the abstract interpretation based plug-in EVA
    1. Presentation of EVA
    2. An application to Contiki
    3. Exercises
    4. Limitations and how to deal with them
3. Deductive verification using the plug-in WP
    1. Presentation of WP
    2. An application to Contiki
    3. Exercises
    4. Limitations and how to deal with them
4. Runtime verification with the plug-in E-ACSL
    1. Presentation of E-ACSL
    2. An application to Contiki
    3. Exercises
5. Conclusion and Further References

# Bibliography

- An overview of Frama-C: [KKP2015:FAC](https://doi.org/10.1007/s00165-014-0326-7)
- [Introduction to deductive verification with Frama-C](https://allan-blanchard.fr/publis/frama-c-wp-tutorial-en.pdf)
- Application of Frama-C to Contiki:
     - \[1\] [MDK2016:CRiSIS](https://doi.org/10.1007/978-3-319-54876-0_9) 
       \[[Authors PDF](https://nikolai-kosmatov.eu/publications/mangano_dk_crisis_2016.pdf)\]
     - \[2\] [PKDR2018:RED-IoT](https://dl.acm.org/citation.cfm?id=3234910)
       \[[Authors PDF](https://nikolai-kosmatov.eu/publications/peyrard_kdr_rediot_2018.pdf)\]
     - \[3\] [BKL2018:NFM](https://doi.org/10.1007/978-3-319-77935-5_3)
       \[[Authors PDF](https://allan-blanchard.fr/publis/bkl_nfm_2018.pdf)\]
     - \[4\] [LBK2018:TAP](https://doi.org/10.1007/978-3-319-92994-1_11)
       \[[Authors PDF](https://hal.inria.fr/hal-01811922/document)\]
     - \[5\] [BKL2019:SAC](https://doi.org/10.1145/3297280.3297495)
       \[[Authors PDF](https://allan-blanchard.fr/publis/bkl_sac_2019.pdf)\]
     - \[6\] [BLK2019:NFM](https://doi.org/10.1007/978-3-030-20652-9_6)
       \[[Authors PDF](https://allan-blanchard.fr/publis/blk_nfm_2019.pdf)\]
- Previous Frama-C tutorial papers:
     - [KPS2013:TAP](https://doi.org/10.1007/978-3-642-38916-0_10)
       \[[Authors PDF](https://nikolai-kosmatov.eu/publications/kosmatov_ps_tap_2013.pdf)\]
     - [KS2013:RV](https://doi.org/10.1007/978-3-642-40787-1_29)
       \[[Authors PDF](https://nikolai-kosmatov.eu/publications/kosmatov_s_rv_2013.pdf)\]
     - [KS2014:TAP](https://doi.org/10.1007/978-3-319-09099-3_13)
       \[[Authors PDF](https://nikolai-kosmatov.eu/publications/kosmatov_s_tap_2014.pdf)\]
     - [KS2016:RV](https://doi.org/10.1007/978-3-319-46982-9_7)
       \[[Authors PDF](https://nikolai-kosmatov.eu/publications/kosmatov_s_rv_2016.pdf)\]

# History of this tutorial

A similar tutorial was presented at

- the Zooming Innovation in Consumer Electronics International Conference ([ZINC 2018](http://www.gozinc.org/#information)), May 30-31, 2018, Novi Sad, Serbia,
- the 16th International Conference on High Performance Computing & Simulation ([HPCS 2018](http://hpcs2018.cisedu.info/)), July 16, 2018, Orléans, France.
- the third IEEE Secure Development Conference ([IEEE SecDev 2018](https://secdev.ieee.org/2018/home)), September 30, 2018, Boston, USA.
- the 29th IEEE International Symposium on Software Reliability Engineering ([IEEE ISSRE 2018](http://2018.issre.net/)), October 16, 2018,  Memphis, Tennessee, USA
- the The 34th ACM/SIGAPP Symposium On Applied Computing ([ACM SIGAPP/SAC 2019](https://www.sigapp.org/sac/sac2019/)), April 8-12, 2019, Limassol, Cyprus
