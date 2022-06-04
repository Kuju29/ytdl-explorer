### Supported formats:
![Screenshot](https://user-images.githubusercontent.com/22098092/171465797-133f3577-ab21-4027-acd9-19bf5593eb66.png)

### How to use it
1. [Download the ZIP archive of this repository](https://github.com/Kuju29/ytdl-explorer/archive/refs/heads/main.zip)
2. Unpack the archive
3. Double-click on the yt-dlp.reg and ffmpeg.reg file and confirm adding the keys to the registry
4. Copy the video link, go to the folder where you want to download it
5. Right click on the empty space and choose your option
6. Voilà!

### This script requires | **yt-dlp** | **ffmpeg** | **XstreamDL-CLI** |
Open a PowerShell as Administrator and run:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
Install **yt-dlp** and **ffmpeg**:
```
choco install yt-dlp ffmpeg
```
Install **XstreamDL-CLI**:
- [Install python](https://www.python.org/)
- <kbd> Download: [XstreamDL-CLI-master.zip](https://github.com/xhlove/XstreamDL-CLI/archive/refs/heads/master.zip) </kbd>
- <kbd> Donwload: [binaries.7z](https://github.com/xhlove/XstreamDL-CLI/releases/download/1.3.1/binaries.7z) </kbd>
> 1. Unzip the file `XstreamDL-CLI-master.zip` and `binaries.7z`
> 2. Copy file from binaries folder `(ffmpeg.exe, mp4box.exe, mp4decrypt.exe)` to `.\XstreamDL-CLI-master\binaries`
> 3. Open cmd in `.\XstreamDL-CLI-master` [example](https://user-images.githubusercontent.com/22098092/171996089-b214f918-c041-4c82-b7d3-c7a161f55f5b.png)
> 4. `pip install -r requirements.txt`

### Uninstalling ytdl-explorer
To uninstall the script, Double-click on the uninstall.reg file and confirm the changes. \
Or delete file from **regedit**
```
- Computer\HKEY_CLASSES_ROOT\*\shell\ffmpeg
```
```
- Computer\HKEY_CLASSES_ROOT\Directory\Background\shell\Ytdlp
```
