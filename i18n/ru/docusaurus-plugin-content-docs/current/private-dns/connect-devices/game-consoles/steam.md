---
title: Steam Deck
sidebar_position: 5
---

Игровые консоли не поддерживают зашифрованный DNS, но они отлично подходят для настройки Публичного AdGuard DNS или Личного AdGuard DNS через привязанный IP-адрес.

Скорее всего, ваш роутер поддерживает использование зашифрованных DNS-серверов, поэтому вы всегда можете настроить Личный AdGuard DNS на нём и подключить к нему вашу игровую консоль.

[Как настроить ваш роутер](/private-dns/connect-devices/routers/routers.md)

## Подключиться к AdGuard DNS

Настройте вашу игровую консоль для использования Публичного AdGuard DNS или настройте её через привязанный IP:

1. Откройте настройки Steam Deck, нажав на значок шестерёнки в правом верхнем углу экрана.
2. Нажмите _Сеть_.
3. Щелкните значок шестерёнки рядом с сетевым подключением, которое вы хотите настроить.
4. Выберите IPv4 или IPv6, в зависимости от типа используемой сети.
5. Выберите «Только автоматические адреса (DHCP)» или «Автоматические (DHCP)».
6. В поле «DNS-сервер» введите один из следующих адресов DNS-сервера:
   - `94.140.14.49`
   - `94.140.14.59`
7. Сохраните изменения.

Предпочтительнее использовать привязанный IP (или выделенный IP, если у вас подписка Team):

- [Выделенные IP-адреса](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [Привязанные IP-адреса](/private-dns/connect-devices/other-options/linked-ip.md)