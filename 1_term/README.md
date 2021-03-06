Первый семестр
===============

Первый модуль
--------------

***1_5.*** Вывести квадраты натуральных чисел от 1 до n, используя только O(n) операций сложения и вычитания (умножением пользоваться нельзя).<br/>
**Ограничения:** n ≤ 1000.


***2_1.*** Даны два массива целых чисел одинаковой длины A[0..n-1] и B[0..n-1]. Необходимо найти первую пару индексов i0 и j0, i0 ≤ j0, такую что A[i0] + B[j0] = max {A[i] + B[j], где 0 <= i < n, 0 <= j < n, i <= j}. Время работы - O(n).<br/>
**Ограничения:** n ≤ 100000.

***3_2.***  Дан массив целых чисел А[0..n-1]. Известно, что на интервале [0, m] значения массива строго возрастают, а на интервале [m, n-1] строго убывают. Найти m за O(log m).<br/>
**Ограничения:** 2 ≤ n ≤ 10000.
 
***4_3.***  Реализовать очередь с помощью двух стеков. Использовать стек, реализованный с помощью динамического буфера. Поддержать методы *push*, *pop*. <br/>
**Формат входных данных.** В первой строке количество команд n. n ≤ 1000000.
Каждая команда задаётся как 2 целых числа: a b.<br/>
a = 2 - pop front<br/>
a = 3 - push back<br/>
Если дана команда pop, то число b - ожидаемое значение.Если команда pop вызвана для пустой структуры данных, то ожидается “-1”. <br/>
**Формат выходных данных.** Требуется напечатать YES - если все ожидаемые значения совпали. Иначе, если хотя бы одно ожидание не оправдалось, то напечатать NO.

***5_1.*** Дан фрагмент последовательности скобок, состоящей из символов (){}[].
Требуется определить, возможно ли продолжить фрагмент в обе стороны, получив корректную последовательность.
Длина исходной последовательности ≤ 800000.<br/>
**Формат входных данных.** Строка, содержащая символы (){}[] и, возможно, перевод строки.<br/>
**Формат выходных данных.** Если возможно - вывести минимальную корректную последовательность, иначе - напечатать "IMPOSSIBLE".

***6_1.*** Вовочка ест фрукты из бабушкиной корзины. В корзине лежат фрукты разной массы. Вовочка может поднять не более K грамм. Каждый фрукт весит не более K грамм. За раз он выбирает несколько самых тяжелых фруктов, которые может поднять одновременно, откусывает от каждого половину и кладет огрызки обратно в корзину. Если фрукт весит нечетное число грамм, он откусывает большую половину. Фрукт массы 1гр он съедает полностью. Определить за сколько подходов Вовочка съест все фрукты в корзине.<br/>
**Формат входных данных.** Вначале вводится n - количество фруктов и n строк с массами фруктов.
n ≤ 50000. Затем K - "грузоподъемность". K ≤ 1000.<br/>
**Формат выходных данных.** Неотрицательное число - количество подходов к корзине.


Второй модуль
--------------
***1_5.*** В базе данных хранится N записей, вида (Name, a1, a2, … , ak) — во всех записях одинаковое число параметров.
На вход задачи подаётся приоритет полей — перестановка на числах 1,...,k — записи нужно вывести в соответствии с этим приоритетом. В случае, если приоритет полей таков: 3 4 2 1, то это следует воспринимать так: надо читать как: приоритет значений из 3 колонки самый высокий, приоритет значений из колонки 4 ниже, приоритет значений из колонки 2 ещё ниже, а приоритет значений из колонки 1 самый низкий.<br/>
**Формат входных данных.** 
N (1⩽N⩽1000)<br/>
k (1⩽k;⩽10)<br/>
p1 p2 ... pk (перестановка на k числах, разделитель пробел)<br/>
N строк вида<br/>
Name a1 a2 ... ak (разделитель — пробел)<br/>
**Формат выходных данных.** N строк с именами согласно приоритету

***2_4.*** На числовой прямой окрасили N отрезков. Известны координаты левого и правого концов каждого отрезка (Li и Ri). Найти сумму длин частей числовой прямой, окрашенных ровно в один слой.

***3_1.*** Даны неотрицательные целые числа n,k и массив целых чисел из [0..10^9] размера n. Требуется найти k-ю порядковую статистику. т.е. напечатать число, которое бы стояло на позиции с индексом k (0..n-1) в отсортированном массиве. Напишите нерекурсивный алгоритм.
Требования к дополнительной памяти: O(n). Требуемое среднее время работы: O(n).<br/>
Реализуйте стратегию выбора опорного элемента “медиана трёх”. Функцию Partition реализуйте методом прохода двумя итераторами от начала массива к концу.

