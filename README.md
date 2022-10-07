# Ansible Playbook: mdatp_onboard
![GitHub last commit](https://img.shields.io/github/last-commit/lpwoodhouse/mdatp_onboard)
![GitHub repo file count](https://img.shields.io/github/directory-file-count/lpwoodhouse/mdatp_onboard)
![GitHub top language](https://img.shields.io/github/languages/top/lpwoodhouse/mdatp_onboard)

## Purpose

Onboards a Linux client distro (Redhat, Ubuntu and Suse families) to Microsoft Defender Advanced Threat Detection

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see ```defaults/main.yml```)
```shell
# Important to provide a path to your onboard json file which will be copied to the hosts during role execution.
# sample_mdatp_onboard.json is provided as a sample only and will not work.
json_path: "files/sample_mdatp_onboard.json"
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: all
      vars:
        - json_path: "files/mdatp_onboard.json"
      roles:
        - mdatp_onboard
```

## License

[![GitHub](https://img.shields.io/github/license/lpwoodhouse/mdatp_onboard)](LICENSE)

## Author Information

This playbook was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
