Третий семестр
================


Первый модуль
--------------

***A.*** Найдите все вхождения шаблона в строку. Длина шаблона – p, длина строки – n. Время O(n + p), доп. память – O(p). p ≤ 30000, n ≤ 300000. С помощью z-функции <br/>
**Формат входных данных.** Шаблон, символ перевода строки, строка.<br/>
**Формат выходных данных.** Позиции вхождения шаблона в строке.

***B.*** Строка называется палиндромом, если она одинаково читается как слева направо, так и справа налево. Например, «abba» – палиндром, а «roman» – нет.
Для заданной строки s длины n (1 ≤ n ≤ 10**5) требуется подсчитать число пар (i, j), 1 ≤ i < j ≤ n, таких что подстрока s[i..j] является палиндромом.<br/>
**Формат входных данных.** Входной файл содержит одну строку s длины n, состоящюю из маленьких латинских букв.<br/>
**Формат выходных данных.** В выходной файл выведите искомое число подстрок-палиндромов.

***C.*** Шаблон поиска задан строкой длины m, в которой кроме обычных символов могут встречаться символы “?”. Найти позиции всех вхождений шаблона в тексте длины n. Каждое вхождение шаблона предполагает, что все обычные символы совпадают с соответствующими из текста, а вместо символа “?” в тексте встречается произвольный символ. Гарантируется, что сам “?” в тексте не встречается.<br/>
Время работы - O(n + m + Z), где Z - общее число вхождений подстрок шаблона “между вопросиками” в исходном тексте. m ≤ 5000, n ≤ 2000000.<br/>
**Формат входных данных.** Первая строка – шаблон, который нужно найти, с джокерами, вторая строка – текст.<br/>
**Формат выходных данных.** В одну строку все позиции вхождения.

***D.*** Дана строка длины n. Найти количество ее различных подстрок. Используйте суффиксный массив.
Построение суффиксного массива выполняйте за O(n log n). Вычисление количества различных подстрок выполняйте за O(n). <br/>
**Формат входных данных.** Строка.<br/>
**Формат выходных данных.** Число - количество различных подстрок.

***E.*** Даны строки s и t. Постройте сжатое суффиксное дерево, которое содержит все суффиксы строки s и строки t. Найдите такое дерево, которое содержит минимальное количество вершин.<br/>
**Формат входных данных.** В первой строке записана строка s (1 ≤ |s| ≤ 10^5), последний символ строки равен `$`, остальные символы строки — маленькие латинские буквы.
Во второй строке записана строка t (1 ≤ |t| ≤ 10**5), последний символ строки равен `#` , остальные символы строки — маленькие латинские буквы.<br/>
**Формат выходных данных.** Пронумеруйте вершины дерева от 0 до n-1 в порядке обхода в глубину, обходя поддеревья в порядке лексикографической сортировки исходящих из вершины ребер. Используйте ASCII-коды символов для опре- деления их порядка.
В первой строке выведите целое число n — количество вершин дерева. В следующих n-1 строках выведите описание вершин дерева, кроме корня, в порядке увеличения их номеров.
Описание вершины дерева v состоит из четырех целых чисел: p, w, lf, rg, где p (0 ≤ p < n, p ≠ v) — номер родителя текущей вершины, w (0 ≤ w ≤ 1) — номер строки для определения подстроки на ребре. Если w = 0, то на ребре, ведущем из p в v, написана подстрока s[lf … rg - 1] (0 ≤ lf < rg ≤ |s|). Если w = 1, то на ребре, ведущем из p в v, написана подстрока t[lf … rg -1] (0 ≤ lf < rg ≤ |t|).

***F.*** Заданы две строки s, t и целое число k. Рассмотрим множество всех таких непустых строк, которые встречаются как подстроки в s и t одновременно. Найдите k-ую в лексикографическом порядке строку из этого множества.<br/>
**Формат входных данных.** В первых двух строках записаны строки s и t (1 ≤ |s|, |t| ≤ 10^5). В третьей строке записано целое число k (1 ≤ k ≤ 10^18). Строки состоят из маленьких латинских букв.<br/>
**Формат выходных данных.** В первой строке выведите искомую строку или -1, если такой не существует.


Второй модуль
--------------

***A.*** В своем сне Арсений добился многих успехов в строительстве. Теперь ему вручили в руки карту и сказали построить трассу от точки A до точки B. Арсений бы и рад помочь, но есть небольшая проблема — реки, которые опять же протекают строго напрямую от одной до другой точки, так как чтобы провести трассу через них, придется строить мосты. Помогите Арсению посчитать, сколько мостов ему придется построить.<br/>
**Формат входных данных.** В первой строке вводятся координаты точек A и B — начала и конца трассы. Во второй строке вводится количество рек N. В следующих N строках записаны координаты начала и конца реки. Все координаты целые и лежат от 0 до 10^5, рек не более 30000.<br/>
**Формат выходных данных.** Выведите количество рек, которые пересекаются с трассой.

***B.*** Арсений продолжает спать. Теперь ему снится кроличья ферма на планете Ка-Пэкс. Правда, ферма у него так себе — одни кроличьи норы в пустом поле. Чтобы её хоть как-то облагородить, Арсений решил поставить забор так, чтобы все норки оказались внутри огражденной территории, а досок он потратил как можно меньше. Помогите Арсению найти длину забора, чтобы он мог уже заказывать стройматериалы!<br/>
**Формат входных данных.** В первой строке вводится число N (3 ≤ N ≤ 10^5). Следующие N строк содержат пары целых чисел x и y (-10^9 ≤ x, y ≤ 10^9) — координаты кроличьих нор.<br/>
**Формат выходных данных.** Одно вещественное число — длину забора — с максимально возможной точностью.

