# **Маркировки ИИ**

Переношу свой легаси пет-проект на современный стек
Переношу свой легаси пет-проект на современный стек.

## Деплой на прод: 

- **Копировать** `ansible-deploy/group_vars/production.yml.example` в `ansible-deploy/group_vars/production.yml`
cd ansible-deploy && ansible-playbook -i inventory.ini playbook.yaml и заполнить параметры.
- **Копировать** `ansible-deploy/inventory.ini.example` в `ansible-deploy/inventory.ini`
- **Выполнить** `ansible-playbook -i inventory.ini playbook.yaml` из директории `ansible-deploy`  

## Полезные команды
- `$ ssh-keygen -R 80.247.210.130` - сбрасываем ключи для хоста (в случае, если была переустановлена ОС)
- `$ sudo nginx -t && sudo systemctl restart nginx` - проверка конфигурационного файла и перезапуск сервера
