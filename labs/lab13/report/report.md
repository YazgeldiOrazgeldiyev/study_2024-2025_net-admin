---
## Front matter
title: "Лабораторная работа № 13"
subtitle: "Статическая маршрутизация в Интернете. Планирование"
author: "Оразгелдиев Язгелди"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Провести подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством статической маршрутизации локальной сети с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Задание

1. Внести изменения в схемы L1, L2 и L3 сети, добавив в них информацию о сети основной территории (42-й квартал в Москве) и сети филиала в г. Сочи.
2. Дополнить схему проекта, добавив подсеть основной территории организации 42-го квартала в Москве и подсеть филиала в г. Сочи (раздел 13.4.1).
3. Сделать первоначальную настройку добавленного в проект оборудования
4. При выполнении работы необходимо учитывать соглашение об именовании

# Выполнение лабораторной работы

Внесли изменения в схемы L1, L2 и L3 сети

![Схема L1](image/1.jpg){#fig:001 width=70%}

![Схема L2](image/2.jpg){#fig:002 width=70%}

![Схема L3](image/3.jpg){#fig:003 width=70%}

На схеме прошлого проекта разместили необходимое оборудование: 4 медиаконвертера (Repeater-PT), 2 маршрутизатора типа Cisco 2811, 1 маршрутизирующий коммутатор типа Cisco 3560-24PS, 2 коммутатора типа Cisco 2950-24, коммутатор Cisco 2950-24T, 3 оконечных устройства типа PC-PT. Присвоил названия рамещенным объектам

![Схема сети с дополнительными площадками](image/6.jpg){#fig:004 width=70%}

На медиаконвертерах заменили имеющиеся модули на PT-REPEATERNM-1FFE и PT-REPEATER-NM-1CFE для подключения витой пары по технологии Fast Ethernet и оптоволокна соответственно

![Медиаконвертер с модулями PT-REPEATER-NM-1FFE PT-REPEATER-NM-1CFЕ](image/4.jpg){#fig:005 width=70%}

На маршрутизаторе msk-q42-gw-1 добавьте дополнительный интерфейс NM-2FE2W 

![дополнительный интерфейс NM-2FE2W на маршрутизаторе msk-q42-gw-1](image/5.jpg){#fig:006 width=70%}

В физической рабочей области Packet Tracer добавили в г. Москва здание 42-го квартала, присвоили ему соответствующее название.

![Здание основной территории организации в Москве на физической схеме проекта](image/7.jpg){#fig:007 width=70%}

В физической рабочей области Packet Tracer добавьте город Сочи и в нём здание филиала, присвойте ему соответствующее название.

![Москва и Сочи на физической схеме проекта](image/8.jpg){#fig:008 width=70%}

Перенесли из сети «Донская» оборудование сети 42-го квартала и сети филиала в соответствующие здания 

![Размещение объектов в основном здании 42-го квартала в Москве](image/9.jpg){#fig:009 width=70%}

![Размещение объектов в основном здании в филиале Сочи](image/10.jpg){#fig:010 width=70%}

Сделали первоначальную настройку добавленного в проект оборудования

![Первоначальная настройка маршрутизатора msk-q42-gw-1](image/11.jpg){#fig:011 width=70%}

![Первоначальная настройка маршрутизатора msk-q42-sw-1](image/12.jpg){#fig:012 width=70%}

![Первоначальная настройка маршрутизатора msk-hostel-gw-1](image/13.jpg){#fig:013 width=70%}

![Первоначальная настройка маршрутизатора msk-hostel-sw-1](image/14.jpg){#fig:014 width=70%}

![Первоначальная настройка маршрутизатора sch-sochi-sw-1](image/15.jpg){#fig:015 width=70%}

![Первоначальная настройка маршрутизатора sch-sochi-gw-1](image/16.jpg){#fig:016 width=70%}

# Выводы

Я провел подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством маршрутизации локальной сети с сетью основного здания расположенного в 42-м квартале в Москве и сетью филиала в Сочи
