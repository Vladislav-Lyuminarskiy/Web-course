[Назад к описанию курса](../README.md)

> **По всем вопросам, возникшим в процессе выполнения производственной практики, можно получить ответ, отправив письмо на почту Vladislav.Lyuminarskiy@gmail.com. В теме письма написать `Web-final` и указать инициалы.**

# Создание веб-сайта с использованием сторонних библиотек

Содержание:
- [Описание производственной практики](#Описание-производственной-практики)
- [Задания](#Задания)
  - [1. Доработка технического задания](#1-Доработка-технического-задания)
  - [2. Доработка макетов страниц](#2-Доработка-макетов-страниц)
  - [3. Доработка веб-сайта с помощью `Bootstrap`](#3-Доработка-веб-сайта-с-помощью-bootstrap)
  - [4. Доработка веб-сайта с помощью `Vue.js`](#4-Доработка-веб-сайта-с-помощью-vuejs)
  - [5. Подготовка отчётности по производственной практике](#5-Подготовка-отчётности-по-производственной-практике)

## Описание производственной практики

При создании веб-сайтов часто возникают ситуации, в которых приходится заново решать одни и те же задачи. Чтобы избежать этой рутины, разработчики создают библиотеки - набор кода, который решает типичные задачи.

В рамках производственной практики предлагается усовершенствовать веб-сайт, созданный в процессе выполнения [второй лабораторной работы](../labs/lab2.md), путём применения следующих сторонних библиотек:

- `Bootstrap`
- `Vue.js`

Эти библиотеки значительно упрощают и ускоряют создание веб-сайтов любой сложности. Они довольно популярны и используются веб-студиями во всему миру. Описание этих библиотек можно найти ниже.

Помимо этих библиотек разрешается использовать любые другие, например: [`jQuery`](https://jquery.com), [`Animate.css`](https://daneden.github.io/animate.css/) и другие.

Общий вид физической структуры веб-сайта:

```
┬(корневой каталог веб-сайта)
├─┬assets
│ └──(медиафайлы)
├─┬pages
│ └──(прочие страницы веб-сайта)
├─┬scripts
│ ├──main.js
│ └──(прочие файлы скриптов)
├─┬styles
│ ├──style.css
│ └──(прочие файлы стилей)
└──index.html (главная страница веб-сайта)
```

## Задания

### 1. Доработка технического задания

ТЗ должно подробно и недвусмысленно описывать требования, предъявляемые к веб-сайту, и его внешний вид. ТЗ и макеты страниц не должны противоречить друг другу, одно должно следовать из другого.

ТЗ должно измениться в сторону усложнения, т.е. ожидается появление новых страниц на веб-сайте, а также требования к поведению веб-сайта (анимации, переходы между страницами, поиск и т.п.).

### 2. Доработка макетов страниц

Создать макеты для новых страниц и доработать уже существующие макеты. Макеты страниц должны соответствовать техническому заданию, быть довольно подробными и наглядными для того, чтобы на их основе создать веб-сайт.

### 3. Доработка веб-сайта с помощью `Bootstrap`

На основе веб-сайта, созданного в процессе выполнения [второй лабораторной работы](../labs/lab2.md), создать новый веб-сайт с использованием библиотеки `Bootstrap`.

`Bootstrap` - библиотека для создания пользовательских интерфейсов. Она позволяет быстро и безболезненно создавать сложные адаптивные пользовательские интерфейсы.

Документацию и примеры использования `Bootstrap` можно найти на [официальном сайте](https://getbootstrap.com), а также на его [русскоязычной версии](http://getbootstrap.ru/docs/v4-alpha/).

### 4. Доработка веб-сайта с помощью `Vue.js`

С помощью библиотеки `Vue.js` доработать веб-сайт, созданный в процессе выполнения предыдущего задания. Необходимо применить механизм шаблонов и создать собственные компоненты.

`Vue.js` - библиотека для создания веб-сайтов. Она предоставляет механизм шаблонов, упрощающий манипулирование элементами DOM, механизм создания переиспользуемых компонентов, обогащающих HTML-разметку, и многое другое.

Документацию и примеры использования `Vue.js` можно найти на [официальном сайте](https://ru.vuejs.org/index.html).

### 5. Подготовка отчётности по производственной практике

Оформить следующие документы:

- отчёт по производственной практике,
- аттестационный лист по производственной практике,
- дневник производственной практики (см. [шаблон](https://docs.google.com/document/d/15exVALQxJCNkgzapwX6NDSJZhSQRjl0OplDvp9YCbzM/edit?usp=sharing)).

Состав отчёта по производственной практике:
- титульный лист (см. [шаблон](https://docs.google.com/document/d/1HogMRk-z7CMOAaytQMERQwJ2K-VUUQyAl3PQr6OiRvs/edit?usp=sharing)),
- содержание,
- задание (на производственную практику),
- техническое задание,
- макеты (скриншоты всех макетов),
- веб-сайт (листинги, скриншоты всех страниц сайта в трёх экземплярах - настольном, планшетном и мобильном).

Соблюдать правила русского языка. Страницы отчёта пронумеровать. Ко всем изображениям и листингам в отчёте добавить поясняющие подписи, например:
- *Рис. 3 - главная страница (вид для мобильных телефонов)*,
- *Исх. код 1 - содержимое файла index.html*.