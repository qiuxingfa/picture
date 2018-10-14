# Epiphany


---

>a multi-core processor made by Adapteva

## Adapteva
* Adapteva is a `fabless semiconductor company` focusing on low power many core microprocessor design
* founded in 2008
* Products are based on its `Epiphany` multi-core MIMD architecture and its Parallella Kickstarter project promoting "a supercomputer for everyone" in September 2012 The company name is a combination of `adapt` and the Hebrew word `Teva` meaning `nature`

## History
* The Epiphany III, was announced in October 2011 using 28 nm and 65 nm manufacturing processes.
* 16-core Adapteva Epiphany chip, E16G301, from Parallella single-board computer<br>
![](https://upload.wikimedia.org/wikipedia/commons/c/cf/Adapteva_Parallella_DK02_-_Epiphany_%2815455181926%29.jpg)<br>

## Products
* The Epiphany architecture could accommodate chips with up to `4,096 RISC` out-of-order microprocessors, all sharing a single `32-bit` flat memory space. 
* Each RISC processor in the Epiphany architecture is superscalar with `64× 32-bit` unified register file (integer or single-precision) microprocessor operating up to `1 GHz` and capable of `2 GFLOPS` (single-precision). 
* Epiphany's RISC processors use a custom instruction set architecture (ISA) optimised for single-precision floating-point,[4] but are programmable in `high level ANSI C` using a standard GNU-GCC tool chain. 
* Each RISC processor (in current implementations; not fixed in the architecture) has `32 KB of local memory`.
* Code (possibly duplicated in each core) and stack space should be in that local memory; in addition (most) temporary data should fit there for full speed. Data can also be used from other processor cores local memory at a speed penalty, or off-chip RAM with much larger speed penalty.
* The `memory architecture` is does not employ explicit hierarchy of hardware caches, similar to the Sony/Toshiba/IBM cell processor, but with the additional benefit of off-chip and inter-core loads and stores being supported (which `simplifies` porting software to the architecture). It is a hardware implementation of partitioned global address space.
* This `eliminated` the need for complex cache coherency hardware, which places a practical limit on the number of cores in a traditional multicore system. The design allows the programmer to leverage greater foreknowledge of independent data access patterns to avoid the runtime cost of figuring this out. All processor nodes are connected through a network on chip, allowing `efficient` message passing.

## Scalability
* The architecture is designed to scale almost `indefinitely`, with 4 e-links allowing multiple chips to be combined in a grid topology, allowing for systems with thousands of cores.

## Multi-core coprocessors
--------------

## EPIPHANY MULTICORE IP

### Epiphany – A breakthrough in parallel processing
* The Epiphany multicore coprocessor is a scalable shared memory architecture(可扩展的共享内存架构), featuring up to `4,096 processors` on a single chip connected through a `high-bandwidth on-chip network`(高带宽片上网络). 
* Each Epiphany processor core `includes` a tiny high performance  `floating point RISC processor` built from scratch for multicore processing, a high bandwidth local `memory system`, and an extensive set of built in `hardware features` for multicore communication. 
* The Epiphany coprocessor is `ANSI-C` and `OpenCL` programmable and works in cooperation with standard microprocessors to provide `unprecedented` level of real-time processing to performance and power constrained `mobile devices` like smartphones and tablet computers, as well as improving performance levels for an array of other parallel computing platforms.
* ![](http://www.adapteva.com/wp-content/uploads/2012/08/epiphany1.png)

### Features
* Complete multicore solution featuring a high performance microprocessor ISA(指令集架构), Network-On-Chip, and distributed memory system
* Fully-featured `ANSI-C` programmable GNU/Eclipse based tool chain
* Scalable to `1000’s` of cores and `TFLOPS` of performance on a single chip
* `1GHz` superscalar RISC processor cores
IEEE Floating Point Instruction Set
* Shared memory architecture with up to `128KB` memory at each processor node
* Zero startup-cost messaging passing
* Vector Interrupt Controller
* Distributed Multicore Multidimensional DMAs(直接存储器存取)
* `32 GB/sec` local memory bandwidth per core
* `8GB/sec` per processor network bandwidth
* `72 GFLOPS/Watt` energy efficiency
* Processor tile size of 0.5mm^2 at 65nm, 0.128mm^2 at 28nm

### Epiphany Benefits
* Out-of-the box floating point C programs enables significantly `faster` time to market and lower development costs compared to ASIC or FPGA based solutions.
* Up to `100X` advantage in energy efficiency compared to traditional multicore floating point processors offers breakthrough improvements in battery life, cost of ownership, and reliability.
* Unparalleled performance, as much as `5 TFLOPs` on a single chip, enables a new set of high performance applications.
* Low latency zero-overhead inter-core communication simplifies `parallel programming`.
* Scalable architecture allows `code reuse` across a wide range of markets and applications from smart-phones all the way to leading edge supercomputers.

### Example Configurations
![](http://www.adapteva.com/wp-content/uploads/2012/08/epiphany_data.png)

----------------------

## EPIPHANY-V: A 1024-CORE 64-BIT RISC PROCESSOR

![](http://www.adapteva.com/wp-content/uploads/e5_epiphany-1024x569.png)<br>
>a 1024-core Epiphany-V RISC processor chip at 16nm.  The chip has 4.5 Billion transistors, which is 36% more transistors than Apple’s latest 4 core A10 processor at roughly the same die size. Compared to leading HPC processors, the chip demonstrates an 80x advantage in processor density and a 3.6x advantage in memory density.

### Epiphany-V Summary
* 1024 64-bit RISC processors
* 64-bit memory architecture
* 64-bit and 32-bit IEEE floating point support
* 64 MB of distributed on-chip SRAM
* 1024 programmable I/O signals
* Three 136-bit wide 2D mesh NOCs
* 2052 separate power domains
* Support for up to One Billion shared memory processors
* Support for up to One Petabyte of shared memory
* Binary compatibility with Epiphany III/IV chips
* Custom ISA extensions for deep learning, communication, and cryptography
* TSMC 16FF process
* 4.56 Billion transistors, 117mm^2 silicon area
* DARPA funded

------------
## Epiphany-V: A 1024 processor 64-bit RISC System-On-Chip

### Abstract
This paper describes the design of a 1024-core processor chip in `16nm FinFet technology`. The chip (“Epiphany-V”) `contains` an array of 1024 64-bit RISC processors, 64MB of on-chip SRAM, three 136-bit wide mesh Networks-On-Chip, and 1024 programmable IO pins.

----------------------------------
## Processor Node Subsystem







