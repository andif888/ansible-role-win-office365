# ansible-role-win-office365

Role to install Office365

## Table of content

- [Default Variables](#default-variables)
  - [office365_configuration_xml](#office365_configuration_xml)
  - [office365_odt_download_url](#office365_odt_download_url)
  - [office365_odt_extract_dir](#office365_odt_extract_dir)
  - [office365_update_cmd](#office365_update_cmd)
  - [office_365_update_cmd](#office_365_update_cmd)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### office365_configuration_xml

Office365 configuration.xml file

#### Default value

```YAML
office365_configuration_xml: files/configuration.xml
```

### office365_odt_download_url

Office365 Deployment Tool download url

#### Default value

```YAML
office365_odt_download_url: https://download.microsoft.com/download/2/7/A/27AF1BE6-DD20-4CB4-B154-EBAB8A7D4A7E/officedeploymenttool_16130-20218.exe
```

### office365_odt_extract_dir

extraction directory

#### Default value

```YAML
office365_odt_extract_dir: C:\windows\temp\odt
```

### office365_update_cmd

#### Default value

```YAML
office365_update_cmd: '"{{ ansible_env.CommonProgramFiles }}\Microsoft Shared\ClickToRun\OfficeC2RClient.exe"
  /update user updatepromptuser=false forceappshutdown=true displaylevel=false'
```

### office_365_update_cmd

Office365 update command

## Discovered Tags

**_never_**

**_office365-update_**


## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888
