# RedHat Ansible Advanced Workshop
## Windows Integration Lab

The "Windows Integration Lab" of the workshop was designed to be executed using a Windows 2012R2.
These roles were modified to use also with a lower version.

# How to use
Clone the repository and change the values of these variables according your environment:

| File                                   | Variable                 |
|----------------------------------------|--------------------------|
| roles/win_ad_install/defaults/main.yml | ad_domain_name           |
| roles/win_ad_install/defaults/main.yml | ad_forestmode_domainmode |
| roles/win_ad_user/tasks/main.yml       | email                    |

# ToDo
  * Make the first block in *[roles/win_ad_install/tasks/main.yml](https://github.com/jcrelling/AnsibleAdvanceWindowsIntegrationLab/blob/dbf868b7ca9a695c702003f1c6e5d140e467dbbf/roles/win_ad_install/tasks/main.yml#L7-L17)* "idempotent" checking first if exist any AD
  * The PS script restart the server so we need to add a control step so it can wait the server back
  
# Author: Christian Relling
