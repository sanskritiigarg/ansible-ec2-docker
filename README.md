# Ansible AWS Project: Provision EC2, Install Docker, Deploy Nginx with Custom Landing Page

This project automates end-to-end setup of a web server on AWS using Ansible. It:
- Provisions a new EC2 instance.
- Installs Docker on it.
- Runs an Nginx container serving a custom HTML landing page.

---
## Project Structure
 ```
ansible_project/
├── ansible.cfg
├── inventory.ini
├── playbook.yml
└── nginx/
    ├── files/
    │   └── index.html
    └── tasks/
        └── main.yml
```
---

## Requirements

- Ansible installed (>= 2.10).
- AWS account with:
  - Access key & secret key configured via AWS CLI or environment variables.
  - Existing VPC, subnet, and security group allowing ports 22 (SSH) & 80 (HTTP).
  - Existing AWS key pair (.pem) for SSH access.
