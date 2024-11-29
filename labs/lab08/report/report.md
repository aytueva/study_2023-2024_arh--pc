---
## Front matter
title: "Отчёт по лабораторной работе №8"
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

Приобрести навыки написания программ с использованием циклов и обработкой аргументов командной строки.

# Выполнение лабораторной работы

Создаём каталог для программам лабораторной работы № 8, переходим в него и создаём файл "lab8-1.asm" (рис. [-@fig:001]).

![Создание файла](image/1.jpg){ #fig:001 width=70% }

Открываем созданный файл "lab8-1.asm", вставляем в него данный текст в соответствием с листингом 8.1. (рис. [-@fig:002]).

![Редактирование файла](image/2.jpg){ #fig:002 width=70% }

Создаем исполняемый файл программы и запускаем его (рис. [-@fig:003]).

![Запуск исполняемого файла](image/3.jpg){ #fig:003 width=70% }

Изменяем в текст программы добавив изменение значение регистра "ecx" в цикле (рис. [-@fig:004]). 

![Редактирование файла](image/4.jpg){ #fig:004 width=70% }

Создаем новый исполняемый файл программы и запускаем его (рис. [-@fig:005]). 

![Запуск исполняемого файла](image/5.jpg){ #fig:005 width=70% }

Изменяем в текст программы добавив команды "push" и "pop" для сохранения значения счетчика цикла "loop" (рис. [-@fig:006]).

![Редактирование файла](image/6.jpg){ #fig:006 width=70% }

Создаем новый исполняемый файл программы и запускаем его (рис. [-@fig:007]).

![Запуск исполняемого файла](image/7.jpg){ #fig:007 width=70% }

Создаем новый файл "lab8-2.asm" с помощью команды "touch".

Вводим в файл текст другой программы в соответствии с листингом 8.2. (рис. [-@fig:008]).

![Редактирование файла](image/8.jpg){ #fig:008 width=70% }

Создаем исполняемый файл программы и запускаем его, указав аргументы : "аргумент1 аргумент 2 'аргумент 3'" (рис. [-@fig:009]).

![Запуск исполняемого файла](image/9.jpg){ #fig:009 width=70% }

Создаем новый файл "lab8-3.asm" с помощью команды "touch".

Вводим в файл текст другой программы в соответствии с листингом 8.3. (рис. [-@fig:010]).

![Файл листинга "lab8-3.asm"](image/10.jpg){ #fig:010 width=70% }

Создаем новый исполняемый файл программы и запускаем его. Также проводим проверку. (рис. [-@fig:011]).

![Запуск исполняемого файла](image/11.jpg){ #fig:011 width=70% }

Изменяем в текст программы для вычисления произведения аргументов командной строки. (рис. [-@fig:012]).

![Редактирование файла](image/12.jpg){ #fig:012 width=70% }

Создаем новый исполняемый файл программы и запускаем его. Также проводим проверку. (рис. [-@fig:013]).

![Запуск исполняемого файла](image/13.jpg){ #fig:013 width=70% }

# Выполнение самостоятельной работы

Создаем новый файл "lab8-4.asm" с помощью команды "touch".

Напишите программу, которая находит сумму значений функции f(x) для x = x1, x2, ..., xn. Мой вариант - 11 (рис. [-@fig:014]).

![Редактирование файла](image/14.jpg){ #fig:014 width=70% }

Создаем исполняемый файл программы и запускаем его. Ответ верный. (рис. [-@fig:015]). 

![Запуск исполняемого файла](image/15.jpg){ #fig:015 width=70% }

# Выводы

Благодаря данной лабораторной работе я приобрела навыки написания программ с использованием циклов и обработкой аргументов командной строки.
