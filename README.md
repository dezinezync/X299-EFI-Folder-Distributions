# X299-EFI-Folder-Distributions
X299 EFI Archive for Asus X299 Deluxe II Motherboard and 9940X CPU. 

#### Note for updating to 11.3

When updating macOS Big Sur to 11.3, the OS will kernel panic after you run the update. 

I have confirmed that this will always be the case. 

Nothing to worry about. Just reboot your system, then in the OpenCore disk selection menu, select the **Macintosh HD** partition and that'll resume the update process. 

I have no crash reports but my guess is that the system panics when setting the boot drive information to the NVRAM. NVRAM continues to work as expected though. 
