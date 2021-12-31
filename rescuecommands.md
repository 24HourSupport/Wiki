# 24 Hour Support Wiki

## Rescue commands

There are three different ways to run rescuecommands, this first one is the one that works in 99.99% of scenarios, only follow what is afterwards if it doesn't work.

1. Download the [24HS-Automator](https://github.com/24HourSupport/Automator/releases/latest/download/24HS-Automator.exe). (You click the text in blue in this line, it's a hyperlink, which will download what you need for you)
2. Once the Automator is downloaded from the above link, open it. 
3. Click the 1st button ("SFC / DISM / CHKDSK scans").
4. Using the 3 buttons, run through the SFC and DISM scans. If we told you to run CHKDSK, then press the CHKDSK button. If we did not tell you to run CHKDSK (or we did not mention it at all) then you just run SFC and DISM. 
5. You can run SFC, then DISM, then SFC again just to be safe. 
6. Restart/reboot the PC (This should happen automatically if you're running a CHKDSK scan).
7. That is it, you don't have to do anything else, successfully finished. See if the issue you were having happens again, if it does then tell us this.


Click the ➜ Arrow next to "I Cannot use the Automator" only if something stopped you from following the above steps. Always follow the above steps first, below ones are a backup.


<details>
<summary>I Cannot use the Automator</summary>
<br>

### I can use my computer and login to Windows, but cannot use the internet. Or I do not want to use the Automator.

Follow this sub-section if you can login to Windows and use your computer, but either do not have internet access or do not want to use the Automator.

1. Press the Windows key + R to open the "Run" dialog
2. Type in "cmd" and press <kbd>Ctrl + Shift + Enter</kbd>
3. Type in `sfc /scannow` and wait for the command to finish
4. Type in `dism /Online /Cleanup-Image /RestoreHealth` and wait for the command to finish
5. If you are instructed to do a `chkdsk` scan, also type in `chkdsk C: /r /x` and press <kbd>Y</kbd> when asked if you want to check the volume the next time the system restarts
6. Restart your computer. If you entered the `chkdsk` command previously, you will see a message on bootup. **Do not skip this check**
7. That is it, you don't have to do anything else, successfully finished. See if the issue you were having happens again, if it does then tell us this.


### If you can't boot up your computer
1. Obtain a Windows Installation Medium and boot from it
2. (Optionally) set your keyboard layout
3. Click "Next", then "Repair your computer" at the bottom-left
4. Click "Troubleshoot" -> "Command Prompt"
5. Type in `bcdedit | find "partition" | more +2`. You should see a <samp>C:</samp>/<samp>D:</samp>/etc at the end  
  Note: The following commands will assume that this command said "C:" at the end. If it did not do this for you, please adapt them accordingly
7. Type in `sfc /scannow /offbootdir=C:\ /offwindir=C:\Windows` and wait for it to finish
8. Type in `dism /Image:C: /Cleanup-Image /RestoreHealth` and wait for it to finish
9. If you are instructed to do a `chkdsk` scan, also type in `chkdsk C: /r /x`.
10. Restart/reboot by closing the CMD window and choosing the "Turn off your PC" option
11. That is it, you don't have to do anything else, successfully finished. See if the issue you were having happens again, if it does then tell us this.
</details>
