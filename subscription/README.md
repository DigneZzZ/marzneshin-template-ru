<p align="center">
  <a href="https://github.com/WhyMan1/marzban-template/tree/master/subscription" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/PreviewTemplate.png">
      <img width="372" height="408" src="https://raw.githubusercontent.com/WhyMan1/marzban-template/master/subscription/PreviewTemplate.png">
    </picture>
  </a>
</p>
<h1 align="center">Шаблон подписки для панели <a href="https://github.com/Gozargah/Marzban">Marzban</a></h1>

## Содержание
- [Особенности](#особенности)
- [Инструкция по установке](#инструкция-по-установке)

# Введение
Простой HTML-шаблон для улучшенного отображения информации о пользователе.

# Особенности
- Быстрое добавление ссылки на подписку в приложение sing-box
- Ссылки на загрузку необходимых приложений

# Инструкция по установке
1. Скачайте файл шаблона:
```sh
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/DigneZzZ/marzneshin-template-ru/master/subscription/index.html
```

2. Выполните следующие команды в терминале вашего сервера:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
```
или добавьте следующие значения в файл `.env` в директории `/opt/marzban`:
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
```

3. Перезапустите Marzban:
```sh
marzban restart
```

## Обновление
Для обновления шаблона достаточно повторить первый шаг.


