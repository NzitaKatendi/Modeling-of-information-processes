---
## Front matter
title: "Презентация по лабораторной работе № 5"
subtitle: "Модель эпидемии (SIR)"
author: " Нзита Диатезилуа Катенди"

## Generic otions
lang: ru-RU

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes:
- \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
- '\makeatletter'
- '\beamer@ignorenonframefalse'
- '\makeatother'
aspectratio: 43
section-titles: true
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Нзита Диатезилуа Катенди
  * студент группы НКНбд-01-21
  * Российский университет дружбы народов
  * <https://github.com/NzitaKatendi/Modeling-of-information-processes>

:::
::: {.column width="30%"}



:::
::::::::::::::

# Цели и задачи работы

## Цель лабораторной работы

Целью данной работы является построение модели эпидемии.
 
---

# Выполнение лабораторной работы

1. Зададим переменные окружения. beta=1,nu=.3


## Задача 1


![Задать переменные окружения в xcos](image/image1.png){ #fig:001 width=70% }

---
2. Сделаем блок-схему для моделирования.

![Модель SIR в xcos](image/image2.png){ #fig:002 width=70% }

---

3. Запустив, получим следующий график.

![](image/image3.png){ #fig:003 width=70% }

---

4. Дальше сделаем аналогичную схему на х cos с применением
modelica. Для этого сделаем следующую схему.

![Модель SIR в xcos и modelica](image/image4.png){ #fig:004 width=70% }

---

5. Запустив, получим аналогичный график как в пункте 3.
6. Перейдем к реализации на OpenModelica.

![Реализуйте модель SIR в OpenModelica](image/image5.png){ #fig:005 width=70% }

---

![Эпидемический порог модели SIR при В = 1, v = 0.3](image/image6.png){ #fig:006 width=70% }

---
##  Задание для самостоятельного выполнения

1. xcos + modelica

![](image/image7.png){ #fig:007 width=70% }

---

![Редактор OMEdit, Simulation Setup](image/image8.png){ #fig:008 width=70% }

---
2. OpenModelicq

![SIR](image/image9.png){ #fig:009 width=70% }

---

# Выводы

Мы реализовали модель "Хищник-жертва" в x cos, modelica и OpenModelica.