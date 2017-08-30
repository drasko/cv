## PROFESSIONAL EXPERIENCE

**Devialet Paris, France**

**R&D Software Engineer (Embedded Linux Expert)**

**March 2013 — Present (1 year)**

Work on system design of wireless digital audio system of next generation based on dual-
core ARM Cortex-A9 FPGA with custom hard-RT Xenomai-patched Yocto Poky Linux

kernel and dual-band 802.11abgn WiFi connection
 Participated in system design, both HW and SW. Electronic components selection
and sourcing. SW architecture.
 Work on Linux system: wrote scripts to automatize OS creation, prototyped the

system using Debian and Linaro Ubuntu on Pandaboard (vanilla kernel + deboot-
strap) and Wandboard (Freescale OpenEmbedded for i.MX6). Integrated Linux

for Altera FPGA CycloneV board. Created and maintained platform build sys-
tem based on Yocto and custom meta layer. Wrote Bitbake recipes and OPKG

packages. Worked on Buildroot platform builder.

 Investigated synchronization over WiFi using NTP and PTP protocols. Imple-
mented precise pulse-per-second GPIO kernel driver and used oscilloscope to ob-
serve and measure synchronization

 Proposed and integrated Xenomai hard-realtime kernel patches to obtain needed
RT performances for audio processing and communication with FPGA cores
 Participated in creation of boot and update procedure specification. Compiled
and integrated U-Boot for Altera Socfpga target and resolved problems with SPL
preloader creation and FPGA sub-system load procedure

1

 Proposed and evaluated (supplier correspondence and sample testing) WiFi mod-
ule based on Realtek RT8192DU dual band 802.11abgn SoftMAC chipset with

concurrent dual MAC and PHY, obtaining good performances in both 2.4GHz
and 5GHz bands, both as a STA and AP. Corrected Linux driver and hostapd
daemon to use cfg80211/nl80211 and helped integration on Linux mainline

 Work on Zigbee support in Linux kernel for Microchip MRF24J40 needed for re-
mote control of digital audio amplifier. Debugged issues with CycloneV SPI driver

on the electronic level (oscilloscope). Implemented 802.15.4 wrapper library.

 Architecture specification and full implementation of the Linux network man-
ager component capable of dynamic management of symulthaneous Ethernet, Wifi

(both STA and AP) and PLC connctions, based on Intel Connman project and
Qt5 framework with libconnman-qt.
Sequans Communications Paris, France
Embedded Platform Software Engineer (LTE 4G)
June 2010 — Present (2 years 6 months)
Work on platform enablement, system and device drivers for LTE multi-processor SoCs,
based on ARM946E-S, MIPS24Kc and Lattice Mico32 architectures with eCos RTOS
(for baseband CPU) and Linux (for application CPU) as a systems of choice.
 Board bring-up and HW/SW debugging (JTAG, oscilloscope, logic analyzer, ASIC

debugging, HW modifications). Work on a new SoC designs from FPGA simula-
tions and prototypes, through PCBs with first ASIC versions up to the mature

chip product
 Compiled and prepared toolchains for ARMEB, MIPSEB and LM32 architectures

based on Binutils, GCC and GDB. Tested and debugged solutions on all 3 archi-
tectures and integrated it into development build process.

 Fully ported uClinux to SQN3010 SoC application processor based on ARM946E-
S. Fully ported Linux for MIPS, OpenWRT distribution to SQN3110 FPGA chip,

and re-wrote specific configuration, Makefile, shell and Perl scripts and prepared
a series of patches in a build system.
 Implemented series of Linux device drivers (WiFi, GPIO, SDIO, ...) and low-level
and userspace services. Created SW workarounds (driver quirks) for ASIC bugs
(specification non-alignments) in third party IP cores
 Fully developed (from scratch) USIM physical layer driver and transport protocol
layers of T=0 and T=1 protocols for Smart Card communication. Used Comprion
and Micropross SC sniffers/analyzers and debugged solution. Debugged ASIC bugs
and created workarounds in SW. Debugged HW bugs using oscilloscope and logic
analyzers. Designed (specification) and implemented low-level API and created a

