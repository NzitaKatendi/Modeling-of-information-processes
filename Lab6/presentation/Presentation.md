---
## Front matter
title: "Презентация по лабораторной работе № 6"
subtitle: "Модель «хищник–жертва"
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

Целью данной работы является построение модели «хищник-жертва».
 
---

# Выполнение лабораторной работы

1. Зафиксируем начальные данные: a = 2, b = 1, c = 0, 3, d = 1, x(0) = 2, y(0) = 1.
В меню Моделирование, Задать переменные окружения зададим значения коэффициентов a, b, c, d


## Задача 1


![Задать переменные окружения в xcos для модели](image/image1.png){ #fig:001 width=70% }

---

![Модель «хищник–жертва» в xcos](image/image2.png){ #fig:002 width=70% }

---

![Динамика изменения численности хищников и жертв модели при a = 2, b = 1, c = 0, 3, d = 1, x(0) = 2, y(0) = 1 ](image/image3.png){ #fig:003 width=70% }

---

![Фазовый портрет модели 6.1 при a = 2, b = 1, c = 0, 3, d = 1, x(0) = 2, y(0) = 1](image/image4.png){ #fig:004 width=70% }

---

![Модель «хищник–жертва» в xcos с применением блока Modelica](image/image5.png){ #fig:005 width=70% }

---

![Параметры блока Modelica для модели](image/image6.png){ #fig:006 width=70% }

Запустив, получим аналогичный график как в пункте 3.
Перейдем к реализации на OpenModelica.

---
##  Задание для самостоятельного выполнения

Упражнение. Реализуйте модель «хищник – жертва» в OpenModelica. Постройте
графики изменения численности популяций и фазовый портрет

1. xcos + modelica

![](image/image7.png){ #fig:007 width=70% }

---

![Динамика изменений отдельных хищников и жертвенных моделей в OpenModelica](image/image8.png){ #fig:008 width=70% }

---
2. OpenModelicq

![Фазовый портрет модели в OpenMadelica](image/image9.png){ #fig:009 width=70% }

---

# Выводы

Мы реализовали модель "Хищник-жертва" в xcos, modelica и OpenModelica.