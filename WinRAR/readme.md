# Documentation and download
Download link: [WinRAR](https://www.win-rar.com/download.html?&L=0) <br />
Documentation link: N/A <br />

### Install command
```powershell
# Make sure that executable name is correct
cmd /c winrar-x64-624.exe /S
```

```powershell
ni "HKLM:\SOFTWARE\Microsoft\Active Setup\Installed Components\runWinRAR" | New-ItemProperty -Name "StubPath" -Value ('REG ADD "HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce" /v runWinRAR /t REG_SZ /d "{0}\WinRAR\WinRAR.exe"' -f $env:ProgramFiles)
```

<b>Both commands in 1</b>
```batch
cmd /c winrar-x64-701.exe /S && powershell.exe New-ItemProperty -Path (ni 'HKLM:\SOFTWARE\Microsoft\Active Setup\Installed Components\runWinRAR').PSPath -Name StubPath -Value ('REG ADD \"HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce\" /v runWinRAR /t REG_SZ /d \"%ProgramFiles%\WinRAR\WinRAR.exe\"')
```

# Related videos
###  PSEXEC
[Windows tools: Using PSEXEC for software deployment testing](https://youtu.be/9ywdTna_TLc) <br />
### Windows registry
[Windows Registry: Run and RunOnce](https://youtu.be/zgFzCq5uEPw) <br />
[Windows Registry: Active Setup](https://youtu.be/HrVJ7wdvfmo) <br />
