---

# Ansible Demo Role – Simple Role

![Ansible](https://img.shields.io/badge/Ansible-Automation-red)
![Platform](https://img.shields.io/badge/platform-Linux-blue)
![License](https://img.shields.io/badge/license-BSD-green)
![Status](https://img.shields.io/badge/status-demo-lightgrey)
![Maintained](https://img.shields.io/badge/maintained-yes-brightgreen)

## Overview

This repository provides a **simple Ansible role designed for demonstration and learning purposes**.
It illustrates the standard **Ansible role structure**, making it suitable for DevOps engineers who want to understand how to build reusable infrastructure automation components.

The role can be used as a **starting template for developing production-ready Ansible roles** or as part of DevOps training and CI/CD demonstrations.

---

## Features

* Demonstrates **standard Ansible role structure**
* Easily reusable within playbooks
* Simple configuration and minimal dependencies
* Suitable for **DevOps training, demos, and testing**

---

## Requirements

Before using this role, ensure the following prerequisites are met:

* **Ansible 2.9 or later**
* Linux-based target hosts (Ubuntu/Debian recommended)
* SSH access to managed nodes
* Python installed on target machines

Install Ansible if needed:

```bash
pip install ansible
```

---

## Role Variables

Variables can be configured using standard Ansible variable locations:

* `defaults/main.yml`
* `vars/main.yml`
* `group_vars/`
* `host_vars/`

Example variable configuration:

```yaml
# defaults/main.yml

demo_message: "Hello from the Ansible Demo Role"
```

These variables can be overridden in playbooks or inventory files.

---

## Role Structure

```
roles/
└── simple-role/
    ├── tasks/
    │   └── main.yml
    ├── handlers/
    │   └── main.yml
    ├── defaults/
    │   └── main.yml
    ├── vars/
    │   └── main.yml
    ├── files/
    ├── templates/
    ├── meta/
    │   └── main.yml
    └── README.md
```

This follows the **recommended Ansible role directory structure**.

---

## Example Playbook

Example playbook using this role:

```yaml
---
- name: Run demo role
  hosts: servers
  become: true

  roles:
    - simple-role
```

Run the playbook:

```bash
ansible-playbook playbook.yml
```

---

## Usage

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/Ansible-role.git
```

2. Add the role to your Ansible roles directory.

3. Reference the role in your playbook.

---

## Use Cases

This role can be used for:

* Learning **Ansible role development**
* Demonstrating **infrastructure automation**
* Testing **CI/CD pipelines**
* DevOps workshops and training

---

## Contributing

Contributions are welcome.
If you find improvements or want to extend the role, please:

1. Fork the repository
2. Create a new branch
3. Submit a pull request

---

## License

BSD License

---

## Author

**Srinivasarao Galla**

Website
[https://www.sgalla.ie](https://www.sgalla.ie)

GitHub
[https://github.com](https://github.com/srinugalla)

---
