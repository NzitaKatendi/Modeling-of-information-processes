---
# Front matter
lang: ru-RU
title: "Отчет по Лабораторной Работе № 7"
subtitle: "Модель M|M|1|∞"
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

Целью данной работы является построение модели M|M|1|∞.
 
---

# Выполнение лабораторной работы

Рассмотрим пример моделирования в xcos системы массового обслуживания типа
M|M|1|∞.

Зафиксируем начальные данные: λ = 0, 3, µ = 0, 35, z0 = 6. Суперблок, моделирующий поступление заявок, представлен на рис. 1


## Задача 1


![Суперблок, моделирующий поступление заявок](image/image1.png){ #fig:001 width=70% }

---
Суперблок, моделирующий процесс обработки заявок, представлен на рис. 2

![Суперблок, моделирующий поступление заявок](image/image2.png){ #fig:002 width=70% }

---

Готовая модель M|M|1|∞ представлена на риc. 3

![Модель M|M|1|∞ в xcos](image/image3.png){ #fig:003 width=70% }

---

Результат моделирования представлен на рис. 4 и 5

![Поступление ( — ) и обработка (– · · – ) заявок](image/image4.png){ #fig:004 width=70% }

---

![Динамика размера очереди](image/image5.png){ #fig:005 width=70% }

---

# Выводы

Реализуем построение модели M|M|1|∞ в xcos.