2

suite of unitary and productions tests
 Enabled OpenOCD open-source project for ARM946E-S and MIPS24Kc platforms,

contributing patches to the community under GPL licence. Reverse-engineered Lat-
tice Mico32 MonitorROM and third-party VHDL code. Adapted UrJTAG for very

low-level JTAG communication debugging. Wrote complex shell and TCL scripts

for usage of cheap FTDI-based USB JTAG dongles and replacing expensive third-
partner solutions, which significantly reduced development costs for the company

Given a support and training to other engineers on using implemented solution
 Fully wrote (from the scratch) scatter-gather zero-copy solution for inter-processor

communication based on parallel communication between eCos and uClinux net-
work drivers, using SW circular FIFOs and HW pointers. Developed Linux applica-
tion to test the implementation by receiving RF packets sent from the eNodeB, sent

via eCos driver and received on Linux side, and observed traffic using Wireshark
 Implemented series of eCos RTOS drivers (watchdog, nework activity GPIO, flash
handling...) and low-level services :
– IQ Mismatch driver for calculation phase, gain and offset convergence and
correction, and tested solution using tone generator and tweaking Maxim RF
chip set-up. Implemented AT commands and services for controlling of the
solution
– Implemented driver for reading ISO images stored on the NOR flash and
proper handling of sector handling and wear leveling. Implemented unitary
test eCos application by creating ISO images on host Linux and turning USB
dongles (dev boards) into ISO storage
Modified bootloader code and NVRAM configuration in the binary form
Pace (ex Philips STB) Paris, France
Embedded Software Engineer
November 2009 — June 2010 (8 months)
Low level system programming for HD TV WiFi Zapper satelite set-top box solution
based on ST7105 SoC with SH4 RISC processor, running embedded Linux as an OS of
choice.
 Work on U-Boot bootloader: rewrote U-Boot procedures and changed low-level
initialization (poke table) in order to use it with proprietary bootcode with strong
security constraints. Debugged ethernet and USB drivers.

 Wrote (in assembly language) bootstrap procedure for auto-decompression of sys-
tem binary in specific format and implemented 29/32-bit addressing mode switch

needed to boot Linux image. Implemented mechanism to pass Linux boot argu-
ments from U-Boot to kernel via bootstrap code

3

 Debugged NAND Flash driver in U-Boot and resolved timing and Bad Block man-
agement issues. Integrated similar solution in Linux system using MTD Utils and

JFFS2 filesystem

 Implemented assembly code which places Audio and Video companions (precom-
piled binaries) to correct shared memory locations before jumping to Linux entry

point and freed necessary RAM memory by reducing root filesystem size
 Attended one week educational seminary and courses titled ”Embedded Linux
kernel and device drivers programing” organized by ORSYS group in Paris, France

 Work on Linux kernel security hardening by re-configuring kernel, rootfs (Busy-
box), uClibc and user-space scripts to respect security constraints

 Implemented kernel module to read NVRAM and trigger userspace helper pro-
grams for mtd subsystem processing

SPiDCOM Technologies Paris, France
Embedded Software Engineer
December 2008 - November 2009 (1 year)
Firmware design and implementation for new SPiDCOM SPC300 HomePlug AV protocol
(powerline communication) compliant SoC. Creation of BSP and Linux (with U-Boot)
SW bundle for ARM based chip

 Work on the U-Boot and board bring-up: implemented SDRAM controller config-
uration (ARM assembly), enabled MMU and DCache for image load optimization.

 Designed (specification creation) a custom protocol for firmware update based on
Ethernet-type Homeplug AV MME messages and implemented it in C. Wrote PC
host client application (based on Linux raw sockets) to test and debug protocol
implementation.
 Fully wrote MAC controller (Ethernet) driver and enabled TFTP image boot

 Designed (specification creation) a custom protocol for FW update based on Ethernet-
type Homeplug AV MME messages and implemented it in C. Wrote PC host client

