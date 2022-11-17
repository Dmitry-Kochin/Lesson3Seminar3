# Туториал по языку разметки Markdown
## Работа с заголовками
Заголовки отмечаются диезом `#` в начале строки, от
одного до шести. Например:
# Заголовок первого уровня #
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6
В декоративных целях заголовки можно «закрывать» с
обратной стороны.

## Работа со списками
Для разметки неупорядоченных списков можно использовать
или `*`, или `-`, или `+`:
- элемент 1
- элемент 2
- элемент ...
Вложенные пункты создаются четырьмя пробелами перед
маркером пункта:
* элемент 1
* элемент 2
 * вложенный элемент 2.1
 * вложенный элемент 2.2
* элемент ...
Упорядоченный список:
1. элемент 1
2. элемент 2
 1. вложенный
 2. вложенный
3. элемент 3
На самом деле не важно как в коде пронумерованы пункты,
главное, чтобы перед элементом списка стояла цифра
(любая) с точкой. Можно сделать и так:
0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4

## Работа с изображениями
бла-бла-бла
Чтобы добавить изображение в MarkDown, используйте следующую конструкцию:
!["Альтернативныйтекст"](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/140-P1020281_-_Flickr_-_Laurie_Nature_Bee.jpg/1280px-140-P1020281_-_Flickr_-_Laurie_Nature_Bee.jpg)
## Работа с таблицами
Для того, чтобы создать таблицу в Markdown, необходимо пойти на следующие "ухищрения". 
Воспользуемся разметкой GFM
В чистом Маркдауне нет синтаксиса для таблиц, а в GFM
есть.
First Header | Second Header
------------- | -------------
Content Cell | Content Cell
Content Cell | Content Cell
Для красоты можно и по бокам линии нарисовать:

|First Header | Second Header |
| ------------- | ------------- |
| Content Cell | Content Cell |
| Content Cell | Content Cell |
Можно управлять выравниванием столбцов при помощи
двоеточия.
| Left-Aligned | Center Aligned | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is | some wordy text | **$1600** |
| col 2 is | centered | $12 |
| zebra stripes | are neat | ~~$1~~ |
Внутри таблиц можно использовать ссылки, наклонный,
жирный или зачеркнутый текст.
Для всего остального есть обычный HTML.
Воспользуйтесь тэгом table:
```HTML
<table><td><tr>drdrdrdrrd</td></tr></table>
```

## Работа со ссылками
Это встроенная ссылка с title элементом (http://example.com/link). Это
— без title (http://example.com/link).
А вот пример (http://example.com/) нескольких
(http://example.com/some) ссылок (http://example.com/links) с
разметкой как у сносок. Прокатит и короткая запись
(http://example.com/short) без указания id.
Вынос длинных урлов из предложения способствует сохранению
читабельности исходника. Сноски можно располагать в любом месте
документа.

## Работа с цитатами
**Цитаты оформляются следующим образом:**


**Цитаты оформляются как в емейлах, с помощью символа >**.
This is a blockquote with two paragraphs. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in,
laoreet vitae, risus.
Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.
Или более ленивым способом, когда знак > ставится перед каждым
элементом цитаты, будь то абзац, заголовок или пустая строка:
This is a blockquote with two paragraphs. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in,
laoreet vitae, risus.
Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.
