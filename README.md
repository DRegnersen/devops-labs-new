# Brand-new repository with Devops labs
Devops labs — Denis Dubovikov, Daniil Kurepin (M34031)

### Ansible & Ansible Galaxy

Чтобы запустить плейбук и выполнить его, сначала нужно скачать роли:
```
ansible-galaxy install -r requirements.yml
```

Далее соотвественно с лабораторной работой запускаем плейбук с нужным инвентори файлом:
```
ansible-playbook -i inventories/lab-<номер лабы от 1 до 4>/hosts playbook.yml
```

Пример:
```
ansible-playbook -i inventories/lab-2/hosts playbook.yml
```

### Molecule

Чтобы запустить тесты molecule выполняем команду:
```
molecule test
```