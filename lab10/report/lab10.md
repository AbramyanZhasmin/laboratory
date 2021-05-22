---
# Front matter
lang: ru-RU
title: "Oтчёт лабораторной работы №10"
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором emacs.

# Задание

– Сделать отчёт по лабораторной работе №10 в формате Markdown.

– В качестве отчёта предоставить отчёты в 3 форматах: pdf, docx и md (в архиве, поскольку он должен содержать скриншоты, Makefile и т.д.).



# Выполнение лабораторной работы

1. Открыли emacs (рисунок 1).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/1.jpg)

(рисунок 1)

2. Создали файл lab7.sh . Используя команду C-x C-f (рисунок 2).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/2.jpg)

(рисунок 2)

3. И внесём текст (рисунок 3):
#!/bin/bash
HELL=Hello
function hello {
LOCAL HELLO=World
echo $HELLO
}
echo $HELLO
hello


![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/3.jpg)

(рисунок 3)

4. Сохранили файл, используя сочетание команд C-x C-s.

5. Проделали с текстом стандартные процедуры редактирования, каждое действие должно осуществляться комбинацией клавиш:

(a) Вырезали одной командой целую строку С-k (рисунок 4).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/4.jpg)

(рисунок 4)

(b) Вставить эту строку в конец файла C-y (рисунок 5).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/5.jpg)

(рисунок 5)

(c) Выделили область текста, команда C-space (рисунок 6).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/6.jpg)

(рисунок 6)

(d) Скопировали область в буфер обмена M-w.

(e) Вставили область в конец файла (рисунок 7).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/7.jpg)

(рисунок 7)

(f) Вновь выделили эту область и вырезали ее C-w (рисунок 8).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/8.jpg)

(рисунок 8)

(g) Отмените последнее действие C-/ (рисунок 9).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/9.jpg)

(рисунок 9)

6. Научились использовать команды по перемещению курсора.

(a) Переместим курсор в начало строки C-a (рисунок 10).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/10.jpg)

(рисунок 10)

(b) Переместите курсор в конец строки C-e (рисунок 11).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/11.jpg)

(рисунок 11)

(c) Переместили курсор в начало буфера M-< (рисунок 12).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/12.jpg)

(рисунок 12)

(d) Переместили курсор в конец буфера M-> (рисунок 13).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/13.jpg)

(рисунок 13)

7. Управление буферами.

(a) Вывели список активных буферов на экран C-x C-b (рисунок 14).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/14.jpg)

(рисунок 14)

(b) Переместились в открытое окно C-x о со списком открытых буферов и переключились на другой буфер (рисунок 15).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/15.jpg)

(рисунок 15)

(c) Закройте это окно C-x 0 (рисунок 16).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/16.jpg)

(рисунок 16)

(d) Теперь вновь переключились между буферами, но уже без вывода их списка на экран C-x b (рисунок 17-18).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/17.jpg)

(рисунок 17)

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/18.jpg)

(рисунок 18)

8. Управление окнами.

(a) Поделили фрейм на 4 часть: разделили фрейм на два окна по вертикали C-x 3, а затем каждое из этих окон на две части по горизонтали C-x 2 (рисунок 19-20).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/19.jpg)

(рисунок 19)

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/20.jpg)

(рисунок 20)

(b) В каждом из четырех созданных окон откроем новый буфер (файл) и введём несколько строк текста (рисунок 21).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/21.jpg)

(рисунок 21)

9. Режим поиска

(a) Переключились в режим поиска и C-s найдите несколько слов, присутствующих в тексте (рисунок 22).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/22.jpg)

(рисунок 22)

(b) Переключились между результатами поиска, нажимая C-s (рисунок 23).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/23.jpg)

(рисунок 23)

(c) Вышли из режима поиска, нажав C-g.

(d) Перейдём в режим поиска и замены M-% ввели текст, который следует найти и заменить, нажали Enter, затем ввели текст для замены (рисунок 24).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/24.jpg)

(рисунок 24)

После того, как будут подсвечены результаты поиска нажали ! для подтверждения замены (рисунок 25).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/25.jpg)

(рисунок 25)

(e) Испробовали другой режим поиска, нажав M-s o. Он отличается от обычного поиска, тем что переводит курсор на конец найденного слова, а не выделяет его (рисунок 26).

![](/Users/klausm1996/Desktop/laboratory/lab10/report/image/26.jpg)

(рисунок 26)

# Контрольные вопросы:

1. Emacs представляет собой мощный экранный редактор текста, написанный на языке высокого уровня Elisp.

2. Для работы с emacs используется система меню и комбинаций клавиш. Используются сочетания c клавишами <ctrl> и <meta>. Сложности могут возникнуть так как на клавиатуре для IBM PC совместимых ПК клавиши <meta> нет, то вместо нее можно использовать <alt> или <esc>\verb . Для доступа к системе меню используйте клавишу F10.

3. В терминологии emacs’а буфер- это область где мы набираем текст, а окно область, которая объединяет открытые буферы.

4. Можно открыть больше 10 буферов в одном окне.

5. Создаются по умолчанию при запуске emacs:
% *GNU Emacs* 844 Fundamental *scratch* 191 Lisp Interaction %* *Messages* 5257 Messages % *Quail Completions* 0 Fundamental

6. Клавиши: Ctrl,C,Shift,\,] и <esc>,Ctrl,C Ctrl,Shift,\,]

7. Разделите фрейм на два окна по вертикали C-x 3, окно на две части по горизонтали C-x 2

8. В файле Emacs хранятся настройки редактора emacs.

9. Kнопка backspace( стереть букву ) = функции C-k и ее можно переназначить.

10. Emacs оказался намного удобнее. В нём больше функций, в нём интересно редактировать информацию.

# Выводы
Я познакомилась с операционной системой Linux. Получила практические навыки работы с редактором emacs.