application (based on Linux raw sockets) to test and debug protocol implementa-
tion

 Implemented (ARM assembly) code for autodetection of parameters stored on flash
used on board wake-up and debuged implementation with jtag and GDB. Wrote
OpenOCD jtag and GDB scripts to speed up debugging process
 Wrote (in C) Linux image boot procedure that supports dual image booting with
candidate selection based on parameters stored in custom image headers. Wrote
user space applications for creating these headers and modified Buildroot Makefiles

4

to enable their pre-pending on image build
 Implemented (from scratch) library for manipulating ethernet type MME message

structures and wrote unitary and functional tests in a form of multithreaded appli-
cation (POSIX threads) using libcheck and TUN/TAP virtual Ethernet interface.

 Implemented (from scratch) library for system configuration and wrote unitary
and functional tests
Texas Instruments Nice, France
Multimedia Software Engineer
July 2006 - December 2008 (2 year 7 months)
DSP Architecture and Applications Group
Module-level verification of In-Loop DeBlocking Filter and Motion Estimation modules
for digital video coding (compliant to several modern standards: H.264, MPEG-4, etc.),
part of the IVA Hardware Accelerator for OMAP4 platform
 Fully wrote C testbenches, embedding them in the reference decoder code (provided
by third party vendors) and programmed filter C model; Development done on
Windows (MS Visual C++ development environment) and Linux

 Ported all code to Linux and developed C interface and synchronization mecha-
nism to enable IPC with Specman RTL simulation tool in order to test Verilog

(hardware) code

 Wrote various Perl scripts and created Perl/Tk GUI application to enable auto-
matic running of the tests, automatic logging and report creation.

 Defined and implemented (in C) functional coverage and algorithms to extract
minimum set of testing conformance video bitstreams needed for full coverage
GSM/GPRS/EDGE L1 Software Engineer
Layer 1 Non-Regression testing and tool development
 Provided in depth testing support during GSM/GPRS/EDGE Layer1 Real-time
embedded software development
 In charge of MCU and DSP L1 SW non-regression testing spread over several
programs that used several TI OMAP platforms with ARM 9 / ARM 11 and TI
C55x DSP

 Extensive laboratory experience - proficiency with various modern mobile tele-
phony protocols test equipment (ANITE, RACAL, CRTU, CMU200, CRTP, etc.)

 Analyzed L1 Trace, troubleshooted L1 sofware in case of issues

5

 Fully developed GSM Voice audio loopback and BER test cases, implemented
complete automation of GSM Voice test process for RACAL AIME 6103.
 Developed ANITE/Agilent SW applications (in C) for testing 2G/UMA (GAN)
handovers
FNX Solutions Belgrade, Serbia
Software Engineer
August 2005 - July 2006 (1 year)
FNX SIERRA System (system for the management and processing of capital market
transactions) development and debugging

 Worked on system coding in C under Solaris within the international team, re-
motely connected to servers in Philadelphia, USA

 Designed and implemented various business objects and data transfer objects used
within a system for database connectivity. Implemented a crucial part of Oracle

database port by adapting various libraries used for application/database commu-
nication.

 Thoroughly debugged and resolved issues for risk-management applications (sys-
tem, network and GUI)

 Programmed and designed various database triggers, table and update scripts,
stored procedures, etc., in SQL, Transact-SQL and PL/SQL, migrating system
from Sybase to Oracle

 Fully wrote various Perl and BASH scripts and successfully implemented automa-
tization of development process

Innovational Centre of School of Electrical Engeneering Belgrade, Serbia
Research Assistant
August 2004 - August 2005 (1 year 1 month)

LINSEC - Linux Security and Protection System, project introducing Mandatory Ac-
cess Control (MAC) mechanism into Linux (as opposed to existing Discretionary Access

Control mechanism)
 Linux kernel hacking (file system domain access control, socket access control)
 Ported the legacy system on 2.6.x ”vanilla” kernel and resolved various errors due
