# 24 Hour Support Wiki

[Return to main wiki page](https://github.com/CommandMC/24HS-Wiki/blob/main/index.md)

### Changing GPUs
If you are changing GPUs (and aren't already on the new GPU), follow [this Wiki](https://github.com/CommandMC/24HS-Wiki/blob/main/changinggpus.md)

### Why should I do DDU?
DDU clean installs GPU drivers to eliminate the possibility of any driver or software conflicts. It is not a long process, and can quickly eliminate potential issues you may be having with your GPU.

Attempting to do this with the “clean install” option in the NVIDIA installer is not the same, as it does not thoroughly delete the GPU drivers and all NVIDIA software as DDU does. The current effect after you use this driver removal tool will be similar as if its the first time you install a new driver just like a fresh, clean install of Windows. 

### What is DDU?
Display Driver Uninstaller is a driver removal utility that can help you completely uninstall AMD/NVIDIA/Intel graphics card drivers and packages from your system, trying to remove all leftovers (including registry keys, folders and files, driver store).

The AMD/Nvidia/Intel video drivers can normally be uninstalled from the Windows Control panel or select the "clean install" option during installation, this driver uninstaller program was designed to be used when you need to thoroughly delete video card drivers and their related software.

The current effect after you use this driver removal tool will be similar as if its the first time you install a new driver just like a fresh, clean install of Windows.

The built in "clean install" functionality of the driver is NOT an alternative to DDU. This option only resets settings, **DDU removes EVERYTHING related to the driver**, and allows you to do a clean install properly. This will remove ANYTHING related to the driver (like GeForce Experience, AMD ReLive, etc)

### Option 1: The automated way
1. Download the [24HS-Automator](https://github.com/CommandMC/24HS-Automator/releases/latest)
2. Run it and accept the UAC prompt.
3. Select the 8th option (<samp>(8) Auto-DDU</samp>) by pressing <kbd>8</kbd> on your keyboard.
4. Follow the instructions on-screen

### Option 2: The manual way
<details>
  <summary>Expand me</summary>

## Creating a local account

If you're using a Microsoft Account, you will not be able to log in once you're inside Safe Mode. To find out if you're using a Microsoft Account:
1. Press the Windows key + R to open the "Run" dialog
2. Type in `powershell -Command Get-LocalUser -Name %USERNAME% ^| Select-Object PrincipalSource`
3. You will see either "Local" or "MicrosoftAccount".

If you see "Local" here, you can [skip to the next section](https://github.com/CommandMC/24HS-Wiki/blob/main/ddu.md#prerequesites). Otherwise, follow these steps:

1. Press the Windows key + R to open the "Run" dialog
2. Type in "cmd" and press <kbd>Ctrl + Shift + Enter</kbd>
3. A new window with the title "Administrator: Command prompt" will pop up.
4. In this window, type in `net user LocalAdmin /add` to add a new account with the name "LocalAdmin"
5. Once that's finished (should only take a second), type in `net localgroup Administrators LocalAdmin /add` to make this newly created account an administrator

## Prerequesites

### 1. Make sure your Windows is up to date

This section has its own Wiki entry [here](https://github.com/CommandMC/24HS-Wiki/blob/main/systemuptodate.md)

### 2. Download the drivers for your GPU

<ul>
  <li>

[//]: # (nvidiaGPU)
[NVIDIA](https://us.download.nvidia.com/Windows/496.13/496.13-desktop-win10-win11-64bit-international-dch-whql.exe)
  </li>
  <li>

[//]: # (amdGPU)
[AMD](https://ftp.nluug.nl/pub/games/PC/guru3d/amd/2021/radeon-software-adrenalin-2020-21.10.1-win10-win11-64bit-oct5.exe)
  </li>
  <li>

[Intel](https://downloadmirror.intel.com/28425/a08/Intel-Driver-and-Support-Assistant-Installer.exe)
  </li>
</ul>

Save the driver somewhere you can remember, such as on your Desktop. **Do not** save them into any folder that says "OneDrive", you will not be able to access this folder once you're in Safe Mode!

##### Note for laptop users

If you have a laptop and have an iGPU and a dGPU, grab the driver for your dGPU (your dedicated GPU, not the one included in your CPU). If you do not have a dedicated GPU, then grab the one for your iGPU (same manufacturer as your CPU above).
For example: If your laptop has an Nvidia GPU, you grab the Nvidia  driver. If your laptop has an AMD GPU, you grab the AMD driver.
If your laptop only has a CPU but not a dedicated GPU, then you grab the driver that is the one from your manufacturer of the CPU (so if you have an Intel CPU, you grab the Intel driver, and vice versa)

### 3. Undo all overclocks/undervolts

Even if you don't think it's causing the issue (since it worked for a long time), undo it!
If you don't know what overclocking is, you can [skip to the next section](https://github.com/CommandMC/24HS-Wiki/blob/main/ddu.md#4-temporarily-disable-windows-updates)

##### Common questions

1. Q: I bought my GPU used so I don’t know if the previous owner overclocked  
  A: Overclocks don’t get applied at the GPU, but at the operating system. For example if you right now overclock your GPU, but then move the GPU over to another PC, it will not run overclocked on that other PC.
2. Q: I didn’t overclock but I see my CPU/GPU running at a higher speed?  
  A: This is called a boost clock, it’s not an overclock, it’s simply the CPU/GPU pushing itself when it can. It does not cause stability issues and won’t affect doing DDU.
3. Q: I overclocked/undervolted, how do I undo it?  
  A: This overclock is usually done through software like MSI afterburner or EVGA Precision. Both these softwares have a reset to default button, MSI Afterburner depending on the theme is either a circular refresh icon in the middle or a button saying default. In EVGA precision it's a button called default in the bottom. If you're unsure of this you can just uninstall the software.
  For the CPU or RAM, reset bios to default and/or Ryzen master if you did such overclock/undervolt/whatever, you want this running at stock. XMP is acceptable.

### 4. Temporarily disable Windows updates

To prevent issues relating to Windows updates pushing an older driver after you do DDU, you should **temporarily** disable Windows updates while doing this.

1. Open up the Settings (<kbd>Win + I</kbd>)
2. Click on "Update and Security" (last option)
3. Select the "Pause updates for 7 days" option ([Image](https://i.imgur.com/bbXdHv3.png))

### 5. Download DDU

1. Download DDU from [here](https://ftp.nluug.nl/pub/games/PC/guru3d/ddu/[Guru3D.com]-DDU.zip)
2. Extract the archive and move its contents to the same place you moved the GPU driver to
3. Double-click the "DDU v18.0.4.3.exe" file and click "Extract"

## Entering safe mode

1. Open Windows Search, search for "System Configuration"
2. Open "System Configuration"
3. Go to the "Boot" tab ([Image](https://i.imgur.com/5ywhrp5.png))
4. Tick the "Safe boot" box in the "Boot options" section ([Image](https://i.imgur.com/EpUaHjP.png))
5. Select "OK" at the bottom
6. System Configuration will ask if you want to restart. **Open these instructions on any device other than the one you're doing them on** (this can be your phone, a laptop, another PC)
7. Click "Restart"

## Inside Safe Mode

### Logging in
Once booted in, you will be presented with your normal login screen. If you created a new account earlier, login with this new account. Otherwise, login with your regular account

### Getting to your files
If you did not log in with your main user, your files will not be in their usual places. To get to them, follow these steps:
1. Open up Explorer (<kbd>Win + E</kbd>)
2. Click on "Local Disk (C:)" ([Image](https://i.imgur.com/jKSTvIS.png))
3. Go into the "Users" folder ([Image](https://i.imgur.com/QjPm5db.png))
4. Go into the folder of your primary user account
5. Your files will be there

### Uninstalling your GPU drivers
1. Navigate to the folder where you put DDU
2. Double-click "Display Driver Uninstaller.exe"
3. Dismiss the disclaimer
4. Close the "Options" window that will open by default. Do not change any settings in this window!
5. In the right panel, select "GPU" in the 1st dropdown, and your GPU manufacturer in the 2nd
6. Select "Clean and restart" on the left and be patient. Your screen may flicker during the uninstallation, this is normal. Be patient, your computer will eventually restart on its own.

### Getting out of safe mode
1. Login with either your main or backup user
2. Open Windows Search, search for "System Configuration"
3. Open "System Configuration"
4. Go to the "Boot" tab ([Image](https://i.imgur.com/5ywhrp5.png))
5. Untick the "Safe boot" box in the "Boot options" section ([Image](https://i.imgur.com/EpUaHjP.png))
6. System Configuration will ask if you want to restart. Click "Restart"

## Back to normal

### Installing GPU drivers
1. Login with your main user (if you can't login with your main user, you did not exit safe mode correctly. Follow [this part]() again)
2. Navigate to the folder where you put your GPU drivers and launch the installer
3. Follow the instructions on screen.
4. **NVIDIA only**: If you get an error saying "Other installations are running", wait for a few minutes, then restart your PC and try again.
5. If you're prompted to restart, do so. If not, still restart your PC manually.

### Enabling Windows Updates again
1. Open up the Settings (<kbd>Win + I</kbd>)
2. Click on "Update and Security" (last option)
3. Click the "Resume updates" button ([Image](https://i.imgur.com/ovLZtxd.png))

## You're done!
Well, almost.

Because you clean-installed your drivers, your monitor settings have very likely been returned to their defaults. Please check these settings (like Resolution or Refresh Rate) and set them to your desired values
</details>
