# ansible-debian-infra

Infrastructure automation lab using **Ansible** to configure two **Debian 13** virtual machines managed by **Libvirt**.

## 🧱 Project structure

ansible-debian-infra/
├── ansible.cfg
├── inventory/
│ └── hosts.ini
├── playbooks/
│ └── site.yml
└── roles/
├── nginx/
└── database/

## ⚙️ Roles

- **nginx** → Configures a web server  
- **database** → Installs and runs MariaDB

## 🚀 Usage

1. Clone the repository  
   ```bash
   git clone https://github.com/moonyr/ansible-debian-infra.git
   cd ansible-debian-infra```
   
2. Update your inventory (inventory/hosts.ini) with your VM IPs.

3. Run the playbook:
   
   ```bash
   ansible-playbook -i inventory/hosts.ini playbooks/site.yml
   ```

