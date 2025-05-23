---
## Front matter
lang: ru-RU
title: Лабораторная работа № 12
subtitle: Настройка NAT
author:
  - Оразгелдиев Язгелди
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

  * Оразгелдиев Язгелди
  * студент
  * Российский университет дружбы народов
  * [orazgeldiyev.yazgeldi@gmail.com](mailto:orazgeldiyev.yazgeldi@gmail.com)
  * <https://github.com/YazgeldiOrazgeldiyev>

## Цель работы

Приобретение практических навыков по настройке доступа локальной сети
к внешней сети посредством NAT.

## Задание

1. Сделать первоначальную настройку маршрутизатора provider-gw-1 и коммутатора provider-sw-1 провайдера: задать имя, настроить доступ по паролю и т.п.
2. Настроить интерфейсы маршрутизатора provider-gw-1 и коммутатора provider-sw-1 провайдера.
3. Настроить интерфейсы маршрутизатора сети «Донская» для доступа к сети провайдера.
4. Настроить на маршрутизаторе сети «Донская» NAT с правилами.
5. Настроить доступ из внешней сети в локальную сеть организации
6. Проверить работоспособность заданных настроек.
7. При выполнении работы необходимо учитывать соглашение об именовании

## Содержание исследования

![Первоначальная настройка маршрутизатора provider-gw-1](image/1.jpg){#fig:001 width=50%}

## Содержание исследования

![Первоначальная настройка маршрутизатора provider-sw-1](image/2.jpg){#fig:002 width=50%}

## Содержание исследования

![Настройка интерфейсов маршрутизатора provider-gw-1](image/3.jpg){#fig:003 width=50%}

## Содержание исследования

![Настройка интерфейсов коммутатора provider-sw-1](image/4.jpg){#fig:004 width=50%}

## Содержание исследования

![Настройка интерфейсов маршрутизатора msk-donskaya-gw-1](image/5.jpg){#fig:005 width=50%}

## Содержание исследования

![Проверка доступности маршрутизатора](image/6.jpg){#fig:006 width=50%}

## Содержание исследования

![Настройка пула адресов для NAT](image/7.jpg){#fig:007 width=50%}

## Содержание исследования

![Настройка списка доступа для NAT](image/8.jpg){#fig:008 width=50%}

## Содержание исследования

![Настройка Port Address Translation](image/9.jpg){#fig:009 width=50%}

## Содержание исследования

![Проверка доступности маршрутизатора](image/10.jpg){#fig:010 width=50%}

## Содержание исследования

![Проверка доступности маршрутизатора](image/11.jpg){#fig:011 width=50%}

## Содержание исследования

![Доступ dk-donskaya к www.yandex.ru](image/12.jpg){#fig:012 width=50%}

## Содержание исследования

![Доступ dep-donskaya к 192.0.2.13](image/13.jpg){#fig:013 width=50%}

## Содержание исследования

![Доступ adm-donskaya к 192.0.2.14](image/14.jpg){#fig:014 width=50%}

## Содержание исследования

![Доступ dk-donskaya к 192.0.2.11](image/15.jpg){#fig:015 width=70%}

## Результаты

В результате выполнения лабораторной работы я приобрел навыки по настройке доступа локальной сети к внешней сети посредством NAT
