# Business Flow

## Requirements
- Your server must be Ubuntu 18.04 or 20.04 (64-bit). 
- Only clean servers (no Nginx, Apache, or MySQL installed) can be connected to CMS Manajer.
- Installed python2.7 or python3.
- Minimum of RAM 256MB

## How to Use
### Connect server
- Connect server use `ansible-playbook cman-optimiz.yml`

### Install app
- Install lamp use `ansible-playbook cman-aemp.yml --tags "apache"`
- Install lemp use `ansible-playbook cman-aemp.yml --tags "nginx"`
- Install wp apache use `ansible-playbook cman-wordpress.yml --tags "apache"`
- Install wp nginx use `ansible-playbook cman-wordpress.yml --tags "nginx"`

### Create app
- Create app apache use `ansible-playbook cman-aemp.yml --tags "create-app-apache"`
- Create app nginx use `ansible-playbook cman-aemp.yml --tags "create-app-nginx"`
- Create app wp apache use `ansible-playbook cman-wordpress.yml --tags "create-app-wp-apache"`
- Create app wp nginx use `ansible-playbook cman-wordpress.yml --tags "create-app-wp-nginx"`

### Delete app
- Delete app apache / apache wp use `ansible-playbook cman-aemp.yml --tags "delete-app-apache"`
- Delete app nginx / nginx wp use `ansible-playbook cman-aemp.yml --tags "delete-app-nginx"`
- Delete the last app (lamp) use `ansible-playbook cman-aemp.yml --tags "delete-lamp"`
- Delete the last app (lemp) use `ansible-playbook cman-aemp.yml --tags "delete-lemp"`

## Todo
- [x] optimiz : connect update, upgrade, kernel, swap and limits.
- [x] users : create users.
- [x] lamp : apache, mysql, php.
- [x] lamp-wp : apache, mysql, php, wp.
- [x] lemp : nginx, mysql, php.
- [x] lemp-wp : nginx, mysql, php, wp.
- [x] delete-app : nginx, apache, wp (apache & nginx).
- [ ] custom-php : php7.4 or php8.0