Experitest - Cloud Emulator Host ansible role
=========

This role will install \ uninstall cloud ehm for mac os hosts

Requirements
------------

This role assumes that you have java 8 installed on the instance
Supports mac os hosts only.

Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| state | should the application be present or absent | present, absent | present | no |
| app_version | application version to install | string | 12.7.6702 | no |
| server_port | port number for the server | number | 8081 | no |
| extra_application_properties | additional props to be override in application.properties file | dict | {} | no |
| extra_xml_conf | extand xml configuration | dict | {} | no |
| extra_java_options | extand java options | array of strings | [] | no |
| installation_folder | the folder in which the applction will be installed | string | for mac: /Applications/Experitest/cloud-agent-version <br> for windows: C:\\Experitest\\cloud-agent-version  | no |
| jmx_port | port number for jmx inspection | number | 51235 | no |
| custom_download_url | custom url to download the installation from (zip format) | string |  | no |
| start_after_install | should application start after installation is completed | boolean | True | no |
| clear_temp_folder | remove temp folder after installation | boolean | False | no |
| clear_before_install | removing old installation before installing new version | boolean | False | no |

Example Playbook
----------------

#### [see working example](/example)
