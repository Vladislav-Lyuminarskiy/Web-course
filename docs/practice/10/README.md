# 10. Циклы. Функции. Подключение скриптов к странице. Отладка кода в браузере

## Темы занятия

### HTML

[`<script>`](https://webref.ru/html/script) - описание скриптов, используемых
на странице и его атрибуты:

- [`src`](https://webref.ru/html/script/src) - адрес скрипта из внешнего 
файла для импорта в текущий документ.
- [`defer`](https://webref.ru/html/script/defer) - откладывает выполнение 
скрипта до тех пор, пока вся страница не будет загружена полностью.
- [`async`](https://webref.ru/html/script/async) - загружает скрипт асинхронно.

### JavaScript

- Объект [`Console`](https://developer.mozilla.org/ru/docs/Web/API/Console):

  - [`console.log()`
  ](https://developer.mozilla.org/ru/docs/Web/API/Console/log) -
  выводит сообщение на консоль браузера.  
  - [`console.info()`
  ](https://developer.mozilla.org/ru/docs/Web/API/Console/info) -
  выводит на консоль браузера информационное сообщение.  
  - [`console.warn()`
  ](https://developer.mozilla.org/ru/docs/Web/API/Console/warn) -
  выводит на консоль браузера предупреждение.  
  - [`console.error()`
  ](https://developer.mozilla.org/ru/docs/Web/API/Console/error) -
  выводит на консоль браузера сообщение об ошибке.

- Циклы:

  - [`while`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/while) -
  выполняет указанное выражение до тех пор, пока истинно проверяемое условие.  
  - [`do...while`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/do...while) -
  выполняет указанное выражение (как минимум один раз) до тех пор,
  пока истинно проверяемое условие.  
  - [`for`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for) -
  выполняет указанное выражение до тех пор, пока истинно проверяемое условие;
  позволяет выполнить _выражение инициализации_ перед началом цикли и 
  _финальное выражение_ в конце каждой итерации цикла.  
  - [`for...of`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...of) -
  выполняет указанное выражение над каждым элементом массива (или любого 
  другого _итерируемого_ объекта).  
  - [`for...in`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...in) -
  выполняет указанное выражение над каждым перечислимым свойством объекта.  
  - [`break`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/break) -
  прерывает выполнение текущего цикла.  
  - [`continue`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/continue) -
  прерывает выполнение текущей итерации цикла и переходит к следующей итерации.

- Функции, конструкторы и методы объектов:

  - [`function`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/function) -
  определяет функцию с указанным именем, аргументами и телом.
  - [Функциональное выражение
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/function) -
  определяет функцию внутри выражения, может быть _именованным_.
  - [`(...) => {...}`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Functions/Arrow_functions) -
  определяет _стрелочную функцию_.
  - [`this`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/this) -
  ссылка на объект, который является текущим контекстом исполнения.
  - [`new`
  ](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/new) -
  оператор, создаёт новый экземпляр объекта с помощью _функции-конструктора_.

- Отложенный вызов функций:

  - [`setTimeout(func, delay)`
  ](https://developer.mozilla.org/ru/docs/Web/API/WindowTimers/setTimeout) - 
  вызывает функции `func` после задержи в `delay` миллисекунд.
  - [`clearTimeout(timeoutId)`
  ](https://developer.mozilla.org/ru/docs/Web/API/WindowOrWorkerGlobalScope/clearTimeout) -
  отменяет вызов функции по задержке по идентификатору `timeoutId`.
  - [`setInterval(func, delay)`
  ](https://developer.mozilla.org/ru/docs/Web/API/WindowOrWorkerGlobalScope/setInterval) -
  циклически вызывает функции `func` с паузой в `delay` миллисекунд
  между вызывами.
  - [`clearInterval(intervalId)`
  ](https://developer.mozilla.org/ru/docs/Web/API/WindowOrWorkerGlobalScope/clearInterval) -
  отменяет циклический вызов функции по идентификатору `intervalId`.
  
### Прочее

Работа с [отладчиком JavaScript
](https://developers.google.com/web/tools/chrome-devtools/javascript)
в инструментах разработчика Chrome.

## Теоретические сведения

### Объект `Console`

#### Ссылки по теме

- [Команды для работы с JavaScript-консолью в браузерах и повышение производительности труда программиста
](https://habr.com/ru/company/ruvds/blog/414375/).

### Циклы

#### Ссылки по теме

- [Циклы while, for](https://learn.javascript.ru/while-for).
- [Объекты: перебор свойств](https://learn.javascript.ru/object-for-in).
- [Итераторы](https://learn.javascript.ru/iterator).
- [Циклы и итерации
](https://developer.mozilla.org/ru/docs/Web/JavaScript/Guide/Циклы_и_итерации).

### Функции, конструкторы и методы объектов

#### Ссылки по теме

- [Функции](https://learn.javascript.ru/function-basics).
- [Функциональные выражения
](https://learn.javascript.ru/function-declaration-expression).
- [Именованные функциональные выражения
](https://learn.javascript.ru/named-function-expression).
- [Функции](https://learn.javascript.ru/es-function).
- [Методы объектов, this](https://learn.javascript.ru/object-methods).
- [Создание объектов через "new"](https://learn.javascript.ru/constructor-new).

### Отложенный вызов функций

#### Ссылки по теме

- [Отложенный вызов функций
](https://learn.javascript.ru/settimeout-setinterval).

### Подключение скриптов к странице

#### Ссылки по теме

- [Внешние скрипты, порядок исполнения
](https://learn.javascript.ru/external-script).

### Отладка кода в браузере

Отладка кода в JavaScript браузере Chrome производится во вкладке `Sources`.

#### Ссылки по теме

- [Отладка в браузере Chrome](https://learn.javascript.ru/debugging-chrome).

## 10.1. Консоль и циклы

### Вывод чётных чисел

Задачи:

1. С помощью цикла [`for`
](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for)
выведите на консоль все чётные числа от `0` до `10`.
2. Сделайте то же самое с помощью цикла [`while`
](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/while).

### Работа с массивами

Задачи:

1. Создайте массив строк.
2. С помощью цикла [`while`
](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/while)
выведите на консоль строки массива с длиной больше `4`.
3. Сделайте то же самое с помощью цикла [`for`
](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for).
4. Сделайте то же самое с помощью цикла [`for...of`
](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...of).

### Работа с объектами

Задачи:

1. Создайте объект с несколькими свойствами.

2. Напишите цикл, который будет выводить на консоль построчно все свойства 
этого объекта и их значения.
 
    Например, создадим следующий объект:
    
    ```js
    {
      name: "Иван",
      surname: "Иванов",
      age: 23
    }
    ```
    
    Вывод для него должен выглядеть следующим образом:

    ```
    name = Иван
    surname = Иванов
    age = 23
    ```

### Запрос числа от пользователя

Задачи:

1. Напишите цикл, который с помощью функции [`prompt()`
](https://developer.mozilla.org/ru/docs/Web/API/Window/prompt)
будет запрашивать у пользователя ввод числа до тех пор, пока пользователь не 
введёт число меньше `100`, либо не нажмёт на кнопку `Отмена`.

2. Если пользователь отменил ввод, выведите на консоль следующее информационное
сообщение:

    ```
    Пользователь отменил ввод числа.
    ```

3. Если пользователь ввёл некорректное число, выведите на консоль следующее
предупреждение:

    ```
    Ожидается число меньше 100.
    Пользователь ввёл число 25.
    ```

4. Если пользователь ввёл значение, не являющееся числом, выведите на консоль
следующее сообщение об ошибке:

    ```
    Ожидается число.
    Пользователь ввёл значение "...".
    ```

## 10.2. Функции, конструкторы и методы объектов

### Возведение числа в степень

Создайте следующую функцию:  

```js
/**
 * Возвращает результат возведения основания в спепень.
 * 
 * @param {number} base - Основание, рациональное число.
 * @param {number} exponent - Показатель степени, целое число.
 * @return {number} Результат возведения основания в степень.
 */
function power(base, exponent) { /* ... */ }
```

Примеры работы функции:

```js
power(2, 4); // 16
power(2, 1); // 2
power(2, 0); // 1
power(2, -1); // 0.5
power(2, -4); // 0.0625
```

Продемонстрируйте работу функции.

### Обращение порядка следования элементов массива

Создайте следующую функцию:  

```js
/**
* Обращает порядок следования элементов массива.
* 
* @param {array} arr - Обращаемый массив.
*/
function reverse(arr) { /* ... */ }
```

Примеры работы функции:

```js
let arr = [1, 2, 3, 4, 5];
reverse(arr); // arr = [5, 4, 3, 2, 1]

arr = ["один", "два", "три"];
reverse(arr); // arr = ["три", "два", "один"]
```

Продемонстрируйте работу функции.

### Фильтрация элементов массива

Создайте следующую функцию:

```js
/**
* Возвращает новый массив со всеми элементами, прошедшими проверку,
* задаваемую в передаваемой функции. Если ни один элемент не пройдет
* проверку, то будет возвращен пустой массив.
* 
* Передаваемая функция будет вызываться для каждого элемента массива и должна
* возвращать true или false. Если функция вернёт true, то элемент
* добавится в новый массив, иначе элемент будет пропущен. В функцию будет
* передан один аргумент - текущий проверяемый элемент массива.
* 
* @param {array} arr - Фильтруемый массив.
* @param {function} callback - Функция проверки элементов массива.
* @return {array} Массив со всеми элементами, прошедшими проверку.
*/
function filter(arr, callback) { /* ... */ }
```

Примеры работы функции:

```js
let arr = [-5, 4, 1, 2, 0, -4, -3];
filter(arr, (item) => item % 2 === 0); // [4, 2, 0, -4]

arr = ["Иван", "Алексей", "Дмитрий", "Алиса"];    
filter(arr, (name) => name.length > 6); // ["Алексей", "Дмитрий"]
```

Продемонстрируйте работу функции.

### Строковое представление объекта

Задачи:

1. Создайте переменную `person`.

2. Создайте и сохраните в переменную объект со следующими свойствами:

    - `name` - строка.
    - `surname` - строка.
    - `age` - число.
    
3. Запишите в свойства объекта произвольные данные.
    
4. Добавьте в объект следующий метод:
    
    ```js
    /**
    * Возвращает строковое представление объекта. Принимает один аргумент
    * логического типа, контролирующий отображение свойства age.
    * Аргумент showAge по умолчанию равен false, т.е. по умолчанию возраст
    * не должен отображаться.
    * 
    * Внешний вид строки, в зависимости от значения аргумента showAge:
    * 1. (false, по умолчанию): "<surname> <name>"
    * 2. (true): "<surname> <name>, <age>"
    * 
    * @param {boolean} [showAge=false] - Признак, контролирующий
    * отображение возраста.
    * @return {string} Строковое представление объекта.
    */
    function toString(showAge) { /* ... */ }
    ```
    
    Примеры работы функции:
    
    ```js
    // {name: "Иван", surname: "Иванов", age: 21, toString: f}
    let person = { /* ... */ };
 
    person.toString(); // "Иванов Иван"
    person.toString(showAge=true); // "Иванов Иван, 21"
    ```
    
5. Продемонстрируйте работу функции.

### Конструктор человека

Задачи:

1. Создайте функцию-конструктор для создания объектов того же вида, что и в 
предыдущем подзадании
[строковое представление объекта](#строковое-представnение-объекта):

```js
/**
* Создаёт объект человека следующего вида:
* 
* {
*   name: "Иван",
*   surname: "Иванов",
*   age: 21,
*   toString(showAge) { ... }
* }
* 
* @param {string} name - Имя человека.
* @param {string} surname - Фамилия человека.
* @param {number} age - Возраст человека
* @constructor
*/
function Person(name, surname, age) { /* ... */ }
```

Примеры работы функции:

```js
// {name: "Иван", surname: "Иванов", age: 21, toString: f} 
let person = new Person("Иван", "Иванов", 21);

person.toString(); // "Иванов Иван"
person.toString(showAge=true); // "Иванов Иван, 21"
```

Продемонстрируйте работу функции.

## 10.3. Отложенный вызов функций

### Отложенное приветствие

Создайте следующую функцию:

```js
/**
* Через указанное количество миллисекунд выводит на консоль приветствие
* следующего вида:
* 
* "Привет, <name>!"
* 
* По умолчанию задержка равна 1000 миллисекунд.
* 
* @param {string} name - Приветственное имя.
* @param {number} [delay=1000] - Задержка приветствия, миллисекунды.
*/
function sayHello(name, delay) { /* ... */ }
```

Примеры работы функции:

```js
// Выведет на консоль "Привет, Дмитрий!" через 1 с.
sayHello("Дмитрий");

// Выведет на консоль "Привет, Юля!" через 3 с.
sayHello("Юля", 3000);
```

Продемонстрируйте работу функции.

### Посчитать до десяти

Создайте следующую функцию:

```js
/**
* Выводит на консоль числа от 1 до 10 с указанным интервалом между выводом
* очередного числа. По умолчанию интервал равен 500 миллисекундам.
* 
* @param {number} [delay=500] - Интервал вывода, миллисекунды.
*/
function countToTen(delay) { /* ... */ }
```

Примеры работы функции:

```js
// Выведет на консоль числа от 1 до 10 с интервалом 500 мс.
countToTen();

// Выведет на консоль числа от 1 до 10 с интервалом 1 с.
countToTen(1000);
```

Продемонстрируйте работу функции.

## 10.4. Подключение скриптов к странице и отладка кода в браузере

Задачи:

1. Создайте файл с именем `index.html` и следующим содержимым:

    ```html
    <!DOCTYPE html>
    
    <html lang="ru">
    <head>
      <meta charset="UTF-8">
      <title>Подключение скриптов</title>
    </head>
    
    <body></body>
    
    </html>
    ```

2. Добавьте на страницу следующий скрипт:

    ```js
    /**
    * Возвращает сумму двух значений.
    * 
    * @param {*} first - Первое значение.
    * @param {*} second - Второе значение.
    * @return {*} Сумма значений.
    */
    function add(first, second) {
      let result = first + second;
      return result;
    }
    
    for(let i = 0; i < 10; i++) {
      console.log(i);
    }
    
    let result = add(1, "2");
    console.log(result);
    ```

3. Вынесите скрипт в отдельный файл с именем `main.js`.

4. Откройте страницу в браузере и в инструментах разработчика Chrome
откройте файл `main.js`.

5. Поставьте точки останова на следующие строчки:

    - `let result = first + second;`,
    - `for(let i = 0; i < 10; i++) {`.
    
6. Перезагрузите страницу для начала процесса отладки.

7. Попав на первую точку останова, сделайте следующее:

    - исследуйте содержимое текущего контекста выполнения,
    - добавьте переменную `i` в перечень отслеживаемых выражений,
    - выполните пошагово три итерации цикла, наблюдая,
    как изменяется значение `i`,
    - измените значение переменной `i` на `10`,
    - продолжите пошагово выполнять скрипт до момента выхода из цикла, 
    - восстановите нормальное выполнение скрипта.
    
8. Попав на вторую точку останова, сделайте следующее:

    - исследуйте содержимое текущего контекста выполнения,
    - по содержимому стека вызовов определите место вызова функции,
    - выйдите из текущей функции,    
    - восстановите нормальное выполнение скрипта.

<disqus-comments
  page-uuid="8bc55875-eaaf-43b1-a013-d9d84e05568c"
  page-title="10. Циклы. Функции. Подключение скриптов к странице.
    Отладка кода в браузере | Практические занятия"/>