***4_1.*** Дана очень длинная последовательность целых чисел длины n. Требуется вывести в отсортированном виде её первые k элементов. Последовательность может не помещаться в память. Время работы O(n * log(k)). Доп. память O(k). Использовать слияние.

***5_2.*** Дан массив неотрицательных целых 64-битных чисел. Количество чисел не больше 106. Отсортировать массив методом поразрядной сортировки LSD по байтам.

Третий модуль
--------------
***1_1.*** Дано число N < 106 и последовательность целых чисел из [-231..231] длиной N. Требуется построить бинарное дерево, заданное наивным порядком вставки. Балансировку выполнять не требуется.

***2_1.*** Дано число N < 106 и последовательность пар целых чисел из [-231..231] длиной N. Построить декартово дерево из N узлов, характеризующихся парами чисел {Xi, Yi}. Каждая пара чисел {Xi, Yi} определяет ключ Xi и приоритет Yi в декартовом дереве. Построить также наивное дерево поиска по ключам Xi методом из задачи 1. Вычислить разницу глубин наивного дерева поиска и декартового дерева. Разница может быть отрицательна.

***3_2.*** (Использование АВЛ-дерева) Дано число N и N строк. Каждая строка содержит команду добавления или удаления натуральных чисел, а также запрос на получение k-ой порядковой статистики. Команда добавления числа A задается положительным числом A, команда удаления числа A задается отрицательным числом “-A”. Запрос на получение k-ой порядковой статистики задается числом k. Требуемая скорость выполнения запроса - O(log n).


Четвертый модуль
--------------

***1_2.*** Реализуйте структуру данных типа “множество строк” на основе динамической хеш-таблицы с открытой адресацией. Хранимые строки непустые и состоят из строчных латинских букв. Начальный размер таблицы должен быть равным 8-ми. Перехеширование выполняйте при добавлении элементов в случае, когда коэффициент заполнения таблицы достигает 3/4.<br/>
Хеш-функцию строки реализуйте с помощью вычисления значения многочлена методом Горнера.<br/>
Структура данных должна поддерживать операции добавления строки в множество, удаления строки из множества и проверки принадлежности данной строки множеству.<br/>
Для разрешения коллизий используйте двойное хеширование.<br/>
**Формат входных данных.** Каждая строка входных данных задает одну операцию над множеством. Запись операции состоит из типа операции и следующей за ним через пробел строки, над которой проводится операция.<br/>
Тип операции  – один из трех символов:<br/>
- "+"  означает добавление данной строки в множество; 
- "-" означает удаление  строки из множества;  
- "?"  означает проверку принадлежности данной строки множеству.


При добавлении элемента в множество НЕ ГАРАНТИРУЕТСЯ, что он отсутствует в этом множестве. При удалении элемента из множества НЕ ГАРАНТИРУЕТСЯ, что он присутствует в этом множестве.<br/>
**Формат выходных данных.** Программа должна вывести для каждой операции одну из двух строк OK или FAIL, в зависимости от того, встречается ли данное слово в нашем множестве.

***2_2.*** В большой IT-фирме есть только одна переговорная комната. Желающие посовещаться заполняют заявки с желаемым временем начала и конца. Ваша задача определить максимальное количество заявок, которое может быть удовлетворено. Число заявок ≤ 100000.<br/>
**Формат входных данных.** Вход содержит только пары целых чисел — начала и концы заявок.<br/>
**Формат выходных данных.** Выход должен содержать натуральное число — максимальное число заявок.

***3_2.*** Дано N кубиков. Требуется определить каким количеством способов можно выстроить из этих кубиков пирамиду. Каждый вышележащий слой пирамиды должен быть строго меньше нижележащего. N ≤ 300.<br/>
**Формат входных данных.** На вход подается количество кубиков N.<br/>
**Формат выходных данных.** Вывести число различных пирамид из N кубиков.

***4_2.*** Дано невзвешенное дерево. Расстоянием между двумя вершинами будем называть количество ребер в пути, соединяющем эти две вершины. Для каждой вершины определите сумму расстояний до всех остальных вершин. Время работы должно быть O(n).<br/>
**Формат входных данных.** В первой строке записано количество вершин n ≤ 10000. Затем следует n – 1 строка, описывающая ребра дерева. Каждое ребро – это два различных целых числа – индексы вершин в диапазоне [0, n–1]. Индекс корня – 0. В каждом ребре родительской вершиной является та, чей номер меньше.<br/>
**Формат выходных данных.** Выход должен содержать n строк. В i-ой строке выводится сумма расстояний от i-ой вершины до всех остальных.
