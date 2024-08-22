# 1-Python-Data-types
## Переменные
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&width=435&lines=variable+%3D+value)](https://git.io/typing-svg)

Перед разбором какие типы данных бывают в Python, необходимо понять где они будут храниться. Для этого, необходимо создать объект - переменную. Переменные — это имена, которые присваиваются значениям для их хранения и использования в программе.

Представьте, что у вас есть шкаф с полками, и каждая полка имеет своё название: "Книги", "Одежда", "Игрушки". Названия полок — это переменные, а то, что лежит на этих полках — значения переменных.

Например:

Полка "Книги" содержит 5 книг.
Полка "Одежда" содержит 10 футболок.
Полка "Игрушки" содержит 7 игрушек.
В этом примере "Книги", "Одежда", "Игрушки" — это переменные, а количество предметов на каждой полке — это их значения. Вы можете заменить содержимое полок, но названия полок остаются теми же, позволяя вам всегда знать, где что находится.

**Ключевые моменты:**

- **Именованная ссылка:** Переменная — это имя, указывающее на объект, содержащий данные.
- **Присваивание:** Когда вы присваиваете значение переменной (x = 10), Python создаёт объект с значением 10 и связывает его с именем x.
- **Изменяемость и неизменяемость:** Тип данных объекта определяет, можно ли изменить объект после создания (например, списки изменяемы, а строки — нет).
- **Сборка мусора:** Когда переменная перестаёт ссылаться на объект, Python автоматически удаляет этот объект из памяти, если на него больше нет ссылок.

**При создании переменных в Python необходимо соблюдать несколько простых правил. Вот основные из них:**

1. Имя переменной должно начинаться с буквы или символа подчёркивания (_):
- Правильно: name, _value, count1
- Неправильно: 1st_value, @temp
2. Имя переменной может содержать только буквы, цифры и символ подчёркивания:
- Правильно: user_name, age25, max_speed
- Неправильно: user-name, max speed, age#
3. Имена переменных чувствительны к регистру:
```
age = 20
Age = 30
print(age)  # Выведет 20
print(Age)  # Выведет 30
```
Переменные age и Age считаются разными.

4. Имена переменных не могут совпадать с ключевыми словами Python:
Например, нельзя использовать if, while, for, True, None и другие ключевые слова.
```
# Неправильно:
if = 10  # Ошибка синтаксиса
```
5. Имя переменной должно быть осмысленным:
Лучше выбирать такие имена, которые отражают смысл хранимых данных.
Правильно: user_name, total_price
Неправильно: x, y, a123 (если они не несут явного смысла)
```
user_name = "Alice"
number_users = 127900
update = True
dog_age = 6
```

## Основные типы данных
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&width=435&lines=%23+data+types;name+%3D+%22FirstName%22;to_do_list+%3D+%5B%22study%22%2C+%22play%22%5D;smile+%3D+%22%F0%9F%98%8A%22)](https://git.io/typing-svg)

В Python, практически каждый объект имеет свой тип данных. Тип данных в Python — это категория, которая определяет, какие операции можно выполнять над объектом и как он будет храниться в памяти. Тип данных указывает на природу значения, хранимого в объекте, и определяет допустимые операции, которые можно выполнять с этим объектом. Например, числа относятся к числовым типам данных, строки — к строковым, списки — к коллекциям и так далее.

В Python существует множество встроенных типов данных, среди которых:

| Тип данных | Описание                         | Пример                                 |
|------------|----------------------------------|----------------------------------------|
| **int**    | Целые числа                      | `x = 10`                               |
| **float**  | Числа с плавающей запятой        | `y = 3.14`                             |
| **str**    | Строки                           | `city  = "Moscow"`                       |
| **list**   | Списки                           | `numbers = [1, 2, 3, 4, 5]`            |
| **tuple**  | Кортежи                          | `coordinates = (10, 20)`               |
| **dict**   | Словари                          | `person = {"name": "John", "age": 30}` |
| **set**    | Множества                        | `unique_numbers = {1, 2, 3}`           |
| **bool**   | Логические значения (`True/False`) | `is_valid = True`                      |

**Разберём более детально:**
1. int (целые числа)
Целые числа представляют собой числа без десятичной части. Они могут быть положительными, отрицательными или нулевыми.
```
age = 25
temperature = -10
```
Целые числа применяются, когда нужно работать с целыми значениями, такими как количество предметов, возраст или счётчики.

2. float (числа с плавающей запятой)
Числа с плавающей запятой представляют собой числа с дробной частью (десятичные числа).
```
pi = 3.14
height = 5.9
```
Этот тип данных используется для представления измерений, результатов деления и других значений, которые могут быть нецелыми.

3. str (строки)
Строки представляют собой последовательности символов и используются для хранения текстовой информации.
```
name = "Alice"
greeting = "Hello, world!"
```
Строки используются для работы с текстом, включая хранение и отображение сообщений, имён и других текстовых данных.

4. list (списки)
Списки (массивы) — это упорядоченные коллекции элементов, которые могут содержать элементы разных типов данных.
```
fruits = ["apple", "banana", "cherry"]
numbers = [-1, 2, 0, 10, 3.5]
matrix = [[1, 2, 3],
          [4, 5, 6],
          [7, 8, 9]]
```
Списки позволяют хранить и манипулировать множеством значений, таких как последовательности чисел, строки или объекты. Их можно изменять по мере необходимости, удалять или добавлять элементы. Могут быть одномерными, двумерными и т.д.

5. tuple (кортежи)
Кортежи — это упорядоченные коллекции элементов, похожие на списки, но в отличие от списков, кортежи неизменяемы (их элементы нельзя изменять после создания).
```
coordinates = (10, 20)
colors = ("red", "green", "blue")
```
Кортежи используются, когда необходимо сохранить набор значений, который не должен изменяться, например, координаты точек или параметры функции.

6. dict (словари)
Словари представляют собой неупорядоченные коллекции пар "ключ-значение", где каждое значение связано с уникальным ключом.
```
person = {"name": "John", "age": 30}
phonebook = {"Alice": "123-4567", "Bob": "987-6543"}
data_users = {1314: "Vasya", 6357: "Olya", 2071: "Dima"}  # Пример хранения id и имени пользователя
```
Словари позволяют быстро находить значения по их ключам и используются для хранения связанной информации, такой как данные о пользователе, телефонные книги и т.д.

7. set (множества)
Множества представляют собой неупорядоченные коллекции уникальных элементов.
```
unique_numbers = {1, 2, 3, 3, 4}
letters = {"a", "b", "c"}
```
Множества используются для хранения коллекций элементов без дубликатов и позволяют выполнять такие операции, как объединение и пересечение множеств.

8. bool (логические значения: True и False)
Логические значения представляют собой тип данных, который может быть только True (истина) или False (ложь).
```
is_valid = True
has_access = False
```
Логические значения применяются для выполнения условий и управления потоком выполнения программы, например, в условных выражениях (if, while) и логических операциях.

Это **основные** типы данных, на практике их будет больше.

## Перейдём к примеру
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&width=435&lines=%23+Example;read+%3D+True;understand+%3D+%22%F0%9F%98%B6%22++%23+%3F)](https://git.io/typing-svg)

Предположим, у нас есть следующая личная карточка пользователя:

**Личная карточка**

| Фото                                                                                      | Имя   | Специальность | Возраст | Вес  | Страны, в которых был                  | Владение языками                                                                                   | Водительские права |
|-------------------------------------------------------------------------------------------|-------|---------------|---------|------|----------------------------------------|------------------------------------------------------------------------------------------------------|--------------------|
| <img src="https://github.com/TeachKait20/NoneCode/blob/main/Igor.png?raw=true" width="250"/> | Игорь | Программист    | 19      | 67.5 | Британия, Китай, Германия              | Русский - профессиональный уровень владения, Английский - Продвинутый, Китайский - начальный, Немецкий - средний | Есть               |


Давайте разберём, как можно представить информацию из личной карточки пользователя в виде переменных в Python. А так же посмотрим, какие способы при этом можно использовать.
```
# Персональная информация
name = "Игорь"
specialty = "Программист"
age = 19
weight = 67.5

# Страны, в которых был
visited_countries = ["Британия", "Китай", "Германия"]

# Владение языками
languages = {
    "Русский": "профессиональный уровень владения",
    "Английский": "Продвинутый",
    "Китайский": "начальный",
    "Немецкий": "средний"
}

# Наличие водительских прав
has_driver_license = True

# Фото Игоря
photo_url = "https://github.com/TeachKait20/NoneCode/blob/main/Igor.png?raw=true"
```

Далее, всё можно будет вывести в консоль, с помощью функции `print()`
