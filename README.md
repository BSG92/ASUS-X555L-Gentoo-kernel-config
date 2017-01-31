# ASUS-X555L-Gentoo-kernel-config

eselect profile: default/linux/amd64/13.0/systemd
This kernel configuration supports for systemd and amd64 (x86_64) architecture with UEFI

ASUS X555L Hardware Specifications

Intel core i5 - 5200U processor
4GB RAM
1GB built-in VGA
DVD Sup MTL
1TB HDD
HDMI & VGA secondary output

Technical Details

"lspci -vk" output
00:00.0 Host bridge: Intel Corporation Broadwell-U Host Bridge -OPI (rev 09)
	Subsystem: ASUSTeK Computer Inc. Broadwell-U Host Bridge -OPI
	Flags: bus master, fast devsel, latency 0
	Capabilities: [e0] Vendor Specific Information: Len=0c <?>
	Kernel driver in use: bdw_uncore

00:02.0 VGA compatible controller: Intel Corporation Broadwell-U Integrated Graphics (rev 09) (prog-if 00 [VGA controller])
	Subsystem: ASUSTeK Computer Inc. Broadwell-U Integrated Graphics
	Flags: bus master, fast devsel, latency 0, IRQ 48
	Memory at f6000000 (64-bit, non-prefetchable) [size=16M]
	Memory at e0000000 (64-bit, prefetchable) [size=256M]
	I/O ports at f000 [size=64]
	Expansion ROM at <unassigned> [disabled]
	Capabilities: [90] MSI: Enable+ Count=1/1 Maskable- 64bit-
	Capabilities: [d0] Power Management version 2
	Capabilities: [a4] PCI Advanced Features
	Kernel driver in use: i915
	Kernel modules: i915

00:03.0 Audio device: Intel Corporation Broadwell-U Audio Controller (rev 09)
	Subsystem: ASUSTeK Computer Inc. Broadwell-U Audio Controller
	Flags: bus master, fast devsel, latency 0, IRQ 49
	Memory at f721c000 (64-bit, non-prefetchable) [size=16K]
	Capabilities: [50] Power Management version 2
	Capabilities: [60] MSI: Enable+ Count=1/1 Maskable- 64bit-
	Capabilities: [70] Express Root Complex Integrated Endpoint, MSI 00
	Kernel driver in use: snd_hda_intel
	Kernel modules: snd_hda_intel

00:04.0 Signal processing controller: Intel Corporation Broadwell-U Camarillo Device (rev 09)
	Subsystem: ASUSTeK Computer Inc. Broadwell-U Camarillo Device
	Flags: bus master, fast devsel, latency 0, IRQ 16
	Memory at f7210000 (64-bit, non-prefetchable) [size=32K]
	Capabilities: [90] MSI: Enable- Count=1/1 Maskable- 64bit-
	Capabilities: [d0] Power Management version 3
	Capabilities: [e0] Vendor Specific Information: Len=0c <?>
	Kernel driver in use: proc_thermal
	Kernel modules: processor_thermal_device

00:14.0 USB controller: Intel Corporation Wildcat Point-LP USB xHCI Controller (rev 03) (prog-if 30 [XHCI])
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP USB xHCI Controller
	Flags: bus master, medium devsel, latency 0, IRQ 43
	Memory at f7200000 (64-bit, non-prefetchable) [size=64K]
	Capabilities: [70] Power Management version 2
	Capabilities: [80] MSI: Enable+ Count=1/8 Maskable- 64bit+
	Kernel driver in use: xhci_hcd
	Kernel modules: xhci_pci

00:16.0 Communication controller: Intel Corporation Wildcat Point-LP MEI Controller #1 (rev 03)
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP MEI Controller
	Flags: bus master, fast devsel, latency 0, IRQ 46
	Memory at f7224000 (64-bit, non-prefetchable) [size=32]
	Capabilities: [50] Power Management version 3
	Capabilities: [8c] MSI: Enable+ Count=1/1 Maskable- 64bit+
	Kernel driver in use: mei_me
	Kernel modules: mei_me

