# Домашнее задание к занятию 3 «Использование Ansible»

## Подготовка к выполнению

1. Подготовьте в Yandex Cloud три хоста: для `clickhouse`, для `vector` и для `lighthouse`.

![image](https://github.com/user-attachments/assets/2fd3e0ff-7d23-43fe-9e4f-80d2bb5ff5dd)

Развернул через terraform

2. Репозиторий LightHouse находится [по ссылке](https://github.com/VKCOM/lighthouse).

## Основная часть

1. Допишите playbook: нужно сделать ещё один play, который устанавливает и настраивает LightHouse.
2. При создании tasks рекомендую использовать модули: `get_url`, `template`, `yum`, `apt`.
3. Tasks должны: скачать статику LightHouse, установить Nginx или любой другой веб-сервер, настроить его конфиг для открытия LightHouse, запустить веб-сервер.
4. Подготовьте свой inventory-файл `prod.yml`.
5. Запустите `ansible-lint site.yml` и исправьте ошибки, если они есть.

![image](https://github.com/user-attachments/assets/938dae37-48a6-4655-84db-75c623a7694f)


6. Попробуйте запустить playbook на этом окружении с флагом `--check`.

![image](https://github.com/user-attachments/assets/129e83d2-cd5b-4949-96c1-c700b57b8984)

7. Запустите playbook на `prod.yml` окружении с флагом `--diff`. Убедитесь, что изменения на системе произведены.

![image](https://github.com/user-attachments/assets/299f7ea7-ffbb-4019-8345-417dda34623b)


8. Повторно запустите playbook с флагом `--diff` и убедитесь, что playbook идемпотентен.

![image](https://github.com/user-attachments/assets/910070d6-ebf9-4021-b909-d2e1fd30f54d)


9. Подготовьте README.md-файл по своему playbook. В нём должно быть описано: что делает playbook, какие у него есть параметры и теги.
10. Готовый playbook выложите в свой репозиторий, поставьте тег `08-ansible-03-yandex` на фиксирующий коммит, в ответ предоставьте ссылку на него.
https://github.com/olegveselov1984/08-ansible-03-yandex/tree/HW01
---

![image](https://github.com/user-attachments/assets/d761824f-fdad-40a4-952c-5e4f1094ed8f)
