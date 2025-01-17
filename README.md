### Supported formats:
![Screenshot](https://user-images.githubusercontent.com/22098092/171465797-133f3577-ab21-4027-acd9-19bf5593eb66.png)

### How to use it
1. [Download the ZIP archive of this repository](https://github.com/Kuju29/ytdl-explorer/archive/refs/heads/main.zip)
2. Unpack the archive
3. Double-click on the yt-dlp.reg and ffmpeg.reg file and confirm adding the keys to the registry
4. Copy the video link, go to the folder where you want to download it
5. Right click on the empty space and choose your option
6. Voilà!

### This script requires | **yt-dlp** | **ffmpeg** | **XstreamDL-CLI & N_m3u8DL-CLI** |
Open a PowerShell as Administrator and run:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
Install **yt-dlp** and **ffmpeg**:
```
choco install yt-dlp ffmpeg
```
Install **XstreamDL-CLI & N_m3u8DL-CLI**:
- <kbd> Download: [N_m3u8DL-CLI.exe](https://github.com/nilaoda/N_m3u8DL-CLI/releases) </kbd>
- <kbd> Donwload: [XstreamDL-CLI.exe](https://github.com/xhlove/XstreamDL-CLI/releases) </kbd>
> 1. Rename file to `N_m3u8DL-CLI.exe` and `XstreamDL-CLI.exe`
> 2. Copy file to new folder `C:\m3u8DL-CLI`

### Update
```
choco upgrade all -y
```

##### _note: if there is an update. You have to change the name here again._

### Uninstalling ytdl-explorer
To uninstall the script, Double-click on the uninstall.reg file and confirm the changes. \
Or delete file from **regedit**
```
- Computer\HKEY_CLASSES_ROOT\*\shell\ffmpeg
```
```
- Computer\HKEY_CLASSES_ROOT\Directory\Background\shell\Ytdlp
```
