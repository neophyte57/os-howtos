# Base64 encoding/decoding

Possible with built-in CLI utility called `certutil`


# Escape from RDP session

To escape from a full-screen RDP session, press `CTRL+ALT+HOME` and then `ALT+TAB`.  For more RDP-related shortcut keys, see [Remote Desktop Services Shortcut Keys](https://docs.microsoft.com/en-us/windows/win32/termserv/terminal-services-shortcut-keys)


# Extracting from CD

Use Windows Media Player:
![Extracting from CD](windows/windows-media-player.png)


# Kill process on command-line

For example, killing Nginx:  `taskkill /IM nginx.exe /F`

For more information:  https://stackoverflow.com/questions/39632667/how-do-i-kill-the-process-currently-using-a-port-on-localhost-in-windows


# Kill process occupying a certain port
First find process ID, e.g. of process running on port 4200:  `netstat -a -n -o | findstr 4200`.
Then kill process by the process ID, e.g. `taskkill -f /pid 29296`

For more information:  https://stackoverflow.com/questions/39091735/port-4200-is-already-in-use-when-running-the-ng-serve-command



# Removing old version of Windows 10 safely

https://support.microsoft.com/en-us/windows/delete-your-previous-version-of-windows-f8b26680-e083-c710-b757-7567d69dbb74


# `which`-equivalent

Similar to the `which` UNIX command, `where` is available as early as Windows XP.  You can use it in the `Command Prompt` but not `PowerShell`:  [Microsoft Docs](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/cc753148(v=ws.11)?redirectedfrom=MSDN).  Reports location of executable that will be used according to PATH environment variable:

```
...>where java
C:\Windows\System32\java.exe 
```
