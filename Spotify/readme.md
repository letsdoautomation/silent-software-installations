# Downloads and documentation
<b>Download links:</b> <br /> 
* [Spotify](https://www.spotify.com/de-en/download/windows/) <br />
* [Spotify Offline Installer](https://download.scdn.co/SpotifyFullSetup.exe)


### Silent install commands
```powershell
cmd /c SpotifySetup.exe /silent
```
### Registry commands
```powershell
ni "HKLM:\SOFTWARE\Microsoft\Active Setup\Installed Components\InstallSpotify" | New-ItemProperty -Name "StubPath" -Value 'REG ADD "HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce" /v InstallSpotify /t REG_SZ /d "C:\SpotifyFullSetup.exe /silent"'
```

# Related videos
###  PSEXEC
[Windows tools: Using PSEXEC for software deployment testing](https://youtu.be/9ywdTna_TLc) <br />
### Windows registry
[Windows Registry: Run and RunOnce](https://youtu.be/zgFzCq5uEPw) <br />
[Windows Registry: Active Setup](https://youtu.be/HrVJ7wdvfmo) <br />