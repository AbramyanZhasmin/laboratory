---
# Front matter
lang: ru-RU
title: "Отчёт лабораторной работы №5"
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

Приобретение практических навыков взаимодействия пользователя с системой
посредством командной строки.

# Задание

– Сделать отчёт по предыдущей лабораторной работе в формате Markdown.

– В качестве отчёта предоставить отчёты в 3 форматах: pdf, docx и md (в архиве, поскольку он должен содержать скриншоты, Makefile и т.д.).

# Выполнение лабораторной работы

1. Определяю полное имя моего домашнего каталога, используя команду `pwd`.

![](/Users/klausm1996/Desktop/laboratory/lab09/image/1.jpg)

(Рисунок 1)

2. Выполняю следующие действия:
  
2.1. Перехожу в каталог /tmp (Рисунок 2).

![](/Users/klausm1996/Downloads/лаба5/2.jpg)

(Рисунок 2)

2.2. Вывожу на экран содержимое каталога /tmp. Рисунок 4). Чтобы вывести на экран подробную информацию о файлах и каталогах, необходимо использовать опцию `l` (Рисунок 5).

![](/Users/klausm1996/Downloads/лаба5/3.jpg)

(Рисунок 3)

![](/Users/klausm1996/Downloads/лаба5/4.jpg)

(Рисунок 4)

![](/Users/klausm1996/Downloads/лаба5/5.jpg))

(Рисунок 5)

2.3. Определяю, есть ли в каталоге /var/spool подкаталог с именем cron. Для этого использую команду `ls -F`, что позволяет определить тип файла cron и убедиться в том, что это каталог (Рисунок 6).

![](/Users/klausm1996/Downloads/лаба5/6.jpg)

(Рисунок 6)

2.4. Перехожу в мой домашний каталог и вывожу на экран его содержимое.(Рисунок 7).

![](/Users/klausm1996/Downloads/лаба5/7.jpg)

(Рисунок 7)

3. Выполняю следующие действия:
   
3.1. В домашнем каталоге создаю новый каталог с именем newdir (Рисунок 8):

![](/Users/klausm1996/Downloads/лаба5/8.jpg)

(Рисунок 8)

3.2. В каталоге ~/newdir создаю новый каталог с именем morefun (Рисунок 9):

![](/Users/klausm1996/Downloads/лаба5/9.jpg)

(Рисунок 9)

3.3. В домашнем каталоге создаю одной командой три новых каталога с именами letters, memos, misk. Затем удаляю эти каталоги одной командой (Рисунок 10).

![](/Users/klausm1996/Downloads/лаба5/10.jpg)

(Рисунок 10)

3.4. Попробую удалить ранее созданный каталог ~/newdir командой `rm`. Проверяю, был ли каталог удалён.

![](/Users/klausm1996/Downloads/лаба5/11.jpg)

(Рисунок 11)

3.5. Удаляю каталог ~/newdir/morefun из домашнего каталога. Проверяю,
был ли каталог удалён.(Рисунок 12)

![](/Users/klausm1996/Downloads/лаба5/12.jpg)

(Рисунок 12)

4. С помощью команды man определяю, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него. (Рисунок 13)

![](/Users/klausm1996/Downloads/лаба5/13.jpg)

(Рисунок 13)
5. С помощью команды man определяю набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого
каталога с развёрнутым описанием файлов.

6. Использую команду man для просмотра описания следующих команд: cd, pwd,
mkdir, rmdir, rm. (Рисунок 14-18)

![](/Users/klausm1996/Downloads/лаба5/14.jpg)

(Рисунок 14)

![](/Users/klausm1996/Downloads/лаба5/15.jpg)

(Рисунок 15)

![](/Users/klausm1996/Downloads/лаба5/16.jpg)

(Рисунок 16)

![](/Users/klausm1996/Downloads/лаба5/17.jpg)

(Рисунок 17)

![](/Users/klausm1996/Downloads/лаба5/18.jpg)

