## Apply for Radxa CM3

Radxa is donating some free [ROCK3 computing modules](https://wiki.radxa.com/Rock3/CM3) to open source hardware projects.

## How to apply

Send a new PR to this repository on GitHub, append your application table(sort Project Name). Radxa team will review/ask questions/discuss about the project detail. If the project is interesting or welcomed by the community, we will approve it. Radxa Team will contact the developer for the further sample shipping&development etc.

## CM3 projects list:

| Project Name        | CM3 Model     | Hardware(Carrier Board)                                      | Software                                                | Notes                                                        |
| ------------------- | ------------- | ------------------------------------------------------------ | ------------------------------------------------------- | ------------------------------------------------------------ |
| AI-Speaker          | RM116-D8E\*   | Custom design                                                | [AI Speaker](https://ai-speaker.com/docs/ais_app_index) | We would like to release something like Home Assistant Amber dev board with Radxa CM3 |
| Buildroot           | RM116-D1E0    | Radxa E23                                                    | [Buildroot](https://buildroot.org/)                     | Adding CM3 support for buildroot                             |
| currypi             | RM116-D8E\*   | [CurryPi](https://github.com/devguardio/currypi)             | Linux                                                   | [Pictures](https://twitter.com/arvidep/status/1445363759313297412) |
| Device Farm         | Any           | Any                                                          | [Device Farm](https://github.com/device-farm)           | DEVICE.FARM is a platform to deploy containerized services to IoT devices, similar to Balena. We need the board for testing before we publish them as supported. |
| Gram Research kiosk | RM116-D2E0W   | Currently the RPi CM4 + LCD                                  | Raspbian/Linux                                          | Custom carrier board for compute module, integrated into slim 2k resolution LCD shell. Project will be open sourced when it is completed, currently it's not public. Here are some early photos: https://i.imgur.com/3xsmMi8.png https://i.imgur.com/irzZMza.png |
| K3s ARM cluster     | RM116-D8E8    | 6 x Rpi CM4                                                  | Ubuntu                                                  | Testing Kubernetes on AArch64 micro clusters                 |
| Lemuria IIoT        | RM116-D1E8(W) | Custom design                                                | [Yocto](https://gitlab.com/linumiz/lemuria/meta-lemuria)/Buildroot (TODO based on Rockchip buildroot/mainline kernel)                                         | Upcoming open souce Industrail IoT hardware with following key features, 12 - 75V DC wide operating range, 5 x UART (RS232/485), 2 x CANFD, 6 x Digital Output, 6 x Digital Input, 4 x Analog Input, 2 x Ethernet, Security (TPM - SLB9670, ATECC608B), 1 x M2.0 for CAT 4 LTE, RTC (with super capacitor), 1 x USB Host port, 1 x MIPI DSI (for future expansion of panel PC). Currently the version 1 of the hardware is functional tested with RPi CM4 and SOQuartz (external eMMC with manual patching). Plan is to deliver the functional software based on custom embedded Linux based on Buildroot/Yocto. Note: Project will be open sourced with documentation after test completion for Version 2. |
| MEMESat-1           | RM1116-D4E0W2 |Custom design                                                 | [Buildroot](https://buildroot.org/)                     | I am with the Small Satelite Research Lab at the University of Georgia. We are looking for a computer to use in one of our projects launching next year. With the CM4 being out of stock everywhere, we are trying to find an alternative with the same form factor. We want to sample this SBC for possible integration. This satellite will be used as an education platform during STEM outreach by our customer Let's Go to Space.
| MSLA resin printers | RM116-D4E32W  | Currently the RPi CM4 + LCD                                  | Raspbian/Linux                                          | The project is currently in experimental state, I am working on Linux driver for current state-of-the-art LCDs featured on resin printers. However, these LCDs use 2x 4-lane MIPI interface, thus I am experimenting with multiplexing MIPI on Rpi CM4 (which sucks). This is why I am reaching out to you - as ROCK3 features 2x 4-lane MIPI! This is a killer feature for such a project. Just to give you context; the resin 3D printing is extremely limited a dominated by Chitusystems. They have terrible closed ecosystem, unlike the open ecosystem available for FDM printers. It is really hard for open project to start, as there is a big obstacle in driving high-resolution LCDs required for these printers. |
| NixOS               | RM116-D4E32W  | Radxa E23                                                    | NixOS                                                   | -                                                            |
| OpenBSD             | RM116-D8E32W  | Radxa CM3 IO Board (or Radxa E23)                            | [OpenBSD](https://www.openbsd.org/)                     | I would like add support for the Radxa CM3 to OpenBSD and continue to help port [UEFI](https://github.com/jaredmcneill/quartz64_uefi). |
| OpenPlotter         | RM116-D4E16W  | Radxa CM3 IO Board                                           | [OpenPlotter](https://openmarine.net/openplotter)       | I would like to look into running the OpenMarine/Openplotter platform on the Radxa CM3 + the IO board, with a special focus on using the UARTS for NMEA-0183 communication. The RM116-D4E16W is the somewhat economical choice, and it could be interesting to see how much functionality could be packed onto an RM116-D8E32W. |
| OpenWRT             | RM116-D1E0    | Radxa E23                                                    | [OpenWRT](https://openwrt.org/)                         | I would like to port Openwrt on CM3 + Radxa E23 carrier board |
| Piunora             | Any with WiFi | [Piunora Pro](https://www.crowdsupply.com/diodes-delight/piunora) | Linux                                              | For compatability testing and new hardware designs           |
| RadBook             | RM116-D4E16W  | Custom                                                       | Linux                                                   | A generic netbook motherboard schematic in KiCAD, for upgrading existing Atom-based devices from 2010s. Community will be encouraged to submit their PCB designs fitting aftermarket computers. A reference design for em350 will be provided, however a board for vastly popular eeePC would probably gain a lot of attention. Currently only Radxa CM3 is suitable, due to its unique LVDS output feature.
| Seaberry Pi         | Any           | Custom Design, standard Mini-ITX form factor                 | Linux                                                   | The Seaberry Pi is a full-featured Raspberry Pi CM4 or Radxa CM3 carrier board in a standard Mini-ITX form factor that exposes the PCIe bus to a variety of different connector types, which include one M.2 Key M slot for NVME SSD, four PCIe Mini connectors, four PCIe M.2 Key E connectors (with dual PCIe and dual Reset lines support to accommodate  dual Coral AI TPU M.2 modules), one x16 standard PCIe add-on card connector (x1 PCIe Lane functionality), and one x1 PCIe side connector. Full description and data can be found here: https://www.tindie.com/products/alftel/seaberry-pi-cm4-carrier-board/ |
| sataPi              | Any model     | Custom PCB design WIP                                        | Debian                                                  | sataPi is a project that aims to fill the empty sata bay slots from a pc case with computing power. Since it is inside a pc, the power will be delivered trough standard conectors in pcs like molex or sata power. Project will be fully opensource, and maybe there will be a kickstarter campaign for it. |
| [Steward Camera](https://www.stewardai.com/) | RM116-D8E16W     | [Waveshare carrier board](https://wiki.radxa.com/Rock3/CM3/wavesharecm4iobase) | Linux | Open source phentotyping hardware, using NIR + RGB cameras + environment sensors. Designed to be used by farmers, implementing the latest in agriculture research.  |
| -                   | RM116-D4E32W  | Currently the RPi CM4 + LCD                                  | Raspbian/Linux                                          | Project will be open sourced closer to going on sale, currently it's not public, details and photos can be shared privately. There is some tease photos [here](https://twitter.com/arturo182/status/1364003299083624452). |
| -                   | RM116-D8E8W   | Radxa E23 Dual Ethernet board                                | Yocto                                                   | Trying to replace an STM32MP1 with a CM3 for a Home Firewall Project (to be released when in presentable state) |
| Turing Pi 2         | Any           | Turing Pi 2                                                  | Kubernettes / Raspian / Debian                          | Raspberry Pis are almost impossible to find. Turing PI 2 just released. Curious if this drop in replacement would work. 1 would be enough, 4 would be better as there are 4 slots|  
| Robot-T500          | RM116-D4E16   | 10" Robot Industrial Terminal                                | Yocto                                                   | Need replacement for Pi CM4. This device is LAN based and optionally Wifi based vehicle mount.            | 
| [Upverter](https://modular.upverter.com)            | Any           | Customizable Carrier Board                                   | Linux                                                   | Add Radxa CM3 support to Modular Upverter |
| Jago Carrier Board            | Any (prefer RM116-D8E64W)           | Drone Carrier Board to interface CM3 with Cube Flight Controller                                   | Linux                                                   | Add Radxa CM3 support to Menapia's Jago Carrier Board for drone companion computer |
| H264/H265 NAE           | Any with Wifi and eMMC (prefer RM116-D8E64W)           | Any                                   | Custom Linux/Yocto/Android                                                   | We would like to ultise CM3 to explore and improve Media Process Platform Drivers, specailly as it also has the newer IP on the slicon including H265 and to also create HDMI RX HAT to allow HDMI capture. network adaptive video encoder application |
