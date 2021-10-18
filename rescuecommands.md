# 24 Hour Support Wiki

[Return to main wiki page](https://github.com/CommandMC/24HS-Wiki/blob/main/index.md)

### If you can boot up your computer and have internet access

1. Download the [24HS-Automator](https://github.com/CommandMC/24HS-Automator/releases/latest)
2. Run it and accept the UAC prompt.
3. Select the 1st option (<samp>(1) Check system files</samp>) by pressing <kbd>1</kbd> on your keyboard.
4. Once the `sfc` and `dism` checks are done, ask the person helping you if you should also run a `chkdsk` scan. Press either Y (for yes) or N (for no)
5. Your PC will restart. If you have selected a `chkdsk` scan, you will see a message on bootup. **Do not skip this check**

### If you can boot up your computer but have no internet access

1. Press the Windows key + R to open the "Run" dialog
2. Type in "cmd" and press <kbd>Ctrl + Shift + Enter</kbd>
3. Type in `sfc /scannow` and wait for the command to finish
4. Type in `dism /Online /Cleanup-Image /RestoreHealth` and wait for the command to finish
5. If you are instructed to do a `ckkdsk` scan, also type in `chkdsk C: /r /x` and press <kbd>Y</kbd> when asked if you want to check the volume the next time the system restarts
6. Restart your computer. If you entered the `chkdsk` command previously, you will see a message on bootup. **Do not skip this check**

### If you can't boot up your computer
1. Obtain a Windows Installation Medium and boot from it
2. (Optionally) set your keyboard layout
3. Click "Next", then "Repair your computer" at the bottom-left
4. Click "Troubleshoot" -> "Command Prompt"
5. Type in `bcdedit | find "partition" | more +2`. You should see a <samp>C:</samp>/<samp>D:</samp>/etc at the end  
  Note: The following commands will assume that this command said "C:" at the end. If it did not do this for you, please adapt them accordingly
7. Type in `sfc /scannow /offbootdir=C:\ /offwindir=C:\Windows` and wait for it to finish
8. Type in `dism /Image:C: /Cleanup-Image /RestoreHealth` and wait for it to finish
9. If you are instructed to do a `ckkdsk` scan, also type in `chkdsk C: /r /x`.
10. Restart by closing the CMD window and choosing the "Turn off your PC" option