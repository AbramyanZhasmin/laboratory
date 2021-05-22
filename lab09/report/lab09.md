---
# Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе №9"
subtitle: "Дисциплина: Операционные системы"
author: "Абрамян Жасмин"

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

# Цель работы
Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию
практически во всех дистрибутивах.
# Задание
– Сделать отчёт по лабораторной работе №9 в формате Markdown.
– В качестве отчёта предоставить отчёты в 3 форматах: pdf, docx и md (в архиве, поскольку он должен содержать скриншоты, Makefile и т.д.).

# Выполнение лабораторной работы
##Задание 1

1. Создали каталог с именем ~/work/os/lab06. Использовали команду mkdir ~/work/os/lab06 (рисунок 1).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/1.jpg)

(рисунок 1)

2. Перешли во вновь созданный каталог, использовав команду cd~/work/os/lab06.
(рисунок 2).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/2.jpg)

(рисунок 2)

3. Вызвали Vi и создали файл hello.sh (рисунок 3).

![]/Users/klausm1996/Desktop/laboratory/lab09/report/image/3.jpg)

(рисунок 3)

4. Нажали клавишу i и ввели следующий текст (предоставленный в лаб.работе) (рисунок 4)
#!/bin/bash
HELL=Hello
function hello {
LOCAL HELLO=World
echo $HELLO
}
echo $HELLO
hello
![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/4.jpg)

(рисунок 4)

5. Нажали клавишу ESC для перехода в командный режим после
завершения ввода текста (рисунок 5).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/5.jpg)

(рисунок 5)

6. Нажали двоеточие (:) для перехода в режим последней строки и
внизу экрана появилось приглашение в виде двоеточия.

7. Затем Нажали w (записать) и q (выйти), а затем нажмём клавишу <RETURN> для сохранения текста и завершения работы (рисунок 6).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/6.jpg)

(рисунок 6)

8. Сделали файл исполняемым chmod +x hello.sh (рисунок 7)

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/7.jpg)

(рисунок 7)

##Задание 2

1. Вызвали Vi на редактирование файла vi ~/work/os/lab06/hello.sh (рисунок 8)

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/8.jpg)

(рисунок 8)

2. Установили курсор на конец слова HELL второй строки.

3.Затем перешли режим вставки и заменили на HELLO. Нажали <ESC>,чтобы вернуться в командный режим (рисунок 9).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/9.jpg)

(рисунок 9)

4. Установим курсор на четвертую строку и сотрём слово LOCAL (рисунок 10).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/10.jpg)

(рисунок 10)

5. Перешли в режим вставки и набрали текст: local нажали ESC, чтобы вернуться в командный режим (рисунок 11).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/11.jpg)

(рисунок 11)

6. Установили курсор на последней строке файла. Вставили после неё
строку, содержащую текст: echo $HELLO (рисунок 12)

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/12.jpg)

(рисунок 12)

7. Нажали <ESC>, чтобы перейти в командный режим.

8. Удалили последнюю строку (рисунок 13).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/13.jpg)

(рисунок 13)

9. Ввели команду отмены изменений u для отмены последней команды (рисунок 14).

![](/Users/klausm1996/Desktop/laboratory/lab09/report/image/14.jpg)

(рисунок 14)

10. Ввели символ: (двоеточие) для перехода в режим последней строки. Записали произведенные изменения на диск и вышли из vi (рисунок 15)

![](/Users/klausm1996/Desktop/laboratory/lab09/image/15.jpg)

(рисунок 15)

# Контрольные вопросы:

1. Командный режим позволяет управлять курсором и вводить команды редактирования.
Режим вставки допускает производить ввод текста. При этом текст не будет восприниматься, как команды редактирования.
Режим последней строки позволяет производить запись файла на диск и выходить из редактора Vi. Кроме того, используя этот режим, можно вводить дополнительные команды редактирования.

2. Если необходимо просто выйти Vi (без сохранения выполненных изменений), то необходимо в последней строке набрать символ q (или q!).

3. 0 (ноль) - перейти в начало строки;
$ - перейти в конец строки;
G - перейти в конец файла;
nG - перейти на строку номер n.

4. Редактор vi предполагает, что слово - это строка символов, которая может включать в себя буквы, цифры и символы подчеркивания.

5. 0 (ноль) - перейти в начало строки;
$ - перейти в конец строки;

6. Добавление / вставка текста 
   а- добавить текст после курсора;
А- добавить текст в конец строки;
i- вставить текст перед курсором;
ni- вставить текст n раз;
I- вставить текст в начало строки.
Вставка строки
o-вставить строку под курсором;
О- вставить строку над курсором.
Удаление текста





# Выводы

Я познакомилась с операционной системой Linux. Получила практические навыки работы с редактором vi, установленным по умолчанию
практически во всех дистрибутивах.
