[Назад к описанию курса](../../README.md)

# Стандартные встроенные объекты JavaScript

Содержание:
- [1. Глобальные функции](#1-Глобальные-функции)
  - [1.1. Ссылки](#11-Ссылки)
  - [1.2. Задачи](#12-Задачи)
    - [1.2.1. Интерпретация кода](#121-Интерпретация-кода)
- [2. Объект `Number` (число)](#2-Объект-Number-число)
  - [2.1. Ссылки](#21-Ссылки)
  - [2.2. Задачи](#22-Задачи)
    - [2.2.1. Граничные значения числа](#221-Граничные-значения-числа)
    - [2.2.2. Приведение к числу](#222-Приведение-к-числу)
- [3. Объект `String` (строка)](#3-Объект-String-строка)
  - [3.1. Ссылки](#31-Ссылки)
  - [3.2. Задачи](#32-Задачи)
    - [3.2.1. Заглавная буква](#321-Заглавная-буква)
    - [3.2.2. Ограничение длины строки](#322-Ограничение-длины-строки)
- [4. Объект `Array` (массив)](#4-Объект-Array-массив)
  - [4.1. Ссылки](#41-Ссылки)
  - [4.2. Задачи](#42-Задачи)
    - [4.2.1 Создание массива](#421-Создание-массива)
    - [4.2.2. Последний элемент массива](#422-Последний-элемент-массива)
    - [4.2.3. Сортировка массива в обратном порядке](#423-Сортировка-массива-в-обратном-порядке)
- [5. Объект `Object` (объект)](#5-Объект-Object-объект)
  - [5.1. Ссылки](#51-Ссылки)
  - [5.2. Задачи](#52-Задачи)
    - [5.2.1. Создание объекта](#521-Создание-объекта)
    - [5.2.2. Проверка объекта на отсутствие свойств](#522-Проверка-объекта-на-отсутствие-свойств)
    - [5.2.3. Сумма свойств объекта](#523-Сумма-свойств-объекта)
    - [5.2.3. Свойство объекта с наибольшим значением](#523-Свойство-объекта-с-наибольшим-значением)
- [6. Объект `Math`](#6-Объект-Math)
  - [5.1. Ссылки](#51-Ссылки)
  - [5.2. Задачи](#52-Задачи)
    - [5.2.1. Вычисление площади круга](#521-Вычисление-площади-круга)
    - [5.2.2. Вычисление площади треугольника](#522-Вычисление-площади-треугольника)

## 1. Глобальные функции

| Функция                   | Описание                                                                                                                                 |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| `eval(string)`            | Выполняет JavaScript код, представленный строкой `string`.                                                                               |
| `isFinite(value)`         | Определяет, является ли переданное значение `value` конечным числом.                                                                     |
| `isNaN(value)`            | Определяет, является ли переданное значение `value` не числовым значением `NaN` или нет.                                                 |
| `parseInt(string, radix)` | Принимает строку `string` в качестве аргумента и возвращает целое число в соответствии с указанным основанием системы счисления `radix`. |
| `parseFloat(string)`      | Принимает строку `string` в качестве аргумента и возвращает десятичное число с плавающей точкой.                                         |

### 1.1. Ссылки

- [Стандартные встроенные объекты](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects)
- [Функция `eval()`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/eval)
- [Функция `isFinite()`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/isFinite)
- [Функция `isNaN()`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/isNaN)
- [Функция `parseInt()`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/parseInt)
- [Функция `parseFloat()`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/parseFloat)

### 1.2. Задачи

#### 1.2.1. Интерпретация кода

С помощью функции `eval()` вычислить сумму двух переменных `a` и `b`:

```js
let a = 3, b = 4;
```

<details>
<summary>Посмотреть решение</summary>
<hr>

Вызов функции `eval()`:

> ```js
> -> let a = 3, b = 4
> <- undefined
> -> eval('a + b')
> <- 7
> ```

<hr>
</details>

## 2. Объект `Number` (число)

Объект `Number` является объектом-обёрткой, позволяющей вам работать с числовыми значениями. Может использоваться для приведения значений других типов к числу:

> ```js
> -> Number('3.14')
> <- 3.14
> -> Number(true)
> <- 1
> -> Number(null)
> <- 0
> ```

Свойства объекта `Number`:

| Свойство                   | Описание                                                                                                                          |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `Number.MAX_VALUE`         | Наибольшее представимое положительное число.                                                                                      |
| `Number.MIN_VALUE`         | Наименьшее представимое положительное число — то есть, самое близкое к нулю положительное число (которое ещё не является нулём). |
| `Number.NaN`               | Специальное значение для представления «не числа».                                                                                |
| `Number.NEGATIVE_INFINITY` | Специальное значение для представления отрицательной бесконечности; возвращается при переполнении.                                |
| `Number.POSITIVE_INFINITY` | Специальное значение для представления положительной бесконечности; возвращается при переполнении.                                |

Методы объекта `Number`:

| Метод                 | Описание                                                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| `num.toFixed(digits)` | Форматирует число, используя запись с фиксированной запятой с `digits` цифр после десятичной запятой (по умолчанию `0`). |
| `num.toString(radix)` | Возвращает строковое представление указанного объекта с необязательным указанием системы счисления.                      |

### 2.1. Ссылки

- [Стандартные встроенные объекты](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects)
- [Объект `Number`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Number)

### 2.2. Задачи

#### 2.2.1. Граничные значения числа

Отобразить значения свойств `Number.MAX_VALUE` и `Number.MIN_VALUE`.

<details>
<summary>Посмотреть решение</summary>
<hr>

Результаты:

> ```js
> -> Number.MAX_VALUE
> <- 1.7976931348623157e+308
> -> Number.MIN_VALUE
> <- 5e-324
> ```

<hr>
</details>

#### 2.2.2. Приведение к числу

Не запуская код в браузере, попытаться вычислить результат вызова `Number()` в каждой строке:

```js
Number('123');
Number('');
Number('0x11');
Number('0b11');
Number('0o11');
Number('foo');
Number('100a');
Number(false);
Number(true);
Number(undefined);
Number(null);
```

Запустить код в браузере и проверить своё решение.

<details>
<summary>Посмотреть решение</summary>
<hr>

Результаты:

> ```js
> -> Number('123')
> <- 123
> -> Number('')
> <- 0
> -> Number('0x11')
> <- 17
> -> Number('0b11')
> <- 3
> -> Number('0o11')
> <- 9
> -> Number('foo')
> <- NaN
> -> Number('100a')
> <- NaN
> -> Number(false)
> <- 0
> -> Number(true)
> <- 1
> -> Number(undefined)
> <- NaN
> -> Number(null)
> <- 0
> ```

<hr>
</details>

## 3. Объект `String` (строка)

Объект `Number` является конструктором строк. Может использоваться для приведения значений других типов к строке:

> ```js
> -> String(3.14)
> <- "3.14"
> -> String(true)
> <- "true"
> -> String(undefined)
> <- "undefined"
> -> String(null)
> <- "null"
> ```

Свойства объекта `String`:

| Свойство     | Описание      |
| ------------ | ------------- |
| `str.length` | Длина строки. |

Методы объекта `String`:

| Метод                               | Описание                                                                                         |
| ----------------------------------- | ------------------------------------------------------------------------------------------------ |
| `str.charAt(index)`                 | Возвращает символ на позиции `index` из строки.                                                  |
| `str.indexOf(value, fromIndex)`     | Возвращает индекс первого вхождения значения `value` в строке, начиная с индекса `fromIndex`.    |
| `str.lastIndexOf(value, fromIndex)` | Возвращает индекс последнего вхождения значения `value` в строке, начиная с индекса `fromIndex`. |
| `str.slice(start, end)`             | Извлекает часть строки, начиная с индекса `start` и заканчивая `end`, и возвращает новую строку. |
| `str.toLowerCase()`                 | Возвращает значение строки преобразованное в нижний регистр.                                     |
| `str.toUpperCase()`                 | Возвращает значение строки преобразованное в верхний регистр.                                    |

### 3.1. Ссылки

- [Стандартные встроенные объекты](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects)
- [Объект `String`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String)

### 3.2. Задачи

#### 3.2.1. Заглавная буква

Написать функцию `capitalize(text)`, которая будет возвращать строку `text` с заглавным первым символом:

> ```js
> -> capitalize('привет, мир!')
> <- "Привет, мир!"
> -> capitalize('')
> <- ""
> ```


<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `capitalize(text)`:

```js
function capitalize(text) {
  // Проверка на случай пустой строки.
  if (!text) {
    return text;
  }

  return text[0].toUpperCase() + text.slice(1);
}
```

<hr>
</details>

#### 3.2.2. Ограничение длины строки

Создать функцию `truncate(text, length)`, которая заменяет часть строки `text` на `"..."` и делает её длину равной `length`, если её длина больше `length`:

> ```js
> -> 'Привет, мир!'.length
> <- 12
> -> truncate('Привет, мир!', 15)
> <- "Привет, мир!"
> -> truncate('Привет, мир!', 10)
> <- "Привет,..."
> -> 'Привет,...'.length
> <- 10
> ```

<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `truncate(text, length)`:

```js
function truncate(text, length) {
  if (text.length > length) {
    // Учитываем длину многоточия.
    return text.slice(0, length - 3) + '...';
  }

  return text;
}
```

<hr>
</details>

## 4. Объект `Array` (массив)

Объект `Array` является глобальным объектом, который используется для создания массивов:

```js
let arr;

// Пустой массив.
arr = [];

// Массив может хранить элементы любого типа.
arr = ['abc', 'def', 'ghi'];
arr = [123, 456, 789];
arr = [123, 'abc', [true, false]];

// Обращение к элементам массива.
arr[0]; // 123
arr[1]; // 'abc'
arr[2]; // [true, false]

// Особый цикл для массивов, обходит значения массива.
for (let item of arr) {
    alert(item);
}
```

Свойства объекта `Array`:

| Свойство     | Описание        |
| ------------ | --------------- |
| `arr.length` | Размер массива. |

Методы объекта `Array`:

| Метод                               | Описание                                                                                                      |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `arr.pop()`                         | Удаляет последний элемент из массива и возвращает его значение.                                               |
| `arr.push(value1, ..., valueN)`     | Добавляет один или более элементов `value1`, ..., `valueN` в конец массива и возвращает новую длину массива.  |
| `arr.shift()`                       | Удаляет первый элемент из массива и возвращает его значение.                                                  |
| `arr.unshift()`                     | Добавляет один или более элементов `value1`, ..., `valueN` в начало массива и возвращает новую длину массива. |
| `arr.reverse()`                     | Обращает порядок следования элементов массива.                                                                |
| `arr.indexOf(value, fromIndex)`     | Возвращает индекс первого вхождения значения `value` в массиве, начиная с индекса `fromIndex`.                |
| `arr.lastIndexOf(value, fromIndex)` | Возвращает индекс последнего вхождения значения `value` в массиве, начиная с индекса `fromIndex`.             |
| `arr.sort(compareFunction)`         | Сортирует элементы массива с помощью функции `compareFunction` и возвращает отсортированный массив.           |

### 4.1. Ссылки

- [Стандартные встроенные объекты](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects)
- [Объект `Array`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array)

### 4.2. Задачи

#### 4.2.1 Создание массива

Задание:
1. создать массив `fruits` с элементами `'Яблоко'` и `'Апельсин'`,
2. добавить в конец массива значение `'Банан'`,
3. заменить предпоследнее значение массива на `'Вишня'`,
4. удалить первое значение массива и вывести его с помощью функции `alert()`,
5. добавить в начало массива значения `'Гранат'` и `'Абрикос'`,
6. отсортировать массив.

<details>
<summary>Посмотреть решение</summary>
<hr>

Порядок действий:

> ```js
> -> let fruits = ['Яблоко', 'Апельсин']
> <- undefined
> -> fruits.push('Банан')
> <- 3
> -> fruits[fruits.length - 2] = 'Вишня'
> <- "Вишня"
> -> alert(fruits.shift())
> <- undefined
> -> fruits.unshift('Гранат', 'Абрикос')
> <- 4
> -> fruits.sort()
> <- ["Абрикос", "Банан", "Вишня", "Гранат"]
> ```

<hr>
</details>

#### 4.2.2. Последний элемент массива

Написать функцию `getLastItem(arr)`, которая будет возвращать последний элемент массива:

> ```js
> -> let arr = [123, 'abc', [true, false]]
> <- undefined
> -> getLastItem(arr)
> <- [true, false]
> ```

<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `getLastItem(arr)`:

```js
function getLastItem(arr) {
  return arr[arr.length - 1];
}
```

<hr>
</details>

#### 4.2.3. Сортировка массива в обратном порядке

Создать такую функцию `compareReversed(a, b)`, которая, при передаче её как аргумент функции `arr.sort(compareFunction)`, отсортирует массив чисел в обратном порядке.

> ```js
> -> let arr = [5, 2, 1, -10, 8]
> <- undefined
> -> arr.sort(compareReversed)
> <- [8, 5, 2, 1, -10]
> ```

<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `compareReversed(a, b)`:

```js
function compareReversed(a, b) {
  return b - a;
}
```

<hr>
</details>

## 5. Объект `Object` (объект)

Объект `Object` создаёт объект-обёртку:

```js
// Пустой объект.
let obj = {};

// Добавить свойства в объект.
obj.name = 'my object'; // obj = { 'name': 'my object' }
obj.age = 10;           // obj = { 'name': 'my object', 'age': 10 }

// Получить значения свойств.
alert(obj.name);        // 'my object'
alert(obj['age']);      // 10

// Особый цикл for для объектов, обходит имена свойств объекта.
for (let prop in obj) {
    alert(obj[prop]);
}

// Удалить свойство.
delete obj.age;         // obj = { 'name': 'my object' }
```

Методы `Object`:

| Метод              | Описание                                                |
| ------------------ | ------------------------------------------------------- |
| `Object.keys(obj)` | Возвращает массив из свойств переданного объекта `obj`. |

### 5.1. Ссылки

- [Стандартные встроенные объекты](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects)
- [Объект `Object`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Object)

### 5.2. Задачи

#### 5.2.1. Создание объекта

Задание:
1. создать пустой объект `user`,
2. добавить свойство `name` со значением `'Иван'`,
3. добавить свойство `surname` со значением `'Иванов'`,
4. поменять значение свойства `surname` на `'Петров'`,
5. с помощью функции `alert()` и цикла `for...in` вывести значения всех свойств объекта `user`,
6. удалить свойство `surname`.

<details>
<summary>Посмотреть решение</summary>
<hr>

Порядок действий:

```js
let user = {};
user.name = 'Иван';      // user = { 'name': 'Иван' }
user.surname = 'Иванов'; // user = { 'name': 'Иван', 'surname': 'Иванов' }
user.surname = 'Петров'; // user = { 'name': 'Иван', 'surname': 'Петров' }

for (let prop in user) {
    alert(user[prop]);
}

delete user.surname;     // user = { 'name': 'Иван' }
```

<hr>
</details>

#### 5.2.2. Проверка объекта на отсутствие свойств

Создать функцию `isEmpty(obj)`, которая возвращает `true`, если в объекте `obj` нет свойств и `false` – если хоть одно свойство есть:

> ```js
> -> let obj = {}
> <- undefined
> -> isEmpty(obj)
> <- true
> -> obj.value = 123
> <- 123
> -> isEmpty(obj)
> <- false
> ```

<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `isEmpty(obj)`:

```js
function isEmpty(obj) {
  let keys = Object.keys(obj);
  return !!keys.length;
}
```

<hr>
</details>

#### 5.2.3. Сумма свойств объекта

Написать скрипт, который выведет сумму значений всех свойств объекта `salaries`:

```js
let salaries = {
  "Василий": 100,
  "Дмитрий": 200,
  "Николай": 300
};
```

<details>
<summary>Посмотреть решение</summary>
<hr>

Подсчёт суммы:

```js
let sum = 0;
for (let name in salaries) {
  sum += salaries[name];
}

alert(sum);
```

<hr>
</details>

#### 5.2.3. Свойство объекта с наибольшим значением

Написать скрипт, который имя свойства с наибольшим значением `salaries`:

```js
let salaries = {
  "Василий": 100,
  "Дмитрий": 200,
  "Николай": 300
};
```

<details>
<summary>Посмотреть решение</summary>
<hr>

Подсчёт суммы:

```js
let max = 0;
let maxName = "";

for (let name in salaries) {
  if (max < salaries[name]) {
    max = salaries[name];
    maxName = name;
  }
}

alert(maxName);
```

<hr>
</details>

## 6. Объект `Math`

Объект `Math` является встроенным объектом, хранящим в своих свойствах и методах различные математические константы и функции.

Свойства объекта `Math`:

| Свойство     | Описание                  |
| ------------ | ------------------------- |
| `Math.PI`    | Число `π`.                |
| `Math.SQRT2` | Квадратный корень из `2`. |

Методы объекта `Math`:

| Метод                   | Описание                                                                      |
| ----------------------- | ----------------------------------------------------------------------------- |
| `Math.abs(x)`           | Возвращает абсолютное значение числа `x`.                                     |
| `Math.round(x)`         | Возвращает значение числа `x`, округлённое до ближайшего целого.              |
| `Math.floor(x)`         | Возвращает наименьшее целое число, меньшее, либо равное указанному числу `x`. |
| `Math.ceil(x)`          | Возвращает наименьшее целое число, большее, либо равное указанному числу `x`. |
| `Math.pow(x, y)`        | Возвращает значение числа `x`, возведённое в степень `y`.                     |
| `Math.random()`         | Возвращает псевдослучайное число в диапазоне от `0` до `1`.                   |
| `Math.max(x1, ..., xN)` | Возвращает наибольшее число из `x1`, ..., `xN`.                               |
| `Math.min(x1, ..., xN)` | Возвращает наименьшее число из `x1`, ..., `xN`.                               |


### 5.1. Ссылки

- [Стандартные встроенные объекты](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects)
- [Объект `Math`](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Math)

### 5.2. Задачи

#### 5.2.1. Вычисление площади круга

Написать функцию `getCircleArea(radius)`, возвращающую площадь круга с радиусом `radius`:

> ```js
> -> getCircleArea(5)
> <- 78.54
> -> getCircleArea(0)
> <- 0
> -> getCircleArea(-5)
> <- NaN
> ```

Значение площади округлить до второго знака после запятой.

<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `getCircleArea(radius)`:

```js
function getCircleArea(radius) {
  if (radius < 0) {
    return NaN;
  }

  let area = Math.PI * Math.pow(radius, 2);
  return +area.toFixed(2);
}
```

<hr>
</details>

#### 5.2.2. Вычисление площади треугольника

Написать функцию `getTriangleArea(a, b, angle)`, возвращающую площадь треугольника со сторонами `a` и `b` и углом `angle` (в градусах) между ними:

> ```js
> -> getTriangleArea(4, 12, 60)
> <- 20.78
> -> getTriangleArea(0, 0, 0)
> <- 0
> -> getTriangleArea(-5, -4, 270)
> <- NaN
> ```

Значение площади округлить до второго знака после запятой.

<details>
<summary>Посмотреть решение</summary>
<hr>

Функция `getTriangleArea(a, b, angle)`:

```js
function getTriangleArea(a, b, angle) {
  if (a < 0 || b < 0 || angle >= 180 || angle <= 0) {
    return NaN;
  }

  // Переводим градусы в радианы.
  let rad = angle * Math.PI / 180.;

  // Вычисляем площадь треугольника.
  let area = a * b * Math.sin(rad) / 2.;
  return +area.toFixed(2);
}
```

<hr>
</details>
