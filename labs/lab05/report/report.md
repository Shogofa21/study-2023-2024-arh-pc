---
## Front matter
title: "Шаблон отчёта по лабораторной работе 04"
subtitle: "Простейший вариант"
author: "Абдуллахи шугофа"

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
Приобретение практических навыков работы в Midnight Commander. Освоение инструкций языка ассемблера mov и int.

# Задание

2 Порядок выполнения лабораторной работы

2.1 Задание 1:
Откроем Midnight Commander (рис. [2.1])

![Открываем Midnight Commander](/labs/lab05/report/image/1.png){#fig:fig1 width=70% }

2.2 Задание 2:

Пользуясь клавишами � , � и Enter перейдем в каталог ~/work/arch-pc, созданный при выполнении лабораторной работы No4 (рис. [2.2])

![Переход в другой каталог](/labs/lab05/report/image/2.png){#fig:fig1 width=70% }

2.3 Задание 3:
С помощью функциональной клавиши F7 создадим папку lab05 (рис. [2.3]) и перейдем в созданный каталог (рис. [2.4])

![Создание каталога](/labs/lab05/report/image/3.png){#fig:fig1 width=70% }

![Переход в созданный каталог](/labs/lab05/report/image/4.png){#fig:fig1 width=70% }

2.4 Задание 4:

Пользуясь строкой ввода и командой touch создадим файл lab5-1.asm (рис. [2.5])

![Создание файла](/labs/lab05/report/image/5.png){#fig:fig1 width=70% }

2.5 Задание 5:

С помощью функциональной клавиши F4 откроем файл lab5-1.asm для редактирова- ния во встроенном редакторе (рис. [2.6])

![Переход во встроенный редактор](/labs/lab05/report/image/6.png){#fig:fig1 width=70% }

2.6 Задание 6:

Введем текст программы из листинга, сохраним изменения и закроем файл (рис. [2.7])

![Ввод текста программы](/labs/lab05/report/image/7.png){#fig:fig1 width=70% }

2.7 Задание 7

С помощью функциональной клавиши F3 откроем файл lab5-1.asm для просмотра. Убедимся, что файл содержит текст программы (рис. [2.8])

![Открытие файла](/labs/lab05/report/image/8.png){#fig:fig1 width=70% }

2.8 Задание 8:

Оттранслируем текст программы lab5-1.asm в объектный файл (рис. [2.9]). Выполним компоновку объектного файла (рис. [2.10]) и запустим получившийся исполняемый файл (рис. [2.11]). Программа выводит строку ‘Введите строку:’ иожидает ввода с клавиатуры. На запрос введу свои ФИО (рис. [2.12])

![Оттранслирование текста программы](/labs/lab05/report/image/9.png){#fig:fig1 width=70% }

![](/labs/lab05/report/image/10.png){#fig:fig1 width=70% }

![Выполнение компановки](/labs/lab05/report/image/11.png){#fig:fig1 width=70% }

![](/labs/lab05/report/image/12.png){#fig:fig1 width=70% }

![Запуск файла](/labs/lab05/report/image/13.png){#fig:fig1 width=70% }

![Ввод с клавиатуры](/labs/lab05/report/image/14.png){#fig:fig1 width=70% }

3 Подключение внешнего файла
in_out.asm

3.1 Задание 9:

Скачаем файл in_out.asm со страницы курса в ТУИС (рис. [3.1])

![Скачивание файла с ТУИС](/labs/lab05/report/image/15.png){#fig:fig1 width=70% }

3.2 Задание 10:

Копируем подключаемый файл in_out.asm в каталог lab05 (рис. [3.2])

![Копирование файла](/labs/lab05/report/image/16.png){#fig:fig1 width=70% }

![](/labs/lab05/report/image/17.png){#fig:fig1 width=70% }

3.3 Задание 11:

С помощью функциональной клавиши F6 создам копию файла lab5-1.asm сименем lab5-2.asm (рис. [3.3])

![Создание копии файла](/labs/lab05/report/image/18.png){#fig:fig1 width=70% }

![](/labs/lab05/report/image/19.png){#fig:fig1 width=70% }

3.4 Задание 12

Исправим текст программы в файле lab5-2.asm с использованием подпрограмм из внешнего файла in_out.asm в соответствии с листингом (рис. [3.4]). Создам испольняемый файл и проверю его работу (рис. [3.5])

![Исправление текста](/labs/lab05/report/image/21.png){#fig:fig1 width=70% }

![Проверка работы](/labs/lab05/report/image/22.png){#fig:fig1 width=70% }

3.5 Задание 13:

В файле lab5-2.asm заменим подпрограмму sprintLF на sprint (рис. [3.6]). Создадим исполняемый файл и проверим его работу (рис. [3.7]). Разница состоит вотступе после заранее написанной фразы и нашим вводом

![Изменение файла](/labs/lab05/report/image/23.png){#fig:fig1 width=70% }

![Запуск файла](/labs/lab05/report/image/24.png){#fig:fig1 width=70% }

4 Задание для самостоятельной работы

4.1 Задание 1:

Создадим копию файла lab5-1.asm и назовем lab5-3.asm (рис. [4.1]). Внесем изменения в программу (без использования внешнего файла in_out.asm), так чтобы она работала по определенному алгоритму

![](/labs/lab05/report/image/25.png){#fig:fig1 width=70% }

![Открытие копии файла](/labs/lab05/report/image/26.png){#fig:fig1 width=70% }

4.2 Задание 2:

Получим исполняемый файл и проверим его работу. На приглашение ввести строку введу свою фамилию (рис. [4.2]).

![Конвертирование и запуск программы](/labs/lab05/report/image/27.png){#fig:fig1 width=70% }


4.3 Задание 3:

Создадим копию файла lab5-2.asm и назовем lab5-4.asm. Исправим текст программы с использование подпрограмм из внешнего файла in_out.asm, так чтобы она работала по заданному алгоритму (рис. [4.3]).

![](/labs/lab05/report/image/28.png){#fig:fig1 width=70% }

![Создании копии файла](/labs/lab05/report/image/29.png){#fig:fig1 width=70% }

4.4 Задание 4:

Создадим исполняемый файл и проверим его работу (рис. [4.4]).

![Проверяем работу](/labs/lab05/report/image/30.png){#fig:fig1 width=70% }

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. @tbl:std-dir приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. @fig:001).

![Название рисунка](image/placeimg_800_600_tech.jpg){#fig:001 width=70%}

# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