***C.*** Арсений решил поиграть в настольную игру со своим другом Ильей. Так как играть обычными кубиками им уже стало неинтересно, Илья попросил по его чертежам сконструировать новую игральную кость. Так как он ленивый, то просто накидал точек в пространстве и сказал, что все они должны лежать в кубике его мечты. У Арсения есть 3D-принтер, вот только материалы для печати достаточно дорогие, поэтому он хочет выполнить требования своего друга, потратив как можно меньше пластика.<br/>
**Формат входных данных.** Первая строка содержит число M — количество тестов. В последующих строках описаны сами тесты. Каждый тест начинается со строки, содержащей N (N ≤ 1000) — число точек. Далее, в N строках даны по три числа — координаты точек. Все координаты целые, не превосходят по модулю 500.<br/>
**Формат выходных данных.** Для каждого теста выведите следующее. В первую строку выведите количество граней m. Далее в последующие m строк выведите описание граней: количество точек грани (=3) и номера точек в исходном множестве. Точки нумеруются в том же порядке, в котором они даны во входном файле. Точки в пределах грани должны быть отсортированы в порядке против часовой стрелки относительно внешней нормали к грани. Первая точка – точка с минимальным номером. Порядок граней лексикографический.

***D.*** Арсений опять уснул. И снова на планете Ка-Пэкс без него никак — два фермера поссорились из-за того, что их территории могут перекрываться. Естественно, как самого рассудительного, Арсения позвали урегулировать конфликт. Для начала он решил узнать, насколько серьезен конфликт. Для этого он решил узнать, пересекаются ли фермы вообще. Помогите Арсению это понять, если известно, что каждая ферма представляет собой выпуклый многоугольник.<br/>
**Формат входных данных.** Первая строка содержит число N точек первого многоугольника. Затем идут N строк с координатами точек первого многоугольника по часовой стрелке (координаты – действительные числа). Второй прямоугольник задается аналогично. N, M ≤ 80000.<br/>
**Формат выходных данных.** Выведите “YES”, если фермы пересекаются, и “NO”, если нет (без кавычек).

***E.*** Арсений открыл эзотерический салон в свои снах на планете Ка-Пэкс. У Арсения всё будет хорошо. А вот у его клиентов — не факт. Если хотя бы какие-нибудь их палочки в гадании "Мокусо Дзэй" пересеклись, то день точно сложится удачно. А если нет — то стоит ждать беды. Чтобы точнее сказать, что конкретно пойдет хорошо в этот день, нужно знать, какие именно палочки пересекаются. Помогите Арсению узнать, как пройдет день у его клиентов. <br/>
**Формат входных данных.** Палочка представляется как отрезок прямой. В первой строке входного файла записано число N (1 ≤ N ≤ 125000) — количество палочек в гадании. Следующие N строк содержат описания палочек: (i + 1)-я строка содержит координаты концов i-й палочки — целые числа x1, y1, x2, y2 (-10000 ≤ x1, y1, x2, y2 ≤ 10000).<br/>
**Формат выходных данных.** В первой строке выходного файла выведите слово "YES", если день сложится удачно. Вторая строка должна содержать числа i и j — номера палочек, которые пересекаются. Если день пройдет плохо, выведите в единственной строке выходного файла "NO".



Третий модуль
--------------

***B.*** Два игрока играют в настольную игру. Игровое поле представляет собой квадратный лабиринт, 8× 8 клеток. В некоторых клетках располагаются стенки. Один игрок управляет фишкой-терминатором, а второй — фишкой-беглецом. Игроки ходят по очереди, ходы пропускать нельзя (гарантируется, что ход всегда возможен). За один ход игрок может переместить свою фишку в любую из свободных клеток, расположенных рядом с исходной по горизонтали, вертикали или по диагонали (то есть ходом короля). Терминатор, кроме того, может стрелять в беглеца ракетами. Выстрел идет по прямой в любом направлении по горизонтали, вертикали или диагонали. Если беглец оказывается на линии выстрела терминатора и не прикрыт стенками, то терминатор незамедлительно делает выстрел (вне зависимости от того, чей ход), и беглец проигрывает. Начальное положение фишек задано. Первый ход делает беглец. Он выигрывает, если сделает ход с восьмой строки за пределы игрового поля, так как остальные границы поля окружены стенками.
Вопрос задачи: может ли беглец выиграть при оптимальной игре обеих сторон?<br/>
**Формат входных данных.** Во входном файле задано игровое поле. Свободная клетка обозначена цифрой 0, а клетка со стенкой — цифрой 1. Клетка, в которой находится беглец, обозначена цифрой 2, а клетка с терминатором — цифрой 3.<br/>
**Формат выходных данных.** В выходной файл выведите число 1, если беглец выигрывает, и -1 — в противном случае.

***C.*** Штирлиц и Мюллер стреляют по очереди. В очереди n человек, стоящих друг за другом. Каждым выстрелом убивается один из стоящих. Кроме того, если у кого-то из стоящих в очереди убиты все его соседи, то этот человек в ужасе убегает. Проигрывает тот, кто не может ходить. Первым стреляет Штирлиц. Требуется определить, кто выиграет при оптимальной игре обеих сторон, и если победителем будет Штирлиц, то найти все возможные первые ходы, ведущие к его победе.<br/>
**Формат входных данных.** Входной файл содержит единственное число n (2≤ n≤ 5 000) — количество человек в очереди.<br/>
**Формат выходных данных.** Если выигрывает Мюллер, выходной файл должен состоять из единственного слова Mueller. Иначе в первой строке необходимо вывести слово Schtirlitz, а в последующих строках — номера людей в очереди, которых мог бы первым ходом убить Штирлиц для достижения своей победы. Номера необходимо выводить в порядке возрастания.
