# initialSettings
Preferences for vsCode with Cmder, burpSuite, proxy, etc.

# vscode
```
// vscode > 설정(톱니바퀴) > settings.json
{
    "workbench.colorTheme": "Visual Studio 2017 Light - C++",
    "workbench.activityBar.location": "hidden",
    "terminal.integrated.profiles.windows": {
        "Cmder": {
            "path": "${env:windir}\\System32\\cmd.exe",
            "args": [
                "/k",
                "C:\\cmder\\vendor\\bin\\vscode_init.cmd"
            ]
        }
    },
    "terminal.integrated.defaultProfile.windows": "Cmder",
    "git.ignoreMissingGitWarning": true,
    "workbench.statusBar.visible": false
}

// vscode > 설정 > keybindings.json (Beautify 설치된 상태)
[
    {
        "key": "alt+shift+f",
        "command": "HookyQR.beautify",
        "when": "editorFocus"
    }
]
```
# Anaconda
```
C:\ProgramData\anaconda3\Scripts\activate.bat
conda create --name py37 python==3.7
```
# Frida
```
pip install frida==14.2.13
pip install frida-tools==9.2.1
```
# Docker
```
CMD(관리자)> dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
CMD(관리자)> dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
Microsoft Store에서 Ubuntu 설치하기
https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi
wsl -l -v
https://docs.docker.com/desktop/install/windows-install/
```

# Proxy Bypass List
```
127.0.0.1
::1
localhost
*google*
*naver*
*chatgpt.com*
*ucloud.lguplus.co.kr*
*github*
*bing.com
*momentumdash.com
*posthog.com
*gvt2.com*
*jwt.io*
*notion*
*cdn.oaistatic.com*
*facebook*
*gstatic.com
browser-intake-datadoghq.com
l.clarity.ms
*sharepoint*
*microsoftonline*
```

# .png, css, gif, woff2, woff를 제외하는 정규식은?
```
🔍 1. 브라우저 개발자 도구 (Network 탭)에서 사용하기
Network 탭을 열고 Filter 입력란에 아래 정규식을 입력합니다.

ruby
코드 복사
/^((?!\.(png|css|gif|woff2?|ico|svg|jpg|woff)$).)*$/
Enter를 누르면, .png, .css, .gif, .woff2, .woff 확장자를 제외한 요청들만 표시됩니다.
```
