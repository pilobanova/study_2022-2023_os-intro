---
## Front matter
title: "Отчет по лабораторной работе №1"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Выполнение лабораторной работы

1. Поскольку в первом семестре мы уже устанавливали VirtualBox с операционной системой Linux и проводили все необходимые настройки, я прикреплю все файлы с пояснениями своих действий.

![*Создание виртуальной машины.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/1.png){#fig:001 width=70%}

![*Указание названия ОС.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/2.png){#fig:002 width=70%}

![*Выбор объема памяти (4096).*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/3.png){#fig:003 width=70%}

![*Создание нового жесткого диска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/4.png){#fig:004 width=70%}

![*Тип диска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/5.png){#fig:005 width=70%}

![*Формат диска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/6.png){#fig:006 width=70%}

![*Размер диска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/7.png){#fig:007 width=70%}

![*Выбор объема видеопамяти (128).*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/8.png){#fig:008 width=70%}

![*Добавление оптического диска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/9.png){#fig:009 width=70%}

![*Запуск виртуальной машины и переход к дальнейшим настройкам.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/10.png){#fig:010 width=70%}

![*Выбор языка.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/11.png){#fig:011 width=70%}

![*Выбор часового пояса.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/12.png){#fig:012 width=70%}

![*Выбор устройства для установки ОС.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/13.png){#fig:013 width=70%}

![*Завершение установки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/14.png){#fig:014 width=70%}

![*Создание учетной записи.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/15.png){#fig:015 width=70%}

2. Переключимся на роль супер-пользователя.

![*Переключение на супер-пользователя.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/16.png){#fig:016 width=70%}

3. Обновим все пакеты.

![*Обновление пакетов.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/17.png){#fig:017 width=70%}

4. Установим программу для удобства работы в консоли.

![*Установка tmux.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/18.png){#fig:018 width=70%}

5. Установим программное обеспечение.

![*Установка программного обеспечения.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/19.png){#fig:019 width=70%}

6. Запустим таймер.

![*Запуск таймера.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/20.png){#fig:020 width=70%}

7. Для отключения системы безопасности SELinux изменим значение в файле /etc/selinux/config.

![*Переход в каталог.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/21.png){#fig:021 width=70%}

![*Изначальные вид файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/22.1.png){#fig:022 width=70%}

![*Измененный вид файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/22.2.png){#fig:023 width=70%}

8. Перезагрузим виртуальную машину.

![*Перезагрузка.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/23.png){#fig:024 width=70%}

9. Установим пакет DKMS.

![*Установка пакета DKMS.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/24.png){#fig:025 width=70%}

10. Настроим раскладку клавиатуры. Для этого отредактируем конфигурационный файл /etc/X11/xorg.conf.d/00-keyboard.conf.

![*Переход к файлу.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/25.png){#fig:026 width=70%}

![*Исходный текст файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/26.1.png){#fig:027 width=70%}

![*Измененный текст файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/26.2.png){#fig:028 width=70%}

11. Перезагрузим виртуальную машину.

![*Перезагрузка.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/23.png){#fig:029 width=70%}

12. Поскольку при создании виртуальной машины я правильно указала имя пользователя, то мы пропустим этот шаг.

13. Также в первом семестре мы устанавливали pandoc и texlive.

![*Установка pandoc.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/28.png){#fig:030 width=70%}

![*Установка texlive.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/29.png){#fig:031 width=70%}

# Домашнее задание

1. С помощью команд dmesg | less и dmesg | grep -i "то, что ищем" получим 
Версия ядра Linux (Linux version).
Частота процессора (Detected Mhz processor).
Модель процессора (CPU0).
Объём доступной оперативной памяти (Memory available).
Тип обнаруженного гипервизора (Hypervisor detected).

![*Версия ядра Linux.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/30.png){#fig:032 width=70%}

![*Частота процессора.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/31.png){#fig:033 width=70%}

![*Модель процессора.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/32.png){#fig:034 width=70%}

![*Объём доступной оперативной памяти.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/33.png){#fig:035 width=70%}

![*Тип обнаруженного гипервизора.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/лаб1с2/34.png){#fig:036 width=70%}

# Контрольные вопросы

1.  Какую информацию содержит учётная запись пользователя? 
1) Имя пользователя (user name)   
2) Индентификационный номер пользвателя (UID) 
3) Индентификационный номер группы (GID) 
4) Пароль (password) 
5) Полное имя (full name) 
6) Домашний каталог (home directory) 
7) Начальную оболочку (login shell)

2. Укажите команды терминала и приведите примеры: 
1) для получения справки по команде –help 
2) для перемещения по файловой системе -cd 
3) для просмотра содержимого каталога -ls 
4) для определения объёма каталога du 
5) для создания / удаления каталогов / файлов - mkdir -создание, rm -r - удаление 
6) для задания определённых прав на файл / каталог - touch/rm
7) для просмотра истории команд -history 

3. Что такое файловая система? Приведите примеры с краткой характеристикой. 
Файловая система - порядок, определяющий способ организации, хранения и наименования данных на носителях иации в пк, а также в другом электронном оборудовании: цифровых фотоаппаратах, мобильных телефона и тд. Файловая система определяет формат содержимого и способ физического хранения информации, которую принято группировать в виде файлов. Конкретная файловая система и раздел, набор атрибутов файла. Некоторые файловые системы представляют сервисные возможности, например, разграничение доступа или цифрование файлов. 

4. Как посмотреть, какие файловые системы подмонтированы в ОС? 
Df - утилита, показывающая список всех файловых систем по имени устройства, сообщает их размер, занятое и свободное пространство и точки монтирования. При выполнении без аргумента, команда mount выведет все подключенные данные. 

5. Как удалить зависший процесс? 
С помощью команды killall-killall ()

# Выводы

Я приобрела практические навыки установки операционной системы на виртуальную машине, настройки минимально необходимых для дальнейшей работы сервисов. 