to GCC incompatibility issues
 Developed enhance for user-space tools for controlling the system patch

6

OPEN SOURCE PROJECTS
GNU and FOSS evangelist, implicated in many open source projects in domains of
development, maintaining, documentation and support.
 OpenOCD (http://openocd.sourceforge.net/)
The Open On-Chip Debugger (OpenOCD) aims to provide debugging, in-system
programming and boundary-scan testing for embedded target devices.
– Added support for ARM946E-S architecture
– Corrected MIPS32 code and added microcode and coprocessor routines for
cache handling
– Documented MIPS32 implementation and functionalities
 WeIO (http://we-io.net)
Project aims at bringing rapid prototyping and ”Internet of Things” platform under

FOSS licence for both HW and SW. Homebrew ”from the scratch” DIY implemen-
tation is employed.

– Project co-author, designer and main system architect
– First version of WeIO - based on ARM Cortex-M3 LPC1768 with NuttX
RTOS:
 Communication and co-operation with MicropendousX Open Hardware
project on PCB design.

 Electronic components selection and ordering and DIY fabrication (sol-
dering of the HW development boards using PCB re-flow technique)

 Enabled OpenOCD low-level JTAG debugging. Wrote TCL configuration
scripts and test for HW sanity checking.
 Compiled and prepared toolchain based on GCC and Binutils and wrote
build system as a combination of Bash shell scripts and set of Make files
 Integrated ARM CMSIS low-level libraries and drivers for NXP LPC1768
(ARM CORTEX-M3) architecture
 Ported NuttX RTOS to WeIO platform (mbed port adaptation)
– Second version of WeIO - OpenWRT Linux on Qualcomm-Atheros AR9331
MIPS based WSoC and ARM Cortex-M0 LPC11u24:
 Adapted OpenWRT for WeIO board and wrote missing Linux drivers
 Designed and implemented embedded web application that is based on
Torando Python asynchronous websocket server for backend and on Twit-

7

ter Bootstrap and jQuery for HTML5/Javasctipt front-end. Specified and
implemented muti-threaded user API
 Wrote from the scratch WiFi configuration and connection manager in
Python capable of handling both AP and STA modes
 Participated in design of HW board and debugged problems with HW

- SD card detection, USB power consumption, WiFi RF signal interfer-
ence...

 Designed, implemented and maintained project’s website, mailing list and
documentation (asciidoc, GitHub, Dokuwiki, markdown)
 Led professional partnership and cooperation with Litvanian HW system
company ”8Devices” working on for HW implementation and fabrication
 Codezero OpenRISC Port (http://opencores.org/project,c0or1k)
Codezero is a new L4 microkernel that has been written from scratch, following the
latest development and research principles on microkernel design. Project c0or1k

aims at porting this microkernel to general purpose open source RISC CPU archi-
tectures.

– Main maintainer of the project
– Modified SCons and CML2 configuration and build system and implemented
set of Python development utilities
– Ported C0 code OpenRISC 1000 architecture

EDUCATION
Diploma Engineer (equivalent to M.Sc.)
School of Electrical Engineering, University of Belgrade
department of Electronics, Telecommunications and Control
Master Thesis in Audiotechnics : ”Analysis of Methodes And Applications for Arti-

ficial Reverberation”, department of Telecommunications, School of Electrical Engeneer-
ing, Belgrade, Serbia

Student projects:
 RT application for railroad traffic signaling and organization written in C++ using
API of a custom RT kernel
 Retriggerable timer with 7-seg display based on PIC16F84 uC written in assembly
(MPlab IDE)

8

 10-band audio equalizer schematic and layout implementation in Protel package
 JK flip-flop VLSI layout done in Magic VLSI tool
FOREIGN LANGUAGES
 English (excellent)
 French (good)
 Russian (understanding)
 Serbian (mother tongue)

PERSONAL INTERESTS
 Music playing (guitar) and sound and video production using GNU tools
 Contemporary and fine art photography, analogue and digital
 Karate (karateka and official member of French Karate Federation)
 Film, literature and philosophy
