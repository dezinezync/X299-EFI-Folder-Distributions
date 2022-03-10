# X299-EFI-Folder-Distributions
X299 EFI Archive for Asus X299 Deluxe II Motherboard and 9940X CPU. 

### 2022-03-09
- Added Monterey EFI for MacPro7,1 based on the Asus X299 Deluxe II BIOS version 3601 (released on 2021/11/10).
- Disable Resize bar in BIOS before using. 
- Additionally: 
  - Use only the `SSDT-X299-BASE.aml` ACPI patch for clean install. 
  - No disables needed for updates. 
- Map ACPI paths to your respective paths in the `aml` files. 
- ACPI patch only for 5700XT installed in the first slot. For a separate GPU, determine necessary patches. For separate slot, update ACPI paths accordingly. 
- Disable `ARPT` ACPI patch if not using a separate Wifi/BT card in Slot 6. Adapt ACPI paths if using a different slot. 

#### Note for updating to 11.3

When updating macOS Big Sur to 11.3, the OS will kernel panic after you run the update. 

I have confirmed that this will always be the case. 

Nothing to worry about. Just reboot your system, then in the OpenCore disk selection menu, select the **Macintosh HD** partition and that'll resume the update process. 

I have no crash reports but my guess is that the system panics when setting the boot drive information to the NVRAM. NVRAM continues to work as expected though. 
