# lab_01
TASK 2.6
nabir.h
- тут створений class Nabir, у якому зберігається інформація про певний набір з кубиків(кількість, ймовірність випадіння граней...)
також тут визначені основні методи для роботи з цим набором кубиків та обчислення операцій порівняння)

- nabir.cpp 
-- Тут реалізовано функції порівняння, метод print(), який виводить інформацію про набір кубиків на консоль.
 Він виводить кількість кубиків у наборі і інформацію про кожен з них
Add(Dice& kub): Цей метод додає кубик kub до набору кубиків. Він спочатку створює новий масив кубиків більшого розміру,
 копіює існуючі кубики в новий масив, додає новий кубик та оновлює кількість кубиків у наборі (numcubes). Після цього викликає метод Summ(), щоб перерахувати ймовірності для нового набору кубиків.
Summ(int show): Цей метод обчислює всі можливі суми результатів кидків кубиків у наборі, а також їхні ймовірності. Він використовує для цього масиви sums і probability, які зберігають кількість сум та ймовірностей для кожної з них.
 Метод працює з урахуванням мінімальних і максимальних можливих сум кубиків та генерує всі можливі комбінації результатів кидків для обчислення сум і ймовірностей.

Також тут створена змінна carry, яка використовується в циклі для перевірки, чи потрібно перенести одиницю з одного розряду в інший під час ітерації.
 (Якщо carry дорівнює 1, то це означає, що в попередньому розряді була досягнута максимальна грань кубика)

-----------------------------------------------------
- dice.h

Тут визначена робота з гральним кубиком(В class Dice), конструктор копіювання на деструктор...

-- Dice.cpp
В цьому класі реалізована можливість генерації кубиків та виведення інформації про них, в тому числі й імовірності.
Конструктори Dice::Dice(int size) та Dice::Dice(int sz1, int sz2) використовуються для створення об'єкта класу Dice з вказаними параметрами щодо діапазону можлих значень граней кубика.

int Dice::CostBySide(int i) і float Dice::ProbBySide(int i) - ці функції повертають вартість (суму очок) та ймовірність випадіння грані з індексом i відповідно.

Dice::~Dice() - це деструктор класу Dice, який виконує звільнення пам'яті, виділеної для збереження граней і ймовірностей.

int Dice::sides() повертає кількість граней кубика.

------------------------------
int main
d.Init(3,8); Ініціалізує об'єкт d кубика зі значенням граней від 3 до 8.
d.Init(5,8); Ініціалізує кубик d із новими значеннями граней від 5 до 8.

d.Init(10,30,3);: Ініціалізує кубик d зі значеннями граней від 10 до 30 з кроком 3.

n1.Add(d); Додає кубик d до набору n1.
n1.print(); Виводить інформацію про оновлений набір n1.

------------------------------------------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------------------------

Task 1.2
