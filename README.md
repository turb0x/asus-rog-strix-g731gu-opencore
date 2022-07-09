# OpenCore - Asus ROG Strix G17-G731GU
![Screenshot](Screenshots/screenshot.png)

### **Laptop Specifications 💻**
- **Processor:** Intel Core i7-9750H
- **iGPU:** Intel UHD630
- **dGPU:** Nvidia GeForce GTX 1660TI
- **RAM:** 16GB
- **Storage:** Micron 2200V NVMe / Kingston A400
- **Audio:** Realtek ALC294

### **Disabled ⚠️**
- Nvidia GeForce GTX 1660TI (not supported)
- Micron 2200V (not supported)

### **Fully Working✅**
- Intel UHD630 (144hz, brightness, sleep)
- Audio (speakers, jack, bluetooth)
- Bluetooh (native)
- Touchpad (incl. gestures)
- Ethernet
- FaceTime
- iMessage
- All USB ports etc.

### **Limited Functionality☑️**
- Wi-FI (use AirportItlwm.kext and HeliPort to get it working)

### **Not Working❌**
- AirDrop (replace the Wi-Fi Card with a compatible one)
- HDMI / USB-C Display Output (due to disabled dGPU)

### **Bios Settings🪛**
- Disable FastBoot
- Disable SecureBoot

### **Hardware Changes🔨**
- Using Kingston A400 SSD instead of Micron 2200V (read important notes)
- ***In the future:** Getting a compatible Wi-FI card*

### **IMPORTANT NOTES❗**
- **OpenCore:** 0.7.1 (had trouble when updating, things are breaking)
- Kexts are updated to the latest version (07/09/2022)
- Micron 2200V is not supported by OpenCore/Apple. Same as Samsung EVO PLUS. This is the reason I am using the Kingston one. NVMe one is disabled trough SSDT-DiscreteSpoof-EVO-Plus.aml
- Got the EFI from u/TLunchFTW. Fixed audio jack, brightness, sleep, nvme kernel panic, improved boot/startup time, got rid of some kexts, cleaned config.plist
