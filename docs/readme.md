# Business Flow

# Requirements
- Your server must be Ubuntu 18.04 or 20.04 (64-bit). 
- Only clean servers (no Nginx, Apache, or MySQL installed) can be connected to CMS Manajer.
- Installed python2.7 or python3.
- Minimum of RAM 256MB

# How to Use
## Connect server
```
ansible-playbook cman.yml --tags "connect-server"
```
## Create system user
```
ansible-playbook cman.yml --tags "create-system-user"
```
## LAMP
```
ansible-playbook cman.yml --tags "lamp-full-install"
ansible-playbook cman.yml --tags "lamp-full-uninstall"

ansible-playbook cman.yml --tags "lamp-create-single-app"
ansible-playbook cman.yml --tags "lamp-delete-single-app" # This command also support for delete WordPress single app (Apache)
```
## LEMP
```
ansible-playbook cman.yml --tags "lemp-full-install"
ansible-playbook cman.yml --tags "lemp-full-uninstall"

ansible-playbook cman.yml --tags "lemp-create-single-app"
ansible-playbook cman.yml --tags "lemp-delete-single-app" # This command also support for delete WordPress single app (Nginx)
```
## MySQL
```
ansible-playbook cman.yml --tags "mysql-install"
ansible-playbook cman.yml --tags "mysql-uninstall"
ansible-playbook cman.yml --tags "mysql-create-single-db"
ansible-playbook cman.yml --tags "mysql-delete-single-db"
```
## WordPress (Apache)
```
ansible-playbook cman.yml --tags "wp-lamp-full-install"
ansible-playbook cman.yml --tags "wp-lamp-full-uninstall"

ansible-playbook cman.yml --tags "wp-lamp-create-single-app"
```
## WordPress (Nginx)
```
ansible-playbook cman.yml --tags "wp-lemp-full-install"
ansible-playbook cman.yml --tags "wp-lemp-full-uninstall"

ansible-playbook cman.yml --tags "wp-lemp-create-single-app"
```
## Docker
```
ansible-playbook cman.yml --tags "docker-install"
ansible-playbook cman.yml --tags "docker-uninstall"
```
## MongoDB
```
ansible-playbook cman.yml --tags "mongodb-install"
ansible-playbook cman.yml --tags "mongodb-uninstall"
```
## Nginx
```
ansible-playbook cman.yml --tags "nginx-install"
ansible-playbook cman.yml --tags "nginx-uninstall"
```
## Apache
```
ansible-playbook cman.yml --tags "apache-install"
ansible-playbook cman.yml --tags "apache-uninstall"
```