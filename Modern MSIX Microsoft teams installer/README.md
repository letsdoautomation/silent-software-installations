# Silent software installation: Modern MSIX Microsoft Teams installer

<b>Download:</b>

[Deploy the new Microsoft Teams client](https://learn.microsoft.com/en-us/microsoftteams/new-teams-vdi-requirements-deploy#deploy-the-new-microsoft-teams-client)

<b>Install using Add-AppProvisionedPackage:</b>

```powershell
Add-AppProvisionedPackage -Online -PackagePath .\MSTeams-x64.msix -SkipLicense
```

<b>Install using DISM:</b>

```powershell
DISM /Online /Add-ProvisionedAppxPackage /PackagePath:"D:\Downloads\MSTeams-x64.msix" /SkipLicense
```

## Related videos

<b>Windows tools:</b>

[Windows tools: Using PSEXEC for software deployment testing](https://youtu.be/9ywdTna_TLc) <br />