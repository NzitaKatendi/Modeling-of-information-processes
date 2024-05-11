---
# Front matter
lang: ru-RU
title: "Отчет по Лабораторной Работе № 5_1"
subtitle: "Компонентное моделирование. Scilab, подсистема xcos"
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

Построить с помощью x cos фигуры Лиссажу с различными значениями параметров.
 
---

# Выполнение лабораторной работы

Строим с помощью xcos формы Лиссажу со следующими параметрами:

1) A = B = 1, a = 2, b = 2, δ = 0; π/4; π/2; 3π/4; π;


## Задача 1


![Пример модели в xcos](image/image1.png){ #fig:001 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 2, δ = 0](image/image2.png){ #fig:002 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 2, δ = π/4](image/image3.png){ #fig:003 width=70% }

---


![Фигура Лиссажу: A = B = 1, a = 2, b = 2, δ = 3π/4](image/image4.png){ #fig:004 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 2, δ = π](image/image5.png){ #fig:005 width=70% }

---
Постройте с помощью xcos фигуры Лиссажу со следующими параметрами:

2) A = B = 1, a = 2, b = 4, δ = 0; π/4; π/2; 3π/4; π;

![Фигура Лиссажу: A = B = 1, a = 2, b = 4, δ = 0](image/image6.png){ #fig:006 width=70% }

---


![Фигура Лиссажу: A = B = 1, a = 2, b = 4, δ = π/4](image/image7.png){ #fig:007 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 4, δ = 3π/4](image/image8.png){ #fig:008 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 4, δ = π](image/image9.png){ #fig:009 width=70% }

---
Постройте с помощью xcos фигуры Лиссажу со следующими параметрами:

3) A = B = 1, a = 2, b = 6, δ = 0; π/4; π/2; 3π/4; π;

![Фигура Лиссажу: A = B = 1, a = 2, b = 6, δ = 0](image/image10.png){ #fig:010 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 6, δ = π/4](image/image11.png){ #fig:011 width=70% }

---

![Фигура Лиссажу: A = B = 1, a = 2, b = 6, δ = π/2](image/image12.png){ #fig:012 width=70% }

---
![Фигура Лиссажу: A = B = 1, a = 2, b = 6, δ = 3π/4](image/image13.png){ #fig:013 width=70% }

---
## Задача 2

Modelica – свободно распространяемый объектно-ориентированный язык для моделирования сложных физических систем. В основе языка Modelica лежит концепция соединяемых блоков. При соединении в соответствии с требуемой схемой
автоматически генерируются соответствующие уравнения.

Язык Modelica в чем-то похож на императивные объектно-ориентированные языки.
В нём есть выражения, классы, наследование, функции. В основу языка положена
конструкция «уравнение» (equation).

![Редактор OMEdit, окно редактирования кода модели](image/image14.png){ #fig:014 width=70% }

---

![Редактор OMEdit, построение графика](image/image15.png){ #fig:015 width=70% }

---

![ Редактор OMEdit, Simulation Setup](image/image16.png){ #fig:016 width=70% }

---

![Редактор OMEdit, построение графика при изменении параметров моделирования](image/image17.png){ #fig:017 width=70% }

---

![Редактор OMEdit, построение графика при изменении параметров моделирования](image/image18.png){ #fig:018 width=70% }

---

# Выводы

По мере выполнения данной работы я построил фигуры Лиссажу на xcos.