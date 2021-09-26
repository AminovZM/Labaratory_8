---
# Front matter
lang: ru-RU
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №8"
subtitle: "Задача на собственные значения"
author: "Аминов Зулфикор Мирзокаримович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---


# Ход работы:

Включим журналирование

![рисунка 1](img/1/1.PNG){ #fig:001 width=70% }

# Собсственные значения и собственные векторы

Зададим матрицу

![рисунка 2](img/1/2.PNG){ #fig:001 width=70% }
![рисунка 3](img/1/3.PNG){ #fig:001 width=70% }
![рисунка 4](img/1/4.PNG){ #fig:001 width=70% }

Умножаем матрицу на транспонированную матрицу

![рисунка 5](img/1/5.PNG){ #fig:001 width=70% }
![рисунка 6](img/1/6.PNG){ #fig:001 width=70% }
![рисунка 7](img/1/7.PNG){ #fig:001 width=70% }

# Марковские цепи

Сформируем матрицу переходов

![рисунка 8](img/2/1.PNG){ #fig:001 width=70% }

Вероятности будущего состояния легко вычисляются как T^k*x, где x - начальный вектор вероятностей.

![рисунка 9](img/2/2.PNG){ #fig:001 width=70% }
![рисунка 10](img/2/3.PNG){ #fig:001 width=70% }

Найдем вектор равновесного состояния для цепи Маркова с переходной матрицей

![рисунка 11](img/2/4.PNG){ #fig:001 width=70% }
![рисунка 12](img/2/5.PNG){ #fig:001 width=70% }
![рисунка 13](img/2/6.PNG){ #fig:001 width=70% }

Таким образом, x = (0.37631 0.29287 0.33.82) является вектором равновесного состояния. Проверим это.

![рисунка 14](img/2/7.PNG){ #fig:001 width=70% }

Выключим журналирование.

![рисунка 15](img/2/8.PNG){ #fig:001 width=70% }

# Вывод

Научился работать с задачой на собственные значения в Octave.
