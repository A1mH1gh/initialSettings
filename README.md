# initialSettings
Preferences for vsCode with Cmder, burpSuite, proxy, etc.

# vscode with cmder
```settings
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