(Рисунок 18)
7. Используя информацию, полученную при помощи команды history, выполняю
модификацию и исполнение нескольких команд из буфера команд.(Рисунок 19-24)

![](/Users/klausm1996/Downloads/лаба5/19.jpg)

(Рисунок 19)

![](/Users/klausm1996/Downloads/лаба5/20.jpg)

(Рисунок 20)

![](/Users/klausm1996/Downloads/лаба5/21.jpg)

(Рисунок 21)

![](/Users/klausm1996/Downloads/лаба5/22.jpg)

(Рисунок 22)

![](/Users/klausm1996/Downloads/лаба5/23.jpg)

(Рисунок 23)

![](/Users/klausm1996/Downloads/лаба5/24.jpg)

(Рисунок 24)

# Контрольные вопросы

1) Командная строка – специальная программа, позволяющая управлять
операционной системой при помощи текстовых команд, вводимых в
окне приложения.

2) Для определения абсолютного пути к текущему каталогу используется
команда pwd (print working directory). Например, команда `pwd` в
моем домашнем каталоге выведет: /home/dvkasjyanov (Рисунок 1).

3) Команда `ls -F` (или `ls -aF`, тогда появятся еще скрытые файлы)
выведет имена файлов в текущем каталоге и их типы.
Тип каталога обозначается /, тип исполняемого файла обозначается *,
тип ссылки обозначается @.

1) Имена скрытых файлов начинаются с точки. Для того, чтобы отобразить имена
скрытых файлов, необходимо использовать команду `ls –a`.

5) Команда rm используется для удаления файлов и/или каталогов.
Команда `rm -i` выдает запрос подтверждения на удаление файла.
Команда `rm -r` необходима, чтобы удалить каталог, содержащий файлы.
Без указания этой опции команда не будет выполняться. Если каталог
пуст, то можно воспользоваться командой `rmdir`. Если удаляемый
каталог содержит файлы, то команда не будет выполнена – нужно
использовать `rm -r имя_каталога`.
Таким образом, каталог, не содержащий файлов, можно удалить и
командой `rm`, и командой `rmdir`. Файл командой `rmdir` удалить нельзя.

6) Чтобы определить, какие команды выполнил пользователь в сеансе
работы, необходимо воспользоваться командой `history`.

7) Чтобы исправить или запустить на выполнение команду, которую
пользователь уже использовал в сеансе работы, необходимо: в первом
случае: воспользоваться конструкцией
`!<номер_команды>:s/<что_меняем>/<на_что_меняем>`, во втором
случае: `!<номер_команды>`. 

8) Чтобы записать в одной строке несколько команд, необходимо между
ними поставить ; . Например, `cd /tmp; ls`.

9) Символ обратного слэша \ позволяет использовать управляющие
символы ( ".", "/", "$", "*", "[", "]", "^", "&") без их интерпретации
командной оболочкой; процедура добавления данного символа перед
управляющими символами называется экранированием символов.
Например, команда `ls newdir\/morefun` отобразит содержимое
каталога newdir/morefun.

10) Команда `ls -l` отображает список каталогов и файлов с подробной
информацией о них (тип файла, право доступа, число ссылок,
владелец, размер, дата последней ревизии, имя файла или каталога).

11) Полный, абсолютный путь от корня файловой системы – этот путь
начинается от корня "/" и описывает весь путь к файлу или каталогу;
Относительный путь – это путь к файлу относительно текущего
каталога (каталога, где находится пользователь). Например, `cd
/newdir/morefun` – абсолютный путь; 
`cd newdir` – относительный путь.

12) Чтобы получить необходимую информацию о команде, необходимо
воспользоваться конструкцией `man [имя_команды]`, либо использовать
опцию `help`, которая предусмотрена для некоторых команд.

13) Для автоматического дополнения вводимых команд служит клавиша
Tab.

# Выводы

Я приобрела практические навыки взаимодействия пользователя с системой
посредством командной строки.