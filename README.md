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
