[Назад к описанию занятия](https://github.com/Vladislav-Lyuminarskiy/Web-course/tree/master/04-CSS-1)

# Добавление стилей на веб-страницу

Определение стиля состоит из селектора (указывает, к каким элементам будет применяться стиль) и блока объявления стиля.

Блок объявления стиля заключён в фигурные скобки и состоит из команд, отделяемых между собой точкой с запятой. Каждая команда состоит из свойства и значения.

Рассмотрим определение стиля:

```css
div {
    color: red;
}
```

Здесь `div` - селектор, `color` - свойство, `red` - значение.

Группу таких определений стилей называют <abbr title="Cascading Style Sheets">CSS</abbr> (каскадные таблицы стилей).

Способы добавления стилей на веб-страницу:
- Для одного элемента с помощью универсального атрибута [style](http://htmlbook.ru/html/attr/style).
- Для всей веб-страницы с помощью элемента [style](http://htmlbook.ru/html/style).
- Для всей веб-страницы через внешний файл с помощью элемента [link](http://htmlbook.ru/html/link).

[Посмотреть пример на JSFiddle](https://jsfiddle.net/Vladislav_Lyuminarskiy/su5jbagp/)