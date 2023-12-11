#  IP-KVM based on Raspberry Pi 3B+

A very simple and fully functional Raspberry Pi-based KVM (Keyboard-Video-Mouse) over IP that you can make with your own hands. This device helps to manage servers or workstations remotely, regardless of the health of the operating system or whether one is installed. You can fix any problem, configure the BIOS, etc.

![](/img/screen1.png)

[**View build images here**](https://imgur.com/a/om2y8T7)

# Features
* Supported **Raspberry Pi 3B+** (low cost);
* **FullHD video** using advanced **HDMI-to-CSI bridge**;
* Extra low **video latency** with **MJPEG** or **H.264 / WebRTC**;
* USB **Keyboard** and **mouse** (with leds and the wheel);
* **Control the server power** using ATX functions;
* Access via **Web UI** or **VNC**;
* Ability to use **IPMI BMC**, **IPMI SoL**, **Redfish** and **Wake-on-LAN** to control the server;
* **The ready-made OS** with read-only filesystem;
* **Extensible authorization** and HTTPS out of the box;
* **Health monitoring** of the Pi;
* Control **GPIO** ports and **USB relays**;
* 100% Open Source from [pikvm.org](https://pikvm.org/)!

# Components
* 1 x Raspberry Pi 3B+
* 1 x Arduino Pro Micro (based on an ATMega32u4) **(An Arduino with a USB Type C port was used in this build to save costs, however, the version with a USB Micro-B connector is recommended.)**
* 1 x [Usb Type C Male Connector Plug on PCB](https://articulo.mercadolibre.com.ar/MLA-1162628212-conector-ficha-usb-tipo-c-macho-en-pcb-pack-x-2-unidades-_JM) **(Only if the Arduinio Pro Micro has a USB Type-C connector.)**
* 1 x [HDMI to CSI Camera Adapter for Raspberry Pi](https://articulo.mercadolibre.com.ar/MLA-1100779294-modulo-capturadora-de-video-dcdz-hdmi-a-csi-2-raspberry-pi-_JM)
* 1 x [Logic Level Converter (Bi-Directional)](https://ar.mouser.com/ProductDetail/474-BOB-12009)
* 4 x [MOSFET relays G3VM-61A1](https://ar.mouser.com/ProductDetail/653-G3VM-61A1)
* 2 x 4.7k Ohm resistors (or 2.2k-10k Ohm)
* 5 x 390 Ohm resistors (or 220-510 Ohm)
* 1 x NPN 2n2222 transistor
* 1 x [PCB 7x9cm (25x30 750 Holes)](https://articulo.mercadolibre.com.ar/MLA-632050891-pcb-placa-experimental-simple-7x9-prototipos-electronica-fr4-_JM)
* Wires & Pin strip for Arduino (You will probably also need heat shrink to assemble some cables such as USB Type-C to USB Type-A.)

# Connections diagram
![](/img/pikvm-final_bb.png)
On the left side you can see the diagram on a breadboard, so that it is easy to understand at a glance. And on the right side the same connections but on the PCB. **(You can download the Fritzing project from this repository, file "pikvm-final.fzz")**

# Arduino HID
Follow the instructions here: https://docs.pikvm.org/arduino_hid/#usb-keyboard-and-mouse

# Pi-KVM SO Download (for Raspberry Pi 3)
* Mega: https://mega.nz/file/UuBjiSgD#TGXlGBxAJB8cK0ZNSkAHrQL38OGOXV9_WqDlu6VqH9A
* Mediafire: https://www.mediafire.com/file/28p6man652wa1f1/v0-hdmi-rpi3-20231126.img/file

# Pi-KVM 3D Case
Tinkercad 3D Project (editable): https://www.tinkercad.com/things/hFE8NpzRvNz-case-for-pikvm-raspberry-pi-3b?sharecode=QYlnFqMV2veGFuivIpqonMM-rSSZrF0tjvj67tX9D_4

STL's:
* Mega: https://mega.nz/folder/Vu4n1ICA#bGvXNo29iyuSNVrqOVY5tw
* Mediafire: https://www.mediafire.com/folder/zcbmjd3c9h0in/Pi-KVM_STL's