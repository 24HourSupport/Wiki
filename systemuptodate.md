# 24 Hour Support Wiki

[Return to main wiki page](https://github.com/CommandMC/24HS-Wiki/blob/main/index.md)
 
## Making sure your system is up to date

Most of the times issues arise when one's system is out of date. This is due to either one part of the system being out of date and the rest being up to date, or developers targeting newer versions and being on an old one. Here it will be explained what to look out for to make sure you are up to date, in order. 

## Windows and GPU drivers

1. Download the [24HS-Automator](https://github.com/CommandMC/24HS-Automator/releases/latest)
2. Run it and accept the UAC prompt.
3. Select the 2nd option (<samp>(2) Check update status</samp>) by pressing <kbd>2</kbd> on your keyboard.
4. Follow the on-screen instructions.

<details>
  <summary>Old instructions</summary>
    
### Windows 

DO NOT JUST CHECK WINDOWS SETTINGS FOR UPDATES. DO THAT AFTER FOLLOWING THIS.

I REPEAT. DO NOT JUST CHECK WINDOWS SETTINGS FOR UPDATES, JUST BECAUSE IT SAYS YOU ARE UP TO DATE DOES NOT MEAN YOU ARE UP TO DATE.

Do `Windows key + R` and type in `winver` and `enter`. See what version you are on, this is a 4 digit number (21H1 being rolled out right now). At the time of writing this the latest is 21H1, with new releases coming every 6-8 months. 21H1 means year 2021, first half of it. [See this photo to verify what you should be looking for](https://imgur.com/a/pzr0fyY)

While Windows does support older versions for months after newer ones come out (look at dates here: https://en.wikipedia.org/wiki/Windows_10_version_history#Channels ) it is recommended to be on the latest version as that is the version developers are targeting. 

If version is not 21H1 (at the time of writing) and if the windows update settings section did not offer you the update to 21H1 , it means you have not been pushed to the newer branch. Force the update by just using the update assistant https://go.microsoft.com/fwlink/?LinkID=799445

Once you are on **the latest version** THEN you check for Windows updates in settings

### Drivers 

#### Graphic card drivers

Often times users are not notified of updates from AMD and Nvidia. Being out of date can cause issues especially in games. 

Checking your graphic card driver version varies

If your graphic driver is up to date or out of date, it may be a good idea to follow the wiki entry on DDU, it is all explained here: https://docs.google.com/document/d/10cY1eNt3o_BpTHLtOsS3CkCXa3ugejCygNJqpohbRkc/edit?usp=sharing

#### DO DDU EVEN IF THE DRIVER IS ALREADY UP TO DATE. CLICK THE ABOVE WIKI AND FOLLOW IT
</details>

## Chipset drivers

Chipset drivers being out of date often cause stability issues, especially if you are an early adopter and may be on an earlier version.

### AMD:
Go to the start menu and look up Device manager. Right click on a chipset (might find under "system devices"), select properties, go to driver tab and check the version.  
Now that you have the version, identify which AMD motherboard you have and get the latest drivers from AMD:
<ul>
  <li>

[B550](https://www.amd.com/en/support/chipsets/amd-socket-am4/b550)
  </li>
  <li>

[B450](https://www.amd.com/en/support/chipsets/amd-socket-am4/b450)
  </li>
  <li>

[B350](https://www.amd.com/en/support/chipsets/amd-socket-am4/b350)
  </li>
  <li>

[X570](https://www.amd.com/en/support/chipsets/amd-socket-am4/x570)
  </li>
  <li>
      
[X470](https://www.amd.com/en/support/chipsets/amd-socket-am4/x470)
  </li>
  <li>

[X370](https://www.amd.com/en/support/chipsets/amd-socket-am4/x370)
  </li>
  <li>

[A320](https://www.amd.com/en/support/chipsets/amd-socket-am4/a320)
  </li>
  <li>

[A520](https://www.amd.com/en/support/chipsets/amd-socket-am4/a520)
  </li>
</ul>

If you do not have the latest version, please update. Note this step may require you updating your BIOS, or it may be a required step to update your BIOS.  
Consult your motherboard page on updating BIOS and chipset drivers for more information.

### Intel: 

Intel rarely has any issues with chipset drivers out of date, however you can [download their utility](https://downloadcenter.intel.com/product/1145/Intel-Chipset-Software-Installation-Utility) to make sure.  
But you rarely need to worry about this. Windows updates typically pushes them fairly frequently.

## Other drivers
If you have an issue with a device in particular, for example your mouse, it may be a good idea to uninstall the driver and clean install it.  
Go to the start menu and look up Device manager. Search for the device you are having issues with, right click it and click Uninstall. Click uninstall software and once done restart your computer. If you are still having issues please grab the drivers from the device's page for drivers.

## BIOS/UEFI
NOTE: Updating BIOS may be risky depending on your configuration, please have backups of your data! And consult your motherboard's page on updating BIOS. Some motherboards require you to update chipset drivers before continuing or to be on a certain version before updating to the latest one. PLEASE CONSULT YOUR MOTHERBOARD UPDATING INSTRUCTIONS.  
You can open up system information from the start menu and your BIOS/UEFI version will be shown there. Then consult the motherboard page for your BIOS/UEFI and see if you have the latest version. If you do not, please follow the manual provided by your motherboard manufacturer on updating. Popular guides are shown here:  
<ul>
  <li>
    
[ASUS](https://www.asus.com/us/support/FAQ/1012815)
  </li>
  <li>
    
[Gigabyte](https://www.gigabyte.com/FileUpload/global/WebPage/20/images/utiltiy_qflash_uefi.pdf)  
Make sure to read the notes (if any) on your BIOS page, as often there're complications.  
If your Gigabyte board supports QFlash you can [follow this guide, substituting for your BIOS](https://www.youtube.com/watch?v=7cQLYROKJ_Q)    
  </li>
  <li>
    
[MSI](https://us.msi.com/support/technical_details/MB_BIOS_Update)
  </li>
  <li>
    
[ASRock](https://www.asrock.com/support/BIOSIG.asp?cat=BIOS10)  
**Warning: Newer BIOS often do not officially support older CPUs, please look at notes. If you update the BIOS and your CPU is not supported, it may cause issues and ASRock will not honor your warranty for this.**  
ASRock boards have issues updating BIOS/UEFI at times. It varies by motherboard. Please consult the forums on others experiences with updating before doing so
  </li>
</ul>
