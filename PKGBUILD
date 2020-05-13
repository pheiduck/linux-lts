# Maintainer: Jonathon Fernyhough <jonathon at_manjaro dot.org>

pkgbase=linux-lts
pkgver=5.4
pkgrel=2
epoch=1
pkgname=(
	"${pkgbase}"
	"${pkgbase}-headers"
	"${pkgbase}-acpi_call"
	"${pkgbase}-bbswitch"
	"${pkgbase}-broadcom-wl"
	"${pkgbase}-ndiswrapper"
	"${pkgbase}-nvidia-340xx"
	"${pkgbase}-nvidia-390xx"
	"${pkgbase}-nvidia-418xx"
	"${pkgbase}-nvidia-430xx"
	"${pkgbase}-nvidia-435xx"
	"${pkgbase}-nvidia-440xx"
	"${pkgbase}-nvidiabl"
	"${pkgbase}-r8168"
	"${pkgbase}-rtl8723bu"
	"${pkgbase}-tp_smapi"
	"${pkgbase}-vhba-module"
	"${pkgbase}-virtualbox-guest-modules"
	"${pkgbase}-virtualbox-host-modules"
	"${pkgbase}-zfs"
)
# Set this as default for the extramodules, override for kernel and headers
groups=(linux-lts-extramodules)
arch=('any')
url="https://www.manjaro.org/"
license=('GPL')
_kernelver="${pkgver/\./}"

# EOL kernels between last and latest LTS
eol=(
	415
	416
	417
	418
)

package_linux-lts() {
	pkgdesc="The latest LTS kernel and modules (metapackage)"
	depends=("linux${_kernelver}")
	groups=()
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}")
		conflicts+=("linux${kernel}")
	done
}

package_linux-lts-headers() {
	pkgdesc="Header files and scripts for building modules for the latest LTS kernel (metapackage)"
	depends=("linux${_kernelver}-headers")
	groups=()
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-headers")
		conflicts+=("linux${kernel}-headers")
	done
}

package_linux-lts-acpi_call(){
	pkgdesc="A linux kernel module that enables calls to ACPI methods through /proc/acpi/call (metapackage)"
	depends=("linux${_kernelver}-acpi_call")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-acpi_call")
		conflicts+=("linux${kernel}-acpi_call")
	done
}

package_linux-lts-bbswitch(){
	pkgdesc="Kernel module allowing to switch dedicated graphics card on Optimus laptops (metapackage)"
	depends=("linux${_kernelver}-bbswitch")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-bbswitch")
		conflicts+=("linux${kernel}-bbswitch")
	done
}

package_linux-lts-broadcom-wl(){
	pkgdesc="Broadcom 802.11 Linux STA wireless driver BCM43142 (metapackage)"
	depends=("linux${_kernelver}-broadcom-wl")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-broadcom-wl")
		conflicts+=("linux${kernel}-broadcom-wl")
	done
}

package_linux-lts-catalyst(){
	pkgdesc="AMD/ATI Catalyst drivers for linux. fglrx kernel module only (metapackage)"
	depends=("linux${_kernelver}-catalyst")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-catalyst")
		conflicts+=("linux${kernel}-catalyst")
	done
}

package_linux-lts-ndiswrapper(){
	pkgdesc="Module for NDIS (Windows Network Drivers) drivers supplied by vendors (metapackage)"
	depends=("linux${_kernelver}-ndiswrapper")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-ndiswrapper")
		conflicts+=("linux${kernel}-ndiswrapper")
	done
}

package_linux-lts-nvidia-340xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-340xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-340xx")
		conflicts+=("linux${kernel}-nvidia-340xx")
	done
}

package_linux-lts-nvidia-390xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-390xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-390xx")
		conflicts+=("linux${kernel}-nvidia-390xx")
	done
}


package_linux-lts-nvidia-418xx(){
	pkgdesc="NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-418xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-418xx")
		conflicts+=("linux${kernel}-nvidia-418xx")
	done
}

package_linux-lts-nvidia-430xx(){
	pkgdesc="NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-430xx")
        replaces+=('linux-lts-nvidia')
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-430xx")
		conflicts+=("linux${kernel}-nvidia-430xx")
	done
}

package_linux-lts-nvidia-435xx(){
	pkgdesc="NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-435xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-435xx")
		conflicts+=("linux${kernel}-nvidia-435xx")
	done
}

package_linux-lts-nvidia-440xx(){
	pkgdesc="NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-440xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-440xx")
		conflicts+=("linux${kernel}-nvidia-440xx")
	done
}

package_linux-lts-nvidiabl(){
	pkgdesc="Driver to adjust display backlight on modern mobile NVidia graphics adapters (metapackage)"
	depends=("linux${_kernelver}-nvidiabl")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidiabl")
		conflicts+=("linux${kernel}-nvidiabl")
	done
}

package_linux-lts-r8168(){
	pkgdesc="A kernel module for Realtek 8168 network cards (metapackage)"
	depends=("linux${_kernelver}-r8168")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-r8168")
		conflicts+=("linux${kernel}-r8168")
	done
}

package_linux-lts-rt3562sta(){
	pkgdesc="Ralink RT3562 PCI WLAN adaptors kernel module (metapackage)"
	depends=("linux${_kernelver}-rt3562sta")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-rt3562sta")
		conflicts+=("linux${kernel}-rt3562sta")
	done
}

package_linux-lts-rtl8723bu(){
	pkgdesc="Realtek 8723bu network card kernel module (metapackage)"
	depends=("linux${_kernelver}-rtl8723bu")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-rtl8723bu")
		conflicts+=("linux${kernel}-rtl8723bu")
	done
}

package_linux-lts-tp_smapi(){
	pkgdesc="Modules for ThinkPad's SMAPI functionality (metapackage)"
	depends=("linux${_kernelver}-tp_smapi")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-tp_smapi")
		conflicts+=("linux${kernel}-tp_smapi")
	done
}

package_linux-lts-vhba-module(){
	pkgdesc="Kernel module that emulates SCSI devices (metapackage)"
	depends=("linux${_kernelver}-vhba-module")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-vhba-module")
		conflicts+=("linux${kernel}-vhba-module")
	done
}

package_linux-lts-virtualbox-guest-modules(){
	pkgdesc="Guest kernel modules for VirtualBox (metapackage)"
	depends=("linux${_kernelver}-virtualbox-guest-modules")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-virtualbox-guest-modules")
		conflicts+=("linux${kernel}-virtualbox-guest-modules")
	done
}

package_linux-lts-virtualbox-host-modules(){
	pkgdesc="Host kernel modules for VirtualBox (metapackage)"
	depends=("linux${_kernelver}-virtualbox-host-modules")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-virtualbox-host-modules")
		conflicts+=("linux${kernel}-virtualbox-host-modules")
	done
}

package_linux-lts-zfs(){
	pkgdesc="Kernel modules for the Zettabyte File System (metapackage)"
	depends=("linux${_kernelver}-zfs")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-zfs")
		conflicts+=("linux${kernel}-zfs")
	done
}
