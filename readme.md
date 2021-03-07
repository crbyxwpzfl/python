# personal portable python 3.9.1 
#### setup 
add __%DESKTOP%\path\to\python-folder__ to PATH enviornment variable<br>

## see yt-dl
```batch
@echo off

:listen https://youtube.com/playlist?list=PLaHzPX64jQ19wU2ckGEefoUlYCNvnjkv7
:see https://youtube.com/playlist?list=PLaHzPX64jQ189iqTEvaWmvK0l1-Dt3ssP

:cd into location of archive.txt since absolut path does not work since python escapes \ as \\ and path c:\\Users does not exsist

cd c:\Users\roess\Desktop\files\shows\see

set out="c:\Users\roess\Desktop\files\shows\see\%%(title)s.%%(ext)s"
set url="https://youtube.com/playlist?list=PLaHzPX64jQ189iqTEvaWmvK0l1-Dt3ssP"

youtube-dl --restrict-filenames -o %out% %url% --download-archive archive.txt"

:timeout /t 120 /nobreak 
```
## listen yt-dl
```batch
@echo off

:listen https://youtube.com/playlist?list=PLaHzPX64jQ19wU2ckGEefoUlYCNvnjkv7
:see https://youtube.com/playlist?list=PLaHzPX64jQ189iqTEvaWmvK0l1-Dt3ssP

:cd into location of archive.txt since absolut path does not work since python escapes \ as \\ and path c:\\Users does not exsist

cd c:\Users\roess\Desktop\files\listen

set out="c:\Users\roess\Desktop\files\listen\%%(title)s.%%(ext)s"
set url="https://youtube.com/playlist?list=PLaHzPX64jQ19wU2ckGEefoUlYCNvnjkv7"

youtube-dl -x --audio-format mp3 --restrict-filenames -o %out% %url% --download-archive archive.txt"

:timeout /t 120 /nobreak 

```

# [python embeddable from](https://www.python.org/downloads/windows/)
# [yt-dl from](https://github.com/ytdl-org/youtube-dl)

