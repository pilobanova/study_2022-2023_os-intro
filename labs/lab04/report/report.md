---
## Front matter
title: "Отчет по лабораторной работе №4"
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
  - \floatplacement{figure}{H} # keep figures where there are in the text/tmp.
---

# Цель работы

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Выполнение лабораторной работы

1. Определим полное имя домашнего каталога.

![*Команда pwd.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/1.png){ #fig:001 width=70% }

2. Перейдем в каталог /tmp.

![*Переход в каталог /tmp.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/2.png){ #fig:002 width=70% }

3. Выведем на экран содержимое каталога /tmp.

![*Команда ls.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/3.png){ #fig:003 width=70% }

![*Команда ls -a.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/4.png){ #fig:004 width=70% }

![*Команда ls -alF.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/5.png){ #fig:005 width=70% }

4. Определим, есть ли в каталоге /var/spool подкаталог с именем cron. Как видно по фотографии, такого подкаталога нет.

![*Содержание каталога /var/spool.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/6.png){ #fig:006 width=70% }

5. Перейдем в домашний каталог и выведем на экран его содержимое.

![*Содержание домашнего каталога.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/7.png){ #fig:007 width=70% }

6. В домашнем каталоге создадим новый каталог с именем newdir.

![*Создание каталога newdir.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/8.png){ #fig:008 width=70% }

7. В каталоге ~/newdir создадим новый каталог с именем morefun.

![*Создание каталога ~/newdir/morefun.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/9.png){ #fig:009 width=70% }

8. В домашнем каталоге создадим одной командой три новых каталога с именами letters, memos, misk. Затем удалим эти каталоги одной командой.

![*Создание трех каталогов letters, memos, misk.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/10.png){ #fig:010 width=70% }

![*Удаление каталогов letters, memos, misk.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/11.png){ #fig:011 width=70% }

9. Попробуем удалить ранее созданный каталог ~/newdir командой rm.

![*Команда rm.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/12.png){ #fig:012 width=70% }

10. Удалим каталог ~/newdir/morefun из домашнего каталога.

![*Удаление каталога ~/newdir/morefun.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/13.png){ #fig:013 width=70% }

11. С помощью команды man определим, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него.

![*Команда ls с опцией *.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/14.png){ #fig:014 width=70% }

12. . С помощью команды man определим набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов.

![*Команда ls с опциями -l, -t.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/15.png){ #fig:015 width=70% }

13. Используем команду man для просмотра описания следующих команд: cd, pwd, mkdir, rmdir, rm.

![*Команда man cd.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/16.png){ #fig:016 width=70% }

![*Команда man pwd.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/17.png){ #fig:017 width=70% }

![*Команда man mkdir.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/18.png){ #fig:018 width=70% }

![*Команда man rmdir.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/19.png){ #fig:019 width=70% }

![*Команда man rm.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/20.png){ #fig:020 width=70% }

14. Используя информацию, полученную при помощи команды history, выполним модификацию и исполнение нескольких команд из буфера команд.

![*Команда history.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/21.png){ #fig:021 width=70% }

![*Пример 1.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/22.png){ #fig:022 width=70% }

![*Пример 2.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab04/report/image/лаб4с2/23.png){ #fig:023 width=70% }

# Контрольные вопросы

1) Что такое командная строка?
    
В ОС Linux командная строка является основным элементов во взаимодействии пользователя и системы.
    
2) При помощи какой команды можно определить абсолютный путь текущего каталога? Приведите пример.

Для определения абсолютного пути к текущему каталогу используется команда pwd (print working directory). 
Например, при вводе данной команды в домашнем каталоге, он выведет /home/pilobanova.
    
3) При помощи какой команды и каких опций можно определить только тип файлов и их имена в текущем каталоге? Приведите примеры.

С помощью команды ls и опция F можно получить информацию о типах файлов (каталог, исполняемый файл, ссылка). 
Например, если ввести команду ls -F в домашнем каталоге, то выведется название каталогов, которые находятся в нем, и “/” после имени(Загрузки/).
    
4) Каким образом отобразить информацию о скрытых файлах? Приведите примеры.

С помощью команды ls и опция -a можно получить информацию о скрытых файлах. 
Например, если ввести команду ls -a в домашнем каталоге, то выведется название всех каталогов, включая скрытые (те, которые начинаюся с .).

5) При помощи каких команд можно удалить файл и каталог? Можно ли это сделать одной и той же командой? Приведите примеры.

Каталог можно удалить с помощью команды rmdir, а файлы с помощью rm. Если в каталоге есть какие-то файлы, то можно все сразу командой rm с опцией r.

6) Каким образом можно вывести информацию о последних выполненных пользователем командах? работы?

Команда history выводит все ранее выполненные команды, которые нумеруются

7) Как воспользоваться историей команд для их модифицированного выполнения? Приведите примеры.

Чтобы модифицировать выполнение команды необходимо ввести следующее: !(номер исходной команды):s/(то, что меняем)/(то, на что меняем).
Например, чтобы изменить команду ls –l –t на ls –a –t нужно ввести !(номер команды):s/-l/-a 

8) Приведите примеры запуска нескольких команд в одной строке.

Для использования нескольких команд последовательно в одной строке, необходимо их разделить их символом “;”. Например, > cd; ls

9) Дайте определение и приведите примера символов экранирования.

Экранирование символов — замена в тексте управляющих символов на соответствующие текстовые подстановки. Например, ‘.’

10) Охарактеризуйте вывод информации на экран после выполнения команды ls с опцией l.

Будет выведена следующая информация: тип файла, право доступа, число ссылок, владелец, размер, дата последней ревизии, имя файла или каталога.

11) Что такое относительный путь к файлу? Приведите примеры использования относительного и абсолютного пути при выполнении какой-либо команды.

Относительный показывает путь к файлу относительно какой-либо “отправной точки”. Например: > cd ~/work/study. Данной командой можно перейти в катало study из любой отправной точки, т.е. мы используем абсолютный путь к файлу. cd 2022-2023 Данной командой из каталога study можно перейти к каталогу 2022-2023. Такой путь можно назвать относительным

12) Как получить информацию об интересующей вас команде?

Воспользоваться командой man и через пробел ввести название команды, информацию которой мы хотим получить.

13) Какая клавиша или комбинация клавиш служит для автоматического дополнения вводимых команд?

Клавиша Tab служит для автоматического дополнения вводимых команд.

# Выводы

Я приобрела практические навыки взаимодействия пользователя с системой посредством командной строки.

