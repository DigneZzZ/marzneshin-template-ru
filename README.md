<h1 align="center">Шаблон для панели <a href="https://github.com/marzneshin/marzneshin">Марзнешин</a></h1>

# Введение
Настраиваемый шаблон для панели Марзнешин.

# Установка
Чтобы установить шаблон, выполните следующие команды в терминале вашего сервера:

1. Скачайте файл шаблона:
```sh
sudo wget -N -P /var/lib/marzneshin/templates/subscription/ https://raw.githubusercontent.com/MatinDehghanian/marzneshin-template/master/subscription/index.html
```

2. Выполните следующие команды в терминале вашего сервера:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"' | sudo tee -a /etc/opt/marzneshin/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /etc/opt/marzneshin/.env
```
или добавьте следующие значения в файл `.env` в директории `/etc/opt/marzneshin`:
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
```

3. Перезапустите Марзнешин:
```sh
marzneshin restart
```

## Обновление
Чтобы обновить шаблоны, просто повторите первый шаг.
