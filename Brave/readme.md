<b>Download links:</b> <br /> 
* [Brave](https://github.com/brave/brave-browser) <br />
* [brave_installer-x64.exe (I do not recommend)](https://brave-browser-downloads.s3.brave.com/latest/brave_installer-x64.exe) <br />

### Silent install commands
```powershell
cmd /c BraveBrowserSetup.exe /silent /install
```
```powershell
cmd /c BraveBrowserStandaloneSetup.exe /silent /install
```
```powershell
cmd /c brave_installer-x64.exe /install /silent /system-level
```
### Registry commands
```powershell
ni "HKLM:\SOFTWARE\Microsoft\Active Setup\Installed Components\InstallBrave" | New-ItemProperty -Name "StubPath" -Value 'REG ADD "HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce" /v InstallBrave /t REG_SZ /d "C:\BraveBrowserStandaloneSilentSetup.exe"'
```

# Related videos
### PSEXEC
[Windows tools: Using PSEXEC for software deployment testing](https://youtu.be/9ywdTna_TLc) <br />
### Windows registry
[Windows Registry: Run and RunOnce](https://youtu.be/zgFzCq5uEPw) <br />
[Windows Registry: Active Setup](https://youtu.be/HrVJ7wdvfmo) <br />