00:1b.0 Audio device: Intel Corporation Wildcat Point-LP High Definition Audio Controller (rev 03)
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP High Definition Audio Controller
	Flags: bus master, fast devsel, latency 32, IRQ 47
	Memory at f7218000 (64-bit, non-prefetchable) [size=16K]
	Capabilities: [50] Power Management version 3
	Capabilities: [60] MSI: Enable+ Count=1/1 Maskable- 64bit+
	Kernel driver in use: snd_hda_intel
	Kernel modules: snd_hda_intel

00:1c.0 PCI bridge: Intel Corporation Wildcat Point-LP PCI Express Root Port #1 (rev e3) (prog-if 00 [Normal decode])
	Flags: bus master, fast devsel, latency 0, IRQ 40
	Bus: primary=00, secondary=01, subordinate=01, sec-latency=0
	Capabilities: [40] Express Root Port (Slot-), MSI 00
	Capabilities: [80] MSI: Enable+ Count=1/1 Maskable- 64bit-
	Capabilities: [90] Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP PCI Express Root Port
	Capabilities: [a0] Power Management version 3
	Kernel driver in use: pcieport

00:1c.2 PCI bridge: Intel Corporation Wildcat Point-LP PCI Express Root Port #3 (rev e3) (prog-if 00 [Normal decode])
	Flags: bus master, fast devsel, latency 0, IRQ 41
	Bus: primary=00, secondary=02, subordinate=02, sec-latency=0
	I/O behind bridge: 0000e000-0000efff
	Memory behind bridge: f7100000-f71fffff
	Capabilities: [40] Express Root Port (Slot+), MSI 00
	Capabilities: [80] MSI: Enable+ Count=1/1 Maskable- 64bit-
	Capabilities: [90] Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP PCI Express Root Port
	Capabilities: [a0] Power Management version 3
	Capabilities: [100] #00
	Capabilities: [200] L1 PM Substates
	Kernel driver in use: pcieport

00:1c.3 PCI bridge: Intel Corporation Wildcat Point-LP PCI Express Root Port #4 (rev e3) (prog-if 00 [Normal decode])
	Flags: bus master, fast devsel, latency 0, IRQ 42
	Bus: primary=00, secondary=03, subordinate=03, sec-latency=0
	Memory behind bridge: f7000000-f70fffff
	Capabilities: [40] Express Root Port (Slot+), MSI 00
	Capabilities: [80] MSI: Enable+ Count=1/1 Maskable- 64bit-
	Capabilities: [90] Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP PCI Express Root Port
	Capabilities: [a0] Power Management version 3
	Capabilities: [100] #00
	Capabilities: [200] L1 PM Substates
	Kernel driver in use: pcieport

00:1f.0 ISA bridge: Intel Corporation Wildcat Point-LP LPC Controller (rev 03)
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP LPC Controller
	Flags: bus master, medium devsel, latency 0
	Capabilities: [e0] Vendor Specific Information: Len=0c <?>
	Kernel driver in use: lpc_ich
	Kernel modules: lpc_ich

00:1f.2 SATA controller: Intel Corporation Wildcat Point-LP SATA Controller [AHCI Mode] (rev 03) (prog-if 01 [AHCI 1.0])
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP SATA Controller [AHCI Mode]
	Flags: bus master, 66MHz, medium devsel, latency 0, IRQ 45
	I/O ports at f0b0 [size=8]
	I/O ports at f0a0 [size=4]
	I/O ports at f090 [size=8]
	I/O ports at f080 [size=4]
	I/O ports at f060 [size=32]
	Memory at f7222000 (32-bit, non-prefetchable) [size=2K]
	Capabilities: [80] MSI: Enable+ Count=1/1 Maskable- 64bit-
	Capabilities: [70] Power Management version 3
	Capabilities: [a8] SATA HBA v1.0
	Kernel driver in use: ahci
	Kernel modules: ahci

