# Silent software installations: Microsoft Office 2016

<b>Documentation</b>

* [Office Customization Tool (OCT) 2016 Help: Overview](https://learn.microsoft.com/en-us/deployoffice/oct/oct-2016-help-overview)<br />
* [Setup properties reference for Office 2013](https://learn.microsoft.com/en-us/previous-versions/office/office-2013-resource-kit/cc179018(v=office.15))

<b>Objectives</b>

* Create MSP customization file
* Use MSP customization file to silently install Office 2016

<b>Open Microsoft Office Customization Tool:</b>

```batch
setup.exe /admin
```

<b>Configure properties:</b>

* Name: SETUP_REBOOT
    * Value: Never
* Name: HIDEUPDATEUI
    * Value: True

<b>Perform silent installation:</b>

```batch
setup.exe /adminfile configuration.MSP
```