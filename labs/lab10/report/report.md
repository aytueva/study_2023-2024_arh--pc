---
## Front matter
title: "Отчёт по лабораторной работе №10"
subtitle: "Архитектура компьютера НММбд-03-24"
author: "Туева Анастасия Юрьевна"

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

Целью работы является приобретение навыков написания программ для работы с файлами

# Задание

1. Напишите программу работающую по следующему алгоритму: 
• Вывод приглашения “Как Вас зовут?” 
• ввести с клавиатуры свои фамилию и имя 
• создать файл с именем name.txt 
• записать в файл сообщение “Меня зовут” 
• дописать в файл строку введенную с клавиатуры 
• закрыть файл Создать исполняемый файл и проверить его работу. Проверить наличие файла и его содержимое с помощью команд ls и cat.

# Выполнение лабораторной работы

1. Создадим каталог для программ лабораторной работы № 10, перейдем в него и создадим файлы lab10-1.asm, readme-1.txt и readme-2.txt

![Переход в каталог и создание файлов](image/1.png){#fig:001 width=70%}

2. Введем в файл lab10-1.asm текст программы из Листинга 10.1 (Программа записи в файл сообщения). Создадим исполняемый файл и проверим его работу.

![Программа записи в файл сообщения](image/2.png){#fig:002 width=70%}

![Исполнение программы из листинга 10.1](image/3.png){#fig:003 width=70%}

3. С помощью команды chmod изменим права доступа к исполняемому файлу lab10-1, запретив его выполнение. Попытаемся выполнить файл. Выведенное сообщение означает, что у нас нет прав на исполнение файла, так как мы запретили это для всех пользователей.

![Изменение прав доступа к файлу lab10-1](image/4.png){#fig:004 width=70%}

4. С помощью команды chmod изменим права доступа к файлу lab10-1.asm с исходным текстом программы, добавив права на исполнение. Попытаемся выполнить его. Сам файл исполнить невозможно, его нужно транслировать в исполняемый файл. У нас получилось вернуть права на исполнение файла lab10-1, теперь программа работает корректно.

![Изменение прав доступа к файлу lab10-1.asm](image/5.png){#fig:005 width=70%}

5. В соответствии с вариантом в таблице 10.4 предоставим права доступа к файлу readme-1.txt представленные в символьном виде, а для файла readme-2.txt – в двоичном виде. Проверим правильность выполнения с помощью команды ls -l.

![Изменение прав доступа к файлам readme1.txt, readme2.txt](image/6.png){#fig:006 width=70%}

# Задания для самостоятельной работы

6. Напишем программу работающую по следующему алгоритму: 
• Вывод приглашения “Как Вас зовут?” • ввести с клавиатуры свои фамилию и имя 
• создать файл с именем name.txt 
• записать в файл сообщение “Меня зовут” 
• дописать в файл строку введенную с клавиатуры 
• закрыть файл Создаем исполняемый файл и проверить его работу. Проверим наличие файла и его содержимое с помощью команд ls и cat. Программа работает корректно.

![Текст программы lab10-2.asm](image/7.png){#fig:007 width=70%}

![Запуск и проверка программы](image/8.png){#fig:008 width=70%}

# Выводы

Благодаря данной лабораторной работе я приобрёла навыки написания программ для работы с файлами.
