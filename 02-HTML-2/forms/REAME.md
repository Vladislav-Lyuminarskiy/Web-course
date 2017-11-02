[Назад к описанию занятия](https://github.com/Vladislav-Lyuminarskiy/Web-course/tree/master/02-HTML-2)

[Посмотреть пример на JSFiddle]()

# Формы

Элементы в этом примере:

Элемент                                          | Описание
-------------------------------------------------|-------------------------------------------------
[`<button>`](http://htmlbook.ru/html/button)     | Тег `<button>` создает на веб-странице кнопки и по своему действию напоминает результат, получаемый с помощью тега `<input>` (с атрибутом `type="button | reset | submit"`). В отличие от этого тега, `<button>` предлагает расширенные возможности по созданию кнопок. Например, на подобной кнопке можно размещать любые элементы HTML, в том числе изображения. Используя стили можно определить вид кнопки путем изменения шрифта, цвета фона, размеров и других параметров.<br>Теоретически, тег `<button>` должен располагаться внутри формы, устанавливаемой элементом `<form>`. Тем не менее, браузеры не выводят сообщение об ошибке и корректно работают с тегом `<button>`, если он встречается самостоятельно. Однако, если необходимо результат нажатия на кнопку отправить на сервер, помещать `<button>` в контейнер `<form>` обязательно.
[`<datalist>`](http://htmlbook.ru/html/datalist) | Создает список вариантов, которые можно выбирать при наборе в текстовом поле. Изначально этот список скрыт и становится доступным при получении полем фокуса или наборе текста.
[`<input>`](http://htmlbook.ru/html/input)       | Тег `<input>` является одним из разносторонних элементов формы и позволяет создавать разные элементы интерфейса и обеспечить взаимодействие с пользователем. Главным образом `<input>` предназначен для создания текстовых полей, различных кнопок, переключателей и флажков. Хотя элемент `<input>` не требуется помещать внутрь контейнера `<form>`, определяющего форму, но если введенные пользователем данные должны быть отправлены на сервер, где их обрабатывает серверная программа, то указывать `<form>` обязательно. То же самое обстоит и в случае обработки данных с помощью клиентских приложений, например, скриптов на языке JavaScript.<br>Основной атрибут тега `<input>`, определяющий вид элемента — `type`. Он позволяет задавать следующие элементы формы: текстовое поле (`text`), поле с паролем (`password`), переключатель (`radio`), флажок (`checkbox`), скрытое поле (`hidden`), кнопка (`button`), кнопка для отправки формы (`submit`), кнопка для очистки формы (`reset`), поле для отправки файла (`file`) и кнопка с изображением (`image`). Для каждого элемента существует свой список атрибутов, которые определяют его вид и характеристики. Кроме того, в HTML5 добавлено еще более десятка новых элементов.
[`<fieldset>`](http://htmlbook.ru/html/fieldset) | Элемент `<fieldset>` предназначен для группирования элементов формы. Такая группировка облегчает работу с формами, содержащими большое число данных. Например, один блок может быть предназначен для ввода текстовой информации, а другой — для флажков.<br>Браузеры для повышения наглядности отображают результат использования тега `<fieldset>` в виде рамки. Ее вид зависит от операционной системы, а также используемого браузера.
[`<form>`](http://htmlbook.ru/html/form)         | Тег `<form>` устанавливает форму на веб-странице. Форма предназначена для обмена данными между пользователем и сервером. Область применения форм не ограничена отправкой данных на сервер, с помощью клиентских скриптов можно получить доступ к любому элементу формы, изменять его и применять по своему усмотрению.<br>Документ может содержать любое количество форм, но одновременно на сервер может быть отправлена только одна форма. По этой причине данные форм должны быть независимы друг от друга.<br>Для отправки формы на сервер используется кнопка `submit`, того же можно добиться, если нажать клавишу `Enter` в пределах формы. Если кнопка `submit` отсутствует в форме, клавиша `Enter` имитирует ее использование.<br>Когда форма отправляется на сервер, управление данными передается программе, заданной атрибутом `action` тега `<form>`. Предварительно браузер подготавливает информацию в виде пары `имя=значение`, где имя определяется атрибутом name тега `<input>`, а значение введено пользователем или установлено в поле формы по умолчанию. Если для отправки данных используется метод `GET`, то адресная строка может принимать следующий вид:<br>`http://www.example.com/index.html?name1=value1&name2=value2&name3=value3`<br>Параметры перечисляются после вопросительного знака, указанного после базового адреса и разделяются между собой символом `&` (амперсанд). Нелатинские символы преобразуются в шестнадцатеричное представление (в форме `%HH`, где `HH` — шестнадцатеричный код для значения ASCII-символа), пробел заменяется на `+` (плюс).<br>Допускается внутрь контейнера `<form>` помещать другие теги, при этом сама форма никак не отображается на веб-странице, видны только ее элементы и результаты вложенных тегов.
[`<label>`](http://htmlbook.ru/html/label)       | Тег `<label>` устанавливает связь между определенной меткой, в качестве которой обычно выступает текст, и элементом формы (`<input>`, `<select>`, `<textarea>`). Такая связь необходима, чтобы изменять значения элементов формы при нажатии курсором мыши на текст. Кроме того, с помощью `<label>` можно устанавливать горячие клавиши на клавиатуре и переходить на активный элемент подобно ссылкам.<br>Существует два способа связывания объекта и метки. Первый заключается в использовании идентификатора `id` внутри элемента формы и указании его имени в качестве атрибута `for` тега `<label>`. При втором способе элемент формы помещается внутрь контейнера `<label>`.
[`<legend>`](http://htmlbook.ru/html/legend)     | Тег `<legend>` применяется для создания заголовка группы элементов формы, которая определяется с помощью тега `<fieldset>`. Группа элементов обозначается в браузере с помощью рамки, а текст, который располагается внутри контейнера `<legend>`, встраивается в эту рамку.
[`<optgroup>`](http://htmlbook.ru/html/optgroup) | Тег `<optgroup>` представляет собой контейнер, внутри которого располагаются теги `<option>` объединенные в одну группу. Особенностью тега `<optgroup>` является то, что он не выделяется как обычный элемент списка, акцентируется с помощью жирного начертания, а все элементы, входящие в этот контейнер, смещаются вправо от своего исходного положения.
[`<option>`](http://htmlbook.ru/html/option)     | Тег `<option>` определяет отдельные пункты списка, создаваемого с помощью контейнера `<select>`. Ширина списка определяется самым широким текстом, указанным в теге `<option>`, а также может изменяться с помощью стилей. Если планируется отправлять данные списка на сервер, то требуется поместить элемент `<select>` внутрь формы. Это также необходимо, когда к данным списка идет обращение через скрипты.
[`<select>`](http://htmlbook.ru/html/select)     | Тег `<select>` позволяет создать элемент интерфейса в виде раскрывающегося списка, а также список с одним или множественным выбором, как показано далее. Конечный вид зависит от использования атрибута `size` тега `<select>`, который устанавливает высоту списка. Ширина списка определяется самым широким текстом, указанным в теге `<option>`, а также может изменяться с помощью стилей. Каждый пункт создается с помощью тега `<option>`, который должен быть вложен в контейнер `<select>`. Если планируется отправлять данные списка на сервер, то требуется поместить элемент `<select>` внутрь формы. Это также необходимо, когда к данным списка идет обращение через скрипты.
[`<textarea>`](http://htmlbook.ru/html/textarea) | Поле `<textarea>` представляет собой элемент формы для создания области, в которую можно вводить несколько строк текста. В отличие от тега `<input>` в текстовом поле допустимо делать переносы строк, они сохраняются при отправке данных на сервер.<br>Между тегами `<textarea>` и `</textarea>` можно поместить любой текст, который будет отображаться внутри поля.