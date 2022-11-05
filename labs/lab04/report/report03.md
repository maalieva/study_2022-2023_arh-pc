---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Дисциплина: Архитектура компьютеров"
author: "Алиева Милена Арифовна"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Целью работы является изучить идеологию и применение средств контроля
версий git. Приобрести практические навыки по работе с системой git

# Задание

1) Базовая настройка git
2) Создание SSH ключа
3) Создание рабочего пространства и репозитория курса на основе
шаблона
4) Настройка каталога курса

# Теоретическое введение

Система контроля версий Git представляет собой набор программ командной
строки. Доступ к ним можно получить из терминала посредством ввода
команды git с различными опциями.


# Выполнение лабораторной работы

1) Базовая настройка git
Сначала сделаем предварительную конфигурацию git. Откроем терминал
и введём следующие команды, указав имя и email владельца репозитория
и настроим utf-8 в выводе сообщений git (рис. [-@fig:001])

![ указание имени и email владельца репозитория, настройка utf-8 в
выводе сообщений git] (image/1.png){ #fig:001 width=70% }

Зададим имя начальной ветки (будем называть её master), также зададим
параметры autocrlf и safecrlf (рис. [-@fig:002])

![ установка имени начальной ветки, параметров autocrlf и safecrlf] (image/2.png){ #fig:002 width=70% }

2) Создание SSH ключа
Для последующей идентификации пользователя на сервере репозиториев
сгенерируем пару ключей (приватный и открытый) (рис. [-@fig:003])

![ генерация приватного и открытого ключей] (image/3.png){ #fig:003 width=70% }

Далее загрузим сгенерённый открытый ключ. Для этого зайдём на сайт
под своей учетной записью и перейдем в Setting, затем в боковом меню
выберем SSH and GPG keys и нажмём на New SSH key. Скопировав из
локальной консоли ключ в буфер обмена вставляем ключ в появившееся
на сайте поле и указываем для ключа имя (Title).

3) Создание рабочего пространства и репозитория курса на основе шаблона
Откроем терминал и создадим каталог для предмета «Архитектура
компьютера» (рис. [-@fig:004])

![ создание каталога для предмета «Архитектура компьютера»] (image/4.png){ #fig:004 width=70% }

Создадим репозиторий на основе шаблона можно через web-интерфейс
github. Перейдём на станицу репозитория с шаблоном курса, выберем Use
this template. В открывшемся окне зададим имя репозитория (Repository name)
study_2022–2023_arh-pc и создадим репозиторий (Create repository from
template) (рис. [-@fig:006])

![ создание репозитория с именем study_2022–2023_arh-pc] (image/6.png){ #fig:006 width=70% }

Откроем терминал и перейдем в каталог курса. Клонируем созданный
репозиторий (рис. [-@fig:007])

![ клонирование репозитория] (image/6.png){ #fig:006 width=70% }

4) Настройка каталога курса
Перейдем в каталог курса и удалим лишние файлы. Создадим необходимые каталоги и отправим файлы на сервер (рис. [-@fig:009])

![ создание необходимых каталогов и отправка файлов на сервер] (image/6.png){ #fig:006 width=70% }

Загрузим все необходимые файлы на github.


# Выводы

В ходе выполнения лабораторной работы я изучила идеологию и применение
средств контроля версий git, а также приобрела практические навыки по
работе с системой git. 

# Список литературы{.unnumbered}

::: {#refs}
:::
