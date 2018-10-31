![Ansible Logo](img/ansible_logo.png)


A Robust Automation System

---
## About the Presentation
* Overview of Ansible
* Review of [Ansible Best Practices](https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html#content-organization)
* Helpful Tips and Tricks

---
## About Me

---
## What is Ansible?

* Configuration Management System
* Deployment Tool
* Network Automation System
* Cloud Configuration System

Note:

Ansible is a fantastic tool that can do just about anything, but that doesn't mean it should be used for everything...

---
## Folder Structure

```text
├── host_vars/
|   ├── host_name/
|   |   └── variables.yml
|   └── host_name.yml
├── group_vars/
|   ├── group_name/
|   |   └── variables.yml
|   └── group_name.yml
├── inventory/
|   ├── dynamic_inventory.py
|   └── static_inventory.yml
├── site.yml
├── webservers.yml
└── roles/
    ├── common/
    |   ├── defaults/
    |   │   └── main.yml
    |   ├── files/
    |   │   └── foo.txt
    |   ├── handlers/
    |   │   └── main.yml
    |   ├── meta/
    |   │   └── main.yml
    |   ├── tasks/
    |   │   └── main.yml
    |   ├── templates/
    |   │   └── ntp.conf.j2
    |   └── vars/
    |       └── main.yml
    └── webserver/
        └── ...
```
@[12-13](Top level playbooks are your starting point!)
@[1-8](Host and Group variables can be both files and directories.)
@[9-11](Inventories can be both static and dynamic.)
@[14-29](Roles follow a standard directory structure.)

Note:

There are more directories and conventions that Ansible supports, but those are beyond the scope of this presentaiton.
