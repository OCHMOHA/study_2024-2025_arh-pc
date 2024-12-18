---
## Front matter
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ No 2"
subtitle: "дисциплина: Архитектура компьютера"
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
---


### МОСКВА

```
2024 г.
```

## Содержание


# Список таблиц

```
3.1 Описание некоторых каталогов файловой системы GNU Linux.......... 3
```

## Список иллюстраций

- 1 Цель работы......................................................................................................................................
- 2 Задание...............................................................................................................................................
- 3 Теоретическое введение..................................................................................................................
- 4 Выполнение лабораторной работы...............................................................................................
- 5 Выводы............................................................................................................................................
- 4.1 профиль на github
- 4.2 user.name и user.email
- 4.3 настройка utf-
- 4.4 имя начальной ветки
- 4.5 параметр autocrlf
- 4.6 параметр safecrlf
- 4.7 команда ssh-keyget - C
- 4.8 копия ключа
- 4.9 загрузка сгенерированного ключа
- 4.10создание каталога
- 4.11 создание репозиторий на основе шаблона
- 4.12 репозиторий study_2024–2025_arh- pc
- 4.13 переход в каталог
- 4.14 ssh для клонирования
- 4.15 команда git clone
- 4.16 переход в каталог
- 4.17 удаление лишних каталогов
- 4.18 создание необходимых каталогов
- 4.19 отправка файлов
- 4.20отправка файлов
- 4.21 отправка файлов
- 4.22иерархия
- 4.23загрузка предыдущей работы
- 4.24загрузка предыдущей работы


## 1 Цель работы......................................................................................................................................

```
Изучить идеологию и применение средств контроля версий. Приобрести
практические навыки по работе с системой git.
```

## 2 Задание...............................................................................................................................................

1. Создать отчет по выполнению лабораторной работы в соответствующем
    каталоге рабочего пространства (labs>lab02>report).
2. Скопировать отчеты по выполнению предыдущих лабораторных работ в
    соответствующие каталоги созданного рабочего пространства.
3. Загрузить файлы на github.


## 3 Теоретическое введение..................................................................................................................

```
Например, в табл. 3.1 приведено краткое описание стандартных
каталогов Unix.
```
```
Таблица 3.1: Описание некоторых каталогов файловой системы GNU
Linux
Имя
ка-
талога
```
```
Описание каталога
```
/ Корневая директория, содержащая всю файловую
/bin Основные системные утилиты, необходимые как в
однопользовательском режиме, так и при обычной работе
всем пользователям
/etc Общесистемные конфигурационные файлы и файлы
конфигурации установленных программ
/home Содержит домашние директории пользователей, которые, в
свою очередь, содержат персональные настройки и данные
пользователя
/media Точки монтирования для сменных носителей
/root Домашняя директория пользователя root
/tmp Временные файлы
/usr Вторичная иерархия для данных пользователя
Более подробно про Unix см. в [1–4].


## 4 Выполнение лабораторной работы...............................................................................................

```
2.4.1.Настройка github На сайте https://github.com/ создаем учётную
запись и заполняем основные данные. (Рис.4.1)
```
```
Рис. 4.1: профиль на github
```
```
2.4.2. Базовая настройка git Сначала сделаем предварительную
конфигурацию git. Откроем терминал и введем следующие команды,
указав свое имя и email репозитория:(Рис.4.2)
```
Рис. 4.2: user.name и user.email
При выполнении команды git config происходит изменение текстового
файла конфигурации. Добавляем опцию –global для того, чтобы GРис.
создание репозиторий на основе шаблонаit использовал эти данные в


дальнейшем для всех наших действий. Настроим utf-8 в выводе
сообщений git: (Рис.4.3)

```
Рис. 4.3: настройка utf- 8
```
```
имя начальной ветки :(Рис.4.4)
```
```
Рис. 4.4: имя начальной ветки
Параметр autocrlf :(Рис.4.5)
```
```
Рис. 4.5: параметр autocrlf
```
Параметр safecrlf:(Рис.4.6)

```
Рис. 4.6: параметр safecrlf
```
```
2.4.3.Создание SSH ключа Для последующей идентификации на сервере
репо- зиториев нужно сгенерировать пару ключей :(Рис.4. 7 )
```

```
Рис. 4.7: команда ssh-keyget - C
```
Далее необходимо загрузить сгенерированный открытый (.pub) ключ.
Зай- дем на сайт [http://github.org/](http://github.org/) под своей учётной записью и перейдем
в меню Setting. После этого выберем в боковом меню SSH and GPG keys
и нужно нажать кнопку New SSH key. Скопируем из локальной консоли
ключ в буфер обмена (cat~/.ssh/id_rsa.pub | xclip -sel clip) вставляем ключ в
появившееся на сайте поле и указываем для ключа имя (Title).(Рис.4.8)
(Рис.4.9)

```
Рис. 4.8: копия ключа
```

```
Рис. 4.9: загрузка сгенерированного ключа
```
2.4.4.Откройем терминал и создадим каталог для предмета
«Архитектура компьютера»:(Рис.4.10)

```
Рис. 4.10: создание каталога
```
```
2.4.5. Перейдем на станицу репозитория с шаблоном курса
https://github.com/yamadharma/course-directory-student- template.
(Рис.4.11) Далее выберите Use this template.
```

```
Рис. 4.11: создание репозиторий на основе шаблона
```
В открывшемся окне задаём имя репозитория study_2024–2025_arh-pc и
созда- ём репозиторий (кнопка Create repository from template).(Рис.4.12)

```
Рис. 4.12: репозиторий study_2024–2025_arh-pc
Откроем терминал и перейдём в каталог курса:(Рис.4.13)
```

```
Рис. 4.13: переход в каталог
```
Клонирую созданный репозиторий:(Рис.4.14)(Рис.4.15)

```
Рис. 4.14: ssh для клонирования
```

```
Рис. 4.15: команда git clone
```
2.4.6 Настройка каталога курса Перейдём в каталог курса:(Рис.4.16)

```
Рис. 4.16: переход в каталог
```

```
Удалим лишние каталоги:(Рис.4.17)
```
```
Рис. 4.17: удаление лишних каталогов
```
```
Создадим необходимые каталоги:(Рис.4.18)
```
```
Рис. 4.18: создание необходимых каталогов
```
Отправляем файлы на сервер (прикрепляю не все скриншоты):
(Рис.4.19)(Рис.4.20)(Рис.4.21)


Рис. 4.19: отправка файлов


Рис. 4.20: отправка файлов


```
Рис. 4.21: отправка файлов
```
Проверяем правильность создания иерархии рабочего пространства в
локаль- ном репозитории на странице github:(Рис.4.22)

```
Рис. 4.22: иерархия
```

2.5. Задание для самостоятельной работы Загрузжаем файлы на github.
(Рис.4.23)(Рис.4.24)

```
Рис. 4.23: загрузка предыдущей работы
```
```
Рис. 4.24: загрузка предыдущей работы
```
```
По аналогии поступаем и со второй работой.
```

# Выводы

В ходе лабораторной работы мы приобрели практические навыки по работе с
системой git. и Мы научились использовать репозиторий.

