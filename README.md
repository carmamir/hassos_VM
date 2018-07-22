# hassos_VM

Here you can find an OVA/OVF and VHD/VHDX files base on the HassOS Project.

steps:
  1.The vmdk file is downloaded from here https://github.com/home-assistant/hassos/releases
  2.A VM is created on Oracle VM VirtualBox
  3.The VM get exported to ova Version 1/2
  4. ova V1 is inported to VMware Workstation Pro 14 (or ESXI 6.5)
  5. VM get exported to ovf and vmdk (disk)
  
  6.TBD (hyper-v) 

  VM settings:
    Name: HassOS{version}
    Type: Linux
    Version: Other linux (64bit)
    Ram: 2048
    Cpu: 2
    Motherboard: EFI
    Network: NAT
    
    
  

More Info here : https://github.com/home-assistant/hassos/

HassOS
Hass.io OS based on buildroot. It's a hypervisor for Docker and supports various kind of IoT hardware. It is also available as virtual appliance. The whole system is optimized for embedded system and security. You can update the system simple with OTA updates or offline updates.

Focus
Linux kernel 4.14 (LT)
Barebox as bootloader on EFI
U-Boot as bootloader on IoT
RAUC for OTA updates
SquashFS LZ4 as filesystem
Docker 18.03.1
AppArmor protected
ZRAM LZ4 for /tmp, /var, swap
Run every supervisor
