---
## Front matter
title: "Отчет по индивидуальному проекту. Этап 2."
subtitle: "Дисциплина: операционные системы."
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

Размещение данных на сайте.

# Выполнение работы

1. Заменим фото в каталоге ~/work/blog/content/autors/admin.

![*Добавление фотографии.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/1.png){#fig:001 width=70%}

2. В том же каталоге находим текстовый файл и меняем в нем данные.

![*Заполнение данных.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/2.png){#fig:002 width=70%}

3. Для того, чтобы создать пост о прошедшей неделе нам необходимо создать отдельную папку для него в каталоге ~/work/blog/content/post.

![*Создание папки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/3.png){#fig:003 width=70%}

4. Заполняем текстовый файл в созданном каталоге.

![*Заполнение файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/4.png){#fig:004 width=70%}

5. Для того, чтобы создать пост о системах контроля версий нам необходимо создать отдельную папку для него в каталоге ~/work/blog/content/post.

![*Создание папки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/5.png){#fig:005 width=70%}

6. Заполняем файл в созданном каталоге.

![*Заполнение файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/6.png){#fig:006 width=70%}

7. Для проверки всех предыдущих действий введем команду hugo server.

![*Проверка.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/7.png){#fig:007 width=70%}

8. После этого вводим команду hugo в каталоге public.

![*Команда hugo.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/8.png){#fig:008 width=70%}

9. Отправляем все изменения на github.

![*Отправка на github.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/9.png){#fig:009 width=70%}

10. Проверяем сайт, заходя через общедоступную ссылку.

![*Сайт с изменениями.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage2/report/image/ip2/10.png){#fig:010 width=70%}

# Вывод

Я разместила свою фотографию, свои данные, а также несколько постов на сайте.
