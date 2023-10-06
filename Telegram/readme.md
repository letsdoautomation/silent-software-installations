# Downloads and documentation
<b>Download links:</b> <br /> 
* [Telegram](https://desktop.telegram.org/) <br />

### Software installation flow using Active Setup and RunOnce:
```mermaid
flowchart TD
    a["User signs-in to the computer"] --> b["Active Setup creates RunOnce registry entry"]
    b --> c[Users Desktop loads]
    c --> d["RunOnce will start software installation"]
```

### Registry commands
```powershell
ni "HKLM:\SOFTWARE\Microsoft\Active Setup\Installed Components\InstallTelegram" | New-ItemProperty -Name "StubPath" -Value 'REG ADD "HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce" /v InstallTelegram /t REG_SZ /d "C:\tsetup-x64.4.10.2.exe /VERYSILENT /NORESTART"'
```

# Related videos
### Windows registry
[Windows Registry: Run and RunOnce](https://youtu.be/zgFzCq5uEPw) <br />
[Windows Registry: Active Setup](https://youtu.be/HrVJ7wdvfmo) <br />
### Creating MSI file
[WiX toolset 4 CLI:Create Telegram MSI installation file](https://youtu.be/wDiuEd88Ovc)