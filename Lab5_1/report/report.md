---
# Front matter
lang: ru-RU
title: "Отчет по Лабораторной Работе № 5"
subtitle: "Модель эпидемии (SIR)"
author: "Нзита Диатезилуа Катенди"

## Pdf output format
toc: true # Table of contents
toc-depth: 2
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
lofTitle: "Цель Работы"
lotTitle: "Ход Работы"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цели и задачи работы

## Цель лабораторной работы

Целью данной работы является построение модели эпидемии.
 
---

# Выполнение лабораторной работы

1. Зададим переменные окружения. beta=1,nu=.3

---

## Задача 1


![Задать переменные окружения в xcos](image/image1.png){ #fig:001 width=70% }

---
2. Сделаем блок-схему для моделирования.

![Модель SIR в xcos](image/image2.png){ #fig:002 width=70% }

---

![Задать начальные значения в блоках интегрирования](image/image3.png){ #fig:003 width=70% }

---

![Задать начальные значения в блоках интегрирования](image/image4.png){ #fig:004 width=70% }

---

![Задать конечное время интегрирования в xcos](image/image5.png){ #fig:005 width=70% }

---

![Эпидемический порог модели SIR 5.1 при β = 1, ν = 0.3](image/image6.png){ #fig:006 width=70% }

---

![Параметры блока Modelica для модели](image/image7.png){ #fig:007 width=70% }

---

![Параметры блока Modelica для модели](image/image8.png){ #fig:008 width=70% }

---

![Модель SIR в xcos с применением блока Modelica](image/image9.png){ #fig:009 width=70% }

---

![](image/image10.png){ #fig:010 width=70% }

---

![Реализуйте модель SIR в OpenModelica](image/image11.png){ #fig:011 width=70% }

---

![Редактор OMEdit, Simulation Setup](image/image12.png){ #fig:012 width=70% }

---
##  Задание для самостоятельного выполнения

В дополнение к предположениям, которые были сделаны для модели SIR (5.1), предположим, что учитываются демографические процессы, в частности, что смертность в популяции полностью уравновешивает рождаемость, а все рожденные индивидуумы появляются на свет абсолютно здоровыми. Тогда получим следующую систему
уравнений:

s˙ = −βs(t)i(t) + µ(N − s(t));
˙i = βs(t)i(t) − νi(t) − µi(t);
r˙ = νi(t) − µr(t),

где µ — константа, которая равна коэффициенту смертности и рождаемости.
Требуется:
– реализовать модель SIR с учётом процесса рождения / гибели особей в xcos (в
том числе и с использованием блока Modelica), а также в OpenModelica;
– построить графики эпидемического порога при различных значениях параметров
модели (в частности изменяя параметр µ);
– сделать анализ полученных графиков в зависимости от выбранных значений
параметров модели

1. xcos + modelica

![Реализуйте модель SIR в OpenModelica.](image/image13.png){ #fig:013 width=70% }

---
2. OpenModelica

![SIR](image/image14.png){ #fig:014 width=70% }

---

# Выводы

Мы реализовали модель "Хищник-жертва" в x cos, modelica и OpenModelica.