# :radio: Темизация для проекта iFrame

* http://html.4enki.ru/frame/twb/ — демо онлайн, превью для партнёра «ТаймВеб»;

----

## Как устроено и как использовать?

Стилевой файл-скин с переменными собирается через таск `styles:skin` в `gulpfile.js`. На выходе — файл `dist/assets/styles/style-skin.css`.

Собранный файл важно подключать после базового файла стилей. Пример:

```html
<link href="assets/styles/style.css" rel="stylesheet" />
<link href="assets/styles/style-skin.css" rel="stylesheet" /> <!-- ← подключаем файл-скин после основного файла стилей -->
```

### Как пользоваться?

В файле есть большой список переменных, каждая из которых переопределяет одно CSS-правило для конкретного элемента или блока.

Все элементы и блоки учесть не реально; сейчас описаны только базовые блоки и правила. Всё, что будет из «не стандратного» — доделывается отдельно под каждого из партнёров.

| Переменная                                | За что отвечает                                         |
|-------------------------------------------|---------------------------------------------------------|
| `$headerBackground`                       | цвет заливки шапки                                      |
| `$projectHeaderBackground:`               | цвет фона для шапки проекта                             |
| `$linkColor`                              | цвет ссылок по-умолчанию                                |
| `$inputBackgroundColor`                   | цвет фона для инпута                                    |
| `$inputBorder`                            | рамка для инпута                                        |
| `$inputBorderRadius`                      | радиусы скругления рамки для инпута                     |
| `$inputTextColor`                         | цвет текста в инпуте                                    |
| `$inputPadding`                           | внутренний отступы для инпута                           |
| `$inputFontSize`                          | шрифт для инпута                                        |
| `$inputLineHeight`                        | межстрочный интвервал для шрифта                        |
| `$inputHoverBorderColor`                  |                                                         |
| `$inputFocusBorderColor`                  |                                                         |
| `$labelColor`                             | цвет для Label-элемента                                 |
| `$labelFontSize`                          | размер шрифта Label-элемента                            |
| `$labelMarginBottom`                      | отступ вниз для Label-элемента                          |
