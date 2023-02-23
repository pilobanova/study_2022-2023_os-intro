---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №3."
subtitle: "Дисциплина: операционные системы."
author:
  - Лобанова П. И.
institute:
  - Российский университет дружбы народов, Москва, Россия
  - Факультет физико-математических и естественных наук
date: 24.02.2023

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
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Лобанова Полина Иннокентьевна
  * учащаяся факультета физико-математических и естественных наук
  * учащаяся направления "Математика и механика"
  * Российский университет дружбы народов
  * [polla-2004@mail.ru](polla-2004@mail.ru)

:::
::: {.column width="30%"}


:::
::::::::::::::

# Цель лабораторной работы

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Ход работы

## Установка необходимых сервисов

Для начала необходимо установить pandoc, pandoc-crossref и Texlive.

![*Установка pandoc.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/1.png){.column width="30%"}

## 

![*Установка Texlive.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/2.png){.column width="30%"}

## Шаблон

Далее необходимо было настроить git, репозиторий и каталог курса для того, чтобы получить шаблон отчета, а также Makefile.

![*Настройка каталога курса.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/3.png){.column width="30%"}

## Заполнение шаблона

Следующим и основным этапом работы является заполнение шаблона. То есть заполнение титульного листа, внесение каких-либо личных данных, а также описание цели работы, задания, вывода  с подкреплением их скриншотами, а также ответы на контрольные вопросы.

![*Исходный шаблон.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/4.png){.column width="30%"}

##

![*Заполненный отчет.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/5.png){.column width="30%"}

## Компиляция файла

После заполнения отчета необходимо создать docx и pdf файлы, введя команду make.

![*Компиляция файлов.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/6.png){.column width="30%"}

## Проверка

И последним этапом является проверка созданных файлов.

![*Готовый pdf файл.*](/home/pilobanova/work/study/2022-2023/Операционные системы/os-intro/labs/lab03/presentation/image/лаб3с2/7.png){.column width="30%"}

# Вывод 

Я научилась оформлять отчёты с помощью легковесного языка разметки Markdown.
