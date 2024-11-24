---
## Front matter
title: "Лабораторная работа No3"
subtitle: "Архитектура компьютера"
author: "Оушен Мухаммад Ламин"


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

## Содержание
- 1 Цель работы
- 2 Задание
- 3 Теоретическое введение
- 3.7 Контрольные вопросы для самопроверки 3-
- 4 Выполнение лабораторной работы 5-
- 5 Выводы

## Список таблиц


## Список иллюстраций

- 4.1 Рис переход в каталог.
- 4.2 Рис команда git pull.
- 4.3 Рис переход в каталог л.р.3
- 4.4 Рис команда make
- 4.5 Рис команда make clean
- 4.6 Рис команда gedit.
- 4.7 Рис содержание каталога image.
- 4.8 Рис загрузака на github.


## 1 Цель работы

Освоить процедуры оформления отчетов с помощью легковесного языка
разметки Markdown.


## 2 Задание

**1.** В соответствующем каталоге сделать отчёт по лабораторной работе No3 в
формате Markdown. В качестве отчёта необходимо предоставить отчёты в 3
форматах: pdf, docx и md.
**2.** Загрузить файлы на github.


## 3 Теоретическое введение

## 3.7 Контрольные вопросы для самопроверки 3-

**1. Что такое Markdown?**
Markdown — это легкий язык разметки, который позволяет форматировать
текст с помощью простых символов, делая его легко читаемым и
редактируемым.
**2. Как в Markdown задается начертание шрифтов?**
- **Курсив:** обрамление текста в одиночные звездочки или подчеркивания,
например, *курсив* или _курсив_.
- **Жирный:** обрамление текста в двойные звездочки или подчеркивания,
например, **жирный** или __жирный__.
- **Жирный курсив:** обрамление текста в три звездочки, например,
***жирный курсив***.
**3. Как в Markdown оформляются списки?
Ненумерованный список:** используется звездочка, плюс или дефис:
- Пункт 1
- Пункт 2
**Нумерованный список:** используются числа с точками:
1. Первый пункт
2. Второй пункт


**4. Как в Markdown оформляются изображения и ссылки на них?
Изображение:** ![Alt text](url_изображения)
**Ссылка:** [Текст ссылки](url_ссылки)
**5. Как в Markdown оформляются математические формулы и ссылки на
них?
-** Для отображения формул используйте знаки доллара:
- Внутри строки: $E=mc^2$
- На отдельной строке: $$E=mc^2$$


## 4 Выполнение лабораторной работы

**1.** Описываются проведённые действия, в качестве иллюстрации даётся ссылка
на иллюстрацию (рис. 4.1). 1. Откроем терминал 2. Перейдем в каталог курса
сформированный при выполнении лабораторной работы No

```
Рис. 4.1: переход в каталог
```
**2.** Обновим локальный репозиторий, скачав изменения из удаленного репозито-
рия с помощью команды git pull4.

```
Рис. 4.2: команда git pull
```
**3.** Перейдем в каталог с шаблоном отчета по лабораторной работе No 3

```
Рис. 4.3: переход в каталог л.р.
```
**4.** Проведем компиляцию шаблона с использованием Makefile. Для этого вве-
дем команду make.

```
Рис. 4.4: команда make
```

**5.** Удалим полученные файлы с использованием Makefile. Для этого введем
команду make clean. Проверим, что после этой команды файлы report.pdf и
report.docx были удалены.4.

```
Рис. 4.5: команда make clean
```
**6.** Откроем файл report.md c помощью любого текстового редактора, например
gedit. Внимательно изучим структуру этого файла.4.

```
Рис. 4.6: команда gedit
```
**7.** Заполним отчет и скомпилируем отчет с использованием Makefile. Прове-
рим корректность полученных файлов. (Обратим внимание, для коррект-
ного отображения скриншотов они должны быть размещены в каталоге
image)4.


```
Рис. 4.7:содержание каталога image
```
**8.** Загрузим файлы на Github.4.

```
Рис. 4.8: загрузака на github
```

## 5 Выводы

```
к концу лабораторной работы этой лабораторной работе мы узнали, как
использовать markdown для создания pdf-docx файлов быстрее иэффективнее.
```

