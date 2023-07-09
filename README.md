# ansible-role-win-office365

Role to install Office365

## Table of content

- [Default Variables](#default-variables)
  - [office365_configuration_xml](#office365_configuration_xml)
  - [office365_extract_dir](#office365_extract_dir)
  - [office365_setup_download_url](#office365_setup_download_url)
  - [office365_update_cmd](#office365_update_cmd)
  - [office365_update_to_version](#office365_update_to_version)
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

### office365_extract_dir

extraction directory

#### Default value

```YAML
office365_extract_dir: C:\windows\temp\odt
```

### office365_setup_download_url

Office365 Setup download url

#### Default value

```YAML
office365_setup_download_url: https://officecdn.microsoft.com/pr/wsus/setup.exe
```

### office365_update_cmd

Office365 update command

#### Default value

```YAML
office365_update_cmd: '"{{ ansible_env.CommonProgramFiles }}\Microsoft Shared\ClickToRun\OfficeC2RClient.exe"
  /update user updatepromptuser=false forceappshutdown=true displaylevel=false'
```

### office365_update_to_version

Updates Office 365 to a specific version This adds updatetoversion parameter to the office365_update_cmd https://support.microsoft.com/en-us/topic/how-to-revert-to-an-earlier-version-of-office-2bd5c457-a917-d57e-35a1-f709e3dda841

#### Default value

```YAML
office365_update_to_version: ''
```

#### Example usage

```YAML
office365_update_to_version: "16.0.14527.20364"
```

## Discovered Tags

**_never_**

**_office365-update_**


## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888
