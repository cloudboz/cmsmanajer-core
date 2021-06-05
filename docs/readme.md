# Business Flow

## Requirements
- Your server must be Ubuntu 18.04 or 20.04 (64-bit). 
- Only clean servers (no Nginx, Apache, or MySQL installed) can be connected to CMS Manajer.
- Installed python2.7 or python3.
- Minimum of RAM 256MB

## How to Use
- Connect server use `ansible-playbook cman-optimiz.yml`

- Install lamp use `ansible-playbook cman-aemp.yml --tags "apache"`
- Install lemp use `ansible-playbook cman-aemp.yml --tags "nginx"`
- Install wp apache use `ansible-playbook cman-wordpress.yml --tags "apache"`
- Install wp nginx use `ansible-playbook cman-wordpress.yml --tags "nginx"`

- Create app apache use `ansible-playbook cman-aemp.yml --tags "create-app-apache"`
- Create app nginx use `ansible-playbook cman-aemp.yml --tags "create-app-nginx"`
- Create app wp apache use `ansible-playbook cman-wordpress.yml --tags "create-app-wp-apache"`
- Create app wp nginx use `ansible-playbook cman-wordpress.yml --tags "create-app-wp-nginx"`