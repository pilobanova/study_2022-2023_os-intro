---
## Front matter
title: "Отчет по лабораторной работе №2"
subtitle: "Дисциплина: операционные системы"
author: "Лобанова Полина Иннокентьевна"

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

Целью работы является изучение идеологии и применения средств контроля версий и освоение умения по работе с git.

# Задание

Создать базовую конфигурацию для работы с git.
Создать ключ SSH.
Создать ключ PGP.
Настроить подписи git.
Зарегистрироваться на Github.
Создать локальный каталог для выполнения заданий по предмету.

# Выполнение лабораторной работы

1. Установим git.

![*Установка git.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/1.png){ #fig:001 width=70% }

2. Установим gh.

![*Установка gh.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/2.png){ #fig:002 width=70% }

3. Зададим имя и email владельца репозитория.

![*Имя пользователя и email.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/3.png){ #fig:003 width=70% }

4. Настроим utf-8 в выводе сообщений git.

![*Настройка utf-8.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/4.png){ #fig:004 width=70% }

5. Зададим имя начальной ветки.

![*Имя начальной ветки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/5.png){ #fig:005 width=70% }

6. Зададим параметр autocrlf.

![*Настройка параметра autocrlf.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/6.png){ #fig:006 width=70% }

7. Зададим параметр safecrlf.

![*Настройка параметра safecrlf.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/7.png){ #fig:007 width=70% }

8. Создадим ssh ключ.

![*Создание ssh ключа.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/8.png){ #fig:008 width=70% }

9. Сгенерируем pgp ключ.

![*Генерация pgp ключа.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/9.png){ #fig:009 width=70% }

10. Настроем github. 

![*Учетная запись на github.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/10.png){ #fig:010 width=70% }

11. Выведем список ключей и скопируем отпечаток приватного ключа.

![*Список ключей и отпечаток приватного ключа.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/11.png){ #fig:011 width=70% }

12. Скопируем наш сгенерированный pgp ключ в буфер обмена.

![*Копирование сгенерированного ключа в буфер обмена.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/12.png){ #fig:012 width=70% }

13. Используя введёный email, укажем Git применять его при подписи коммитов.

![*Настройка автоматических подписей коммитов  git.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/13.png){ #fig:013 width=70% }

14. Авторизируемся для настройки gh.

![*Авторизация.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/14.png){ #fig:014 width=70% }

![*Авторизация успешно выполнена.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/15.png){ #fig:015 width=70% }

15. Создадим репозиторий курса на основе шаблона.

![*Создание репозитория курса.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/16.png){ #fig:016 width=70% }

![*Создание репозитория курса.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/17.png){ #fig:017 width=70% }

16. Перейдем в каталог курса.

![*Переход в каталог ~/work/study/2022-2023/"Операционные системы"/os-intro.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/18.png){ #fig:018 width=70% }

17. Удалим лишний файл.

![*Удаление файла package.json.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/19.png){ #fig:019 width=70% }

18. Создадим необходимые каталоги.

![*Создание каталогов.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/20.png){ #fig:020 width=70% }

19. Отправим файлы на сервер.

![*Оправление файлов на сервер.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/21.png){ #fig:021 width=70% }

![*Оправление файлов на севрер.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/лаб2с2/22.png){ #fig:022 width=70% }

# Ответы на контрольные вопросы

1. Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются?
Система, позволяющая работать нескольким людям над одним проектом.
2. Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия.
Хранилище (репозиторий) - директория, хранящая конкретный проект; 
Коммит - текущее состояние рабочей копии;
История - последовательность коммитов в порядке, в котором они добавлялись в репозиторий; 
Рабочая копия - текущее состояние репозитория, которое находится в состоянии изменения.
3. Что представляют собой и чем отличаются централизованные и децентрализованные VCS? Приведите примеры VCS каждого вида.
В централизованных VCS (Mercurial) все пользователи подключены к единому серверу; в децентрализованных VCS пользователи подключены к нескольким владельцам.
4.  Опишите действия с VCS при единоличной работе с хранилищем.
При единоличной работе с хранилищем все изменения, созданные пользователем, не влияют на общий репозиторий.
5. Опишите порядок работы с общим хранилищем VCS.
Из общего хранилища можно получать изменения проекта.
6. Каковы основные задачи, решаемые инструментальным средством git?
git позволяет нескольким людям работать над одним проектом.
7. Назовите и дайте краткую характеристику командам git.
add - добавить файлы в коммит, 
push - отправить коммит на удалённый репозиторий; 
pull - импортировать проект с удалённого репозитория.
8. Приведите примеры использования при работе с локальным и удалённым репозиториями.
1) Работа с удаленным репозиторием: git remote – просмотр списка настроенных удаленных репозиториев.
2) Работа с локальным репозиторием: git status - выводит информацию обо всех изменениях, внесенных в дерево директорий проекта по сравнению с последним коммитом рабочей ветки
9. Что такое и зачем могут быть нужны ветви (branches)?
Создав новую ветвь, можно, не вредя проекту, работать над конкретной частью проекта.
10. Как и зачем можно игнорировать некоторые файлы при commit?
some files may well be user specific

# Выводы

Я изучила идеологию и применение средств контроля версий и освоила работу с git.


