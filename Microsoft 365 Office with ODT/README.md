# Silent software installation: Microsoft 365 Office with ODT

<b>Downloads</b>

* [Office Deployment Tool](https://www.microsoft.com/en-us/download/details.aspx?id=49117)

<b>Documentation:</b>

* [Overview of the Office Deployment Tool](https://learn.microsoft.com/en-us/deployoffice/overview-office-deployment-tool)
* [Configuration options for the Office Deployment Tool](https://learn.microsoft.com/en-us/deployoffice/office-deployment-tool-configuration-options)
* [List of Product IDs that are supported by the Office Deployment Tool for Click-to-Run](https://learn.microsoft.com/en-us/microsoft-365/troubleshoot/installation/product-ids-supported-office-deployment-click-to-run)

<b>Tools:</b>

* [Office Customization Tool](https://config.office.com/deploymentsettings)

<b>Objectives:</b>

* Perform online ms365 installation
* Perform offline ms365 installation


### Online installation

<b>Perform online installation:</b>

```powershell
setup.exe /configure configuration-online.xml
```

### Offline installation

<b>Download installation files:</b>

```powershell
setup.exe /download configuration-offline.xml
```

<b>Perform offline installation:</b>

```powershell
setup.exe /configure configuration-offline.xml
```
