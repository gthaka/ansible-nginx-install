# Simple Ansible Project

This is an Ansible project that automates the setup and configuration of servers. In this case, installation and starting of Nginx

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

What things you need to install the software and how to install them
- Ansible (You can install it with `pip install ansible`)
- Python (Ansible is written in Python, so you need Python installed on your machine. You can download it from [here](https://www.python.org/downloads/))

### Installation

1. Clone the repository
    ```bash
    git clone https://github.com/gthaka/ansible-nginx-install.git
    ```
2. Navigate to the directory
    ```bash
    cd ansible-nginx-install
    ```
3. Update `inventory` file with your server ips. In this case, we have server groups `ubuntu_servers` and `alpine_servers`
4. Run the Ansible Playbook
    ```bash
    ansible-playbook -i inventory first-playbook.yml -kK
    ```

    `-kK` option specifies promp for password for ssh and user

### For more info on ansible, [read the docs here!](https://docs.ansible.com/ansible/latest/)