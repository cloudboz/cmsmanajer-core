# Requirements
- Your server must be Ubuntu version 18.04/20.04 (64-bit recommended).
- Only clean servers (no NGINX, Apache or MySQL installed).
- Installed python2 or python3.
- Minimum of RAM 256MB.
- Open port 22, 80, 443.
- Use static public IPv4.

# Installed
- Postfix
- Memcached
- Fail2ban
- Redis
- UFW
- php-memcached

# Environments
- AMP (Apache, MySQL, PHP)
- EMP (Nginx, MySQL, PHP)
- AMN (Apache, MySQL, Node.js)
- EMN (Nginx, MySQL, Node.js)
- AMPy (Apache, MySQL, Python)
- EMPy (Nginx, MySQL, Python)

# How to Use?
## Install environments
```
ansible-playbook cman.yml --tags "install-amp"
ansible-playbook cman.yml --tags "install-emp"
ansible-playbook cman.yml --tags "install-amn"
ansible-playbook cman.yml --tags "install-emn"
ansible-playbook cman.yml --tags "install-ampy"
ansible-playbook cman.yml --tags "install-empy"
```

## Purge environments
```
ansible-playbook cman.yml --tags "purge-amp"
ansible-playbook cman.yml --tags "purge-emp"
ansible-playbook cman.yml --tags "purge-amn"
ansible-playbook cman.yml --tags "purge-emn"
ansible-playbook cman.yml --tags "purge-ampy"
ansible-playbook cman.yml --tags "purge-empy"
```

## Create & delete databases
```
ansible-playbook cman.yml --tags "create-db"
ansible-playbook cman.yml --tags "delete-db"
```

## Import & Export databases
```
ansible-playbook cman.yml --tags "import-db"
ansible-playbook cman.yml --tags "export-db"
```

## Create & delete system user
```
ansible-playbook cman.yml --tags "create-sysuser"
ansible-playbook cman.yml --tags "delete-sysuser"
```

## Deploy & destroy wordpress
```
ansible-playbook cman.yml --tags "deploy-wordpress"
ansible-playbook cman.yml --tags "destroy-wordpress"
```

## Deploy & destroy joomla
```
ansible-playbook cman.yml --tags "deploy-joomla"
ansible-playbook cman.yml --tags "destroy-joomla"
```

## Deploy & destroy drupal
```
ansible-playbook cman.yml --tags "deploy-drupal"
ansible-playbook cman.yml --tags "destroy-drupal"
```

## Deploy & destroy prestashop
```
ansible-playbook cman.yml --tags "deploy-prestashop"
ansible-playbook cman.yml --tags "destroy-prestashop"