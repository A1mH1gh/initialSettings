# initialSettings
Preferences for vsCode with Cmder, burpSuite, proxy, etc.

# vscode with cmder
```
// vscode > 설정 > settings.json
{
    "workbench.colorTheme": "Default Light Modern",
    "terminal.integrated.profiles.windows": {
        "Cmder": {
            "path": "${env:windir}\\System32\\cmd.exe",
            "args": [
                "/k",
                "C:\\cmder\\vendor\\bin\\vscode_init.cmd"
            ]
        }
    },
    "terminal.integrated.defaultProfile.windows": "Cmder"
}
```
# 시스템 환경 변수
```
//아나콘다
C:\ProgramData\anaconda3\Scripts\
```
