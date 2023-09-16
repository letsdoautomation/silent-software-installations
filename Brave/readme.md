# Documentation and download
Download link: [Brave](https://github.com/brave/brave-browser) <br />
Download link(I do not recommend): [brave_installer-x64.exe](https://brave-browser-downloads.s3.brave.com/latest/brave_installer-x64.exe) <br />
Documentation link:  N/A

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
### WiX commands
```powershell
wix build Brave.wxs
```
# Related videos <br />
###  PSEXEC
[Windows tools: Using PSEXEC for software deployment testing](https://youtu.be/9ywdTna_TLc) <br />
### WiX Toolset 4 CLI <br />
[Windows Tools: Download and install .NET 7 SDK and WiXtoolset 4 CLI tool](https://youtu.be/ukrIlmadTjw) <br />
[Group Policy: Packaging EXE into MSI for Group Policy software deployment using WiX toolset CLI](https://youtu.be/pZ42XS2Ucsg) <br />