00:1f.3 SMBus: Intel Corporation Wildcat Point-LP SMBus Controller (rev 03)
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP SMBus Controller
	Flags: medium devsel, IRQ 18
	Memory at f7221000 (64-bit, non-prefetchable) [size=256]
	I/O ports at f040 [size=32]
	Kernel driver in use: i801_smbus
	Kernel modules: i2c_i801

00:1f.6 Signal processing controller: Intel Corporation Wildcat Point-LP Thermal Management Controller (rev 03)
	Subsystem: ASUSTeK Computer Inc. Wildcat Point-LP Thermal Management Controller
	Flags: bus master, fast devsel, latency 0, IRQ 18
	Memory at f7220000 (64-bit, non-prefetchable) [size=4K]
	Capabilities: [50] Power Management version 3
	Capabilities: [80] MSI: Enable- Count=1/1 Maskable- 64bit-
	Kernel driver in use: intel_pch_thermal
	Kernel modules: intel_pch_thermal

02:00.0 Ethernet controller: Realtek Semiconductor Co., Ltd. RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller (rev 10)
	Subsystem: ASUSTeK Computer Inc. RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller
	Flags: bus master, fast devsel, latency 0, IRQ 44
	I/O ports at e000 [size=256]
	Memory at f7104000 (64-bit, non-prefetchable) [size=4K]
	Memory at f7100000 (64-bit, non-prefetchable) [size=16K]
	Capabilities: [40] Power Management version 3
	Capabilities: [50] MSI: Enable+ Count=1/1 Maskable- 64bit+
	Capabilities: [70] Express Endpoint, MSI 01
	Capabilities: [b0] MSI-X: Enable- Count=4 Masked-
	Capabilities: [d0] Vital Product Data
	Capabilities: [100] Advanced Error Reporting
	Capabilities: [140] Virtual Channel
	Capabilities: [160] Device Serial Number <**************************>
	Capabilities: [170] Latency Tolerance Reporting
	Capabilities: [178] L1 PM Substates
	Kernel driver in use: r8169
	Kernel modules: r8169

03:00.0 Network controller: MEDIATEK Corp. MT7630e 802.11bgn Wireless Network Adapter
	Subsystem: Foxconn International, Inc. MT7630e 802.11bgn Wireless Network Adapter
	Flags: bus master, fast devsel, latency 0, IRQ 19
	Memory at f7000000 (32-bit, non-prefetchable) [size=1M]
	Capabilities: [40] Power Management version 3
	Capabilities: [50] MSI: Enable- Count=1/1 Maskable- 64bit+
	Capabilities: [70] Express Endpoint, MSI 00
	Capabilities: [100] Advanced Error Reporting
	Capabilities: [140] Device Serial Number <***************************>
	Capabilities: [150] Latency Tolerance Reporting
	Kernel driver in use: mt7630e
	Kernel modules: mt7630e

"lsusb" output
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 001 Device 003: ID 0bda:0129 Realtek Semiconductor Corp. RTS5129 Card Reader Controller
Bus 001 Device 002: ID 04f2:b483 Chicony Electronics Co., Ltd 
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub

Necessary /etc/portage/make.conf flags
CFLAGS="-march=native -O2 -pipe"
#Add "gnome X" in USE flag if you are building for gnome
USE="systemd acl alsa "
CPU_FLAGS_X86="aes avx avx2 fma3 mmx mmxext popcnt sse sse2 sse3 sse4_1 sse4_2 ssse3"
MAKEOPTS="-j5"
VIDEO_CARDS="intel"
INPUT_DEVICES="evdev keyboard mouse synaptics"
GRUB_PLATFORMS="efi-64"

Notes
VIDEO_CARDS=”intel” will add support for i915 and i965. However you can change it to “intel i965” or “intel i915”. The latter is not recommended.
Wireless device driver is not included in this configuration file.
Some acpi keys may not work - issue is yet to be handled
ASUS_WMI configuration parameter is missing
Suggestions for changes and improvements are welcome.
