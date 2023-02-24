---
## Front matter
title: "Отчет о выполнении первого этапа индивидуального проекта"
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

# Выполнение первого этапа

1. Скачаем исполняемый файл hugo.

![*Скачивание hugo.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/1.png){ #fig:001 width=70% }

2. Разархивируем его и перенесем в каталог bin.

![*Файл hugo в каталоге bin.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/2.png){ #fig:002 width=70% }

3. Перейдем на github и создадим новый репозиторий с названием "ippi", используя данный шаблон.

![*Репозиторий, используемый, как шаблон.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/3.png){ #fig:003 width=70% }

![*Создание моего репозитория.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/4.png){ #fig:004 width=70% }

4. Перейдя в терминал, скопируем репозиторий в каталог work.

![*Клонирование репозитория.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/5.png){ #fig:005 width=70% }

5. Далее введем команду "~/bin/hugo".

![*Команда "~/bin/hugo".*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/6.png){ #fig:006 width=70% }

6. У нас появились необходимые файлы, но нам нужно удалить один файл "public".

![*Удаление файла public.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/7.png){ #fig:007 width=70% }

7. Далее введем команду "~/bin/hugo server".

![*Команда "~/bin/hugo server".*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/8.png){ #fig:008 width=70% }

8. На экране появится адрес ссылки, по которой нам нужно перейти. Тогда мы увидим наш сайт.

![*Сайт.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/9.png){ #fig:009 width=70% }

9. На сайте есть область синего цвета. Для того, чтобы ее удалить нам необходимо отредактировать файл ~/work/ippi/content/_index.md.

![*Исходный текст файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/10.png){ #fig:010 width=70% }

![*Отредактированный текст файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/11.png){ #fig:011 width=70% }

10. Далее создадим новый репозиторий с названием "pilobanova.github.io".

![*Создание нового репозитория.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/12.png){ #fig:012 width=70% }

11. Клонируем новый репозиторий в каталог work (рядом с ippi).

![*Клонирование репозитория.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/13.png){ #fig:013 width=70% }

12. Переходим в новый каталог и вводим команду для создания ветки.

![*Создание ветки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/14.png){ #fig:014 width=70% }

13. Создаем пустой файл.

![*Создание файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/15.png){ #fig:015 width=70% }

14. Загружаем все это на github.

![*Загрузка на github.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/16.png){ #fig:016 width=70% }

15. Далее создаем каталог ~/work/ippi/public и привязываем к нему наш новый репозиторий.

![*Каталог public.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/17.png){ #fig:017 width=70% }

16. Нам выдаем ошибку и для того, чтобы ее исправить нам нужно отредактировать файл ".gitignore".

![*Исходный текст файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/18.png){ #fig:018 width=70% }

![*Отредактированный текст файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/19.png){ #fig:019 width=70% }

17. Далее нужно повторить команду, указанную в пункте 15.

![*Привязываение репозитория.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/20.png){ #fig:020 width=70% }

18. Введем команду "~/bin/hugo". У нас появятся необходимые файлы теперь в каталоге public.

![*Создание необходимых файлов.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/21.png){ #fig:021 width=70% }

19. Загрузим все новые файлы на github.

![*Загрузка на github.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/22.png){ #fig:022 width=70% }

![*Загрузка на github.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/23.png){ #fig:023 width=70% }

20. Проверим все ли сделано правильно.

![*Верно отредактированный репозиторий.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/24.png){ #fig:024 width=70% }

21. Проверим открывается ли наш сайт через github.

![*Наш сайт.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/ip1/25.png){ #fig:025 width=70% }

# Вывод

Я создала исходный сайт, который в дальнейшем буду редактировать, и сделала так, что его можно просмотреть с разных устройств, используя github.
