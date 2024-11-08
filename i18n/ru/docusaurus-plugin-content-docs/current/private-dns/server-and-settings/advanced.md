---
title: Расширенные настройки
sidebar_position: 2
---

Раздел «Расширенные настройки» предназначен для более опытных пользователей и включает следующие параметры.

## Ответ на заблокированные домены

Здесь можно выбрать DNS-ответ для заблокированного запроса:

- **По умолчанию**: Отвечает с нулевым IP-адресом (0.0.0.0 для A; :: для AAAA), когда заблокировано правилом в стиле Adblock; отвечает с IP-адресом, указанным в правиле, когда заблокировано правилом в стиле /etc/hosts
- **REFUSED**: Отвечает с кодом REFUSED
- **NXDOMAIN**: Отвечает с кодом NXDOMAIN
- **Пользовательский IP**: Отвечает с вручную настроенным IP-адресом

## TTL (время жизни)

Время жизни (TTL) задаёт период (в секундах), в течение которого устройство клиента будет хранить ответ на DNS-запрос в кеше и извлекать его без повторного обращения к DNS-серверу. Если значение TTL велико, недавно разблокированные запросы могут ещё некоторое время выглядеть заблокированными. Если TTL равен 0, устройство не кеширует ответы.

## Блокировать доступ к Частному узлу iCloud

Устройства с Частным узлом iCloud могут игнорировать настройки DNS, поэтому AdGuard DNS не может их защитить.

## Блокировать канареечный домен Firefox

Не позволяет Firefox переключаться на DNS преобразователь (DNS resolver) в настройках, если AdGuard DNS настроен на уровне системы.

## Записывать IP-адреса

По умолчанию AdGuard DNS не записывает IP-адреса входящих DNS-запросов. Если вы включите эту настройку, IP-адреса будут записываться и отображаться в журнале запросов.
