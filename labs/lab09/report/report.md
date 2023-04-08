---
## Front matter
title: "Отчет по лабораторной работе №9"
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Выполнение лабораторной работы

1. Откроем редактор emacs.

![*Редактор emacs.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/1.png){#fig:001 width=70%}


2. Создадим файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).

![*Создание файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/2.png){#fig:002 width=70%}

3. Наберием текст:
1 #!/bin/bash
2 HELL=Hello
3 function hello {
4 LOCAL HELLO=World
5 echo $HELLO
6 }
7 echo $HELLO
8 hello

![*Ввод текста.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/3.png){#fig:003 width=70%}

4. Сохраним файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s).

![*Сохранение файла.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/4.png){#fig:004 width=70%}

5. Вырежем одной командой целую строку (С-k).

![*Удаление строки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/5.png){#fig:005 width=70%}

6. Вставим эту строку в конец файла (C-y).

![*Вставка этой строки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/6.png){#fig:006 width=70%}

7. Выделим область текста (C-space).

![*Выделение области.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/7.png){#fig:007 width=70%}

8. Скопируем область в буфер обмена (M-w).

9.  Вставим область в конец файла.

![*Вставка этой области.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/8.png){#fig:008 width=70%}

10. Вновь выделим эту область и на этот раз вырежем её (C-w).

![*Удаление этой области.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/9.png){#fig:009 width=70%}

11. Отменим последнее действие (C-/).

![*Отмена последнего действия.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/10.png){#fig:010 width=70%}

12. Переместим курсор в начало строки (C-a).

![*Перенос курсора в начало строки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/11.png){#fig:011 width=70%}

13. Переместим курсор в конец строки (C-e).

![*Перенос курсора в конец строки.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/12.png){#fig:012 width=70%}

14. Переместим курсор в начало буфера (M-<).

![*Перенос курсора в начало буфера.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/13.png){#fig:013 width=70%}

15. Переместим курсор в конец буфера (M->).

![*Перенос курсора в конец буфера.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/14.png){#fig:014 width=70%}

16. Выведем список активных буферов на экран (C-x C-b).

![*Список активных буферов.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/15.png){#fig:015 width=70%}

17. Переместимся во вновь открытое окно (C-x) o со списком открытых буферов
и переключимся на другой буфер.

![*Переключение на другой буфер.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/16.png){#fig:016 width=70%}

18. Закроем это окно (C-x 0).

![*Закрытие окна.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/17.png){#fig:017 width=70%}

19. Теперь вновь переключимся между буферами, но уже без вывода их списка на
экран (C-x b).

![*Переключение между буферами.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/18.png){#fig:018 width=70%}

20. Поделим фрейм на 4 части: разделим фрейм на два окна по вертикали (C-x 3),
а затем каждое из этих окон на две части по горизонтали (C-x 2).

![*Разделение фрейма.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/19.png){#fig:019 width=70%}

21. В каждом из четырёх созданных окон откроем новый буфер (файл) и введем несколько строк текста.

![*Открытие новых буферов и их заполнение.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/20.png){#fig:020 width=70%}

22. Переключимся в режим поиска (C-s) и найдем несколько слов, присутствующих в тексте.

![*Переключение в режим поиска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/21.png){#fig:021 width=70%}

23. Переключаемся между результатами поиска, нажимая C-s.

![*Переключение между результатами поиска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/22.png){#fig:022 width=70%}

24. Выйдем из режима поиска, нажав C-g.

![*Выход из режима поиска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/23.png){#fig:023 width=70%}

25. Перейдем в режим поиска и замены (M-%), введем текст, который следует найти
и заменить, нажмем Enter , затем введем текст для замены. После того как будут
подсвечены результаты поиска, нажмем ! для подтверждения замены.

![*Переход в режим поиска и замены.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/24.png){#fig:024 width=70%}

26. Испробуем другой режим поиска, нажав M-s o.

![*Другой режим поиска.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab09/report/image/лаба9с2/25.png){#fig:025 width=70%}

# Контрольные вопросы

1. Кратко охарактеризуйте редактор emacs.

Emacs представляет собой мощный экранный редактор текста, написанный на языке высокого уровня Elisp.

2. Какие особенности данного редактора могут сделать его сложным для освоения новичком?

Многие рутинные операции в Emacs удобнее производить с помощью клавиатуры, а не графического меню. Наиболее часто в командах Emacs используются сочетания c клавишами Ctrl и Meta (в обозначениях Emacs: C- и M-; клавиша Shift в Emasc обозначается как S-). Так как на клавиатуре для IBM PC совместимых ПК клавиши Meta нет, то вместо неё можно использовать Alt или Esc.

3. Своими словами опишите, что такое буфер и окно в терминологии emacs’а.

Если своими словами, то буфер - это файл, содержащий какой-либо текст. Окно же можно сказать область, где вы водится текст определенного буфера.

4. Можно ли открыть больше 10 буферов в одном окне?

Можно открыть больше 10 буферов в одном окне.

5. Какие буферы создаются по умолчанию при запуске emacs?

Только что запущенный Emacs несет один буфер с именем `scratch’, который может быть использован для вычисления выражений Лиспа в Emacs.

6. Какие клавиши вы нажмёте, чтобы ввести следующую комбинацию C-c | и C-c C-|?

Ctrl-c |(первые две нажму вместе, а третью отдельно), Ctrl-c Ctrl-|(каждую пару нажму раздельно).

7. Как поделить текущее окно на две части?

Разделить фрейм на два окна по вертикали (C-x 3),а по горизонтали (C-x 2)

8. В каком файле хранятся настройки редактора emacs?

В файле Emacs хранятся настройки редактора.

9. Какую функцию выполняет клавиша и можно ли её переназначить?

Кнопка BACKSPACE = функции C-k и ее можно переназначить.

10. Какой редактор вам показался удобнее в работе vi или emacs? Поясните почему

Редактор Emacs мне показался удобнее, так как в нем больше возможностей по сравнению с vi.

# Вывод

Я ознакомилась с операционной системой Linux и получила практические навыки работы с редактором Emacs.

