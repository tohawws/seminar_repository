# Создаём туториал по Git

## Как добавить файл на отслеживание

Чтобы добавить файл на отслеживание, используйте команду:

```
 git add <имя_файла.расширение>
```

## Как добавить переключение между коммитами

Чтобы добавить переключение между коммитами, добавте следующию команду:

```
git checkout <хеш-код_коммита>
```

или же:

```
git switch <хеш-код_коммита>
```

Можно вводить первые 4-5 символов хеш-кода для перехода к нему.

## Как получить текущию информацию от Git о статусе файла

Для того чтобы получить информацию в каком состоянии находится файл нужно ввести команду:

```
git status
```

## Как записать commit в репозиторий

Для того чтобы записать commit нужно ввести команду:

```
git commit -m "message"
```

## Как посмотреть всю историю записанных коммитов

Для того чтобы вывести на экран историю всех коммитов с их хеш-кодом, нужно ввести команду:

```
git log
```

или же:

```
git reflog
```

## Как посмотреть разницу текущего файла с "закоммиченным" файлом

Для того чтобы увидеть внесенные не закомичиные строчки текста или же кода, нужно ввести команду:

```
git diff
```

## Для создания новой директории и файла

Для того чтобы создать новую директорию, вводим команду:

```
mkdir <название_папки>
```

Для того чтобы создать новый файл, вводим команду:

```
touch <имя_файла.расширение>
```

# Краткая инструкция по Markdown

## Цитаты

Внутри таблиц можно использовать ссылки, наклонный,
жирный или зачеркнутый текст.
Для всего остального есть обычный HTML.
Цитаты оформляются как в емейлах, с помощью символа `>`.
> This is a blockquote with two paragraphs. Lorem ipsum
dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in,
laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Или более ленивым способом, когда знак `>` ставится
перед каждым элементом цитаты, будь то абзац, заголовок
или пустая строка:

> This is a blockquote with two paragraphs. Lorem ipsum
dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet
vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

В цитаты можно помещать всё что угодно, в том числе
вложенные цитаты:

> ## This is a header
>
> 1. This is the first list item.
> 2. This is the second list item.
>
> > Вложенная цитата.

## Ссылки

Это встроенная [ссылка с tittle элементом](http://example.com/link "Я ссылка"). Это — [без title](http://example.com/link).
А вот [пример][1] [нескольких][2] [ссылок][id] с
разметкой как у сносок. Прокатит и [короткая запись][]
без указания id

[1]: http://example.com/ "Optional Title Here"
[2]: http://example.com/some
[id]: http://example.com/links (Optional Title Here)
[короткая запись]: http://example.com/short

Вынос длинных узлов из предложения способствует
сохранению читабельности исходника. Сноски можно
располагать в любом месте документа.

## Исохдный код

В чистом Маркдауне блоки кода отбиваются 4 пробелами в
начале каждой строки.
Но в GitHub-Flavored Markdown (сокращенно GFM) есть
более удобный способ: ставим по три апострофа (на букве
Ё) до и после кода. Также можно указать язык исходного
кода.

```html
<nav class="nav nav-primary">
    <ul>
        <li class="tab-conversation active">
            <a href="#" data-role="post-count" class="publ
isher-nav-color" data-nav="conversation">
        <span class="comment-count">0 комментариев</
span>
        <span class="comment-count-placeholder">Комм
ентарии</span>
      </a>
    </li>
    <li class="dropdown user-menu" data-role="logou
t">
      <a href="#" class="dropdown-toggle" data-toggl
e="dropdown">
        <span class="dropdown-toggle-wrapper">
          <span>
            Войти
          </span>
        </span>
        <span class="caret"></span>
      </a>
    </li>
  </ul>
</nav>
```

## Таблицы

В чистом Маркдауне нет синтаксиса для таблиц, а в GFM
есть.
First Header | Second Header
------------- | -------------
Content Cell | Content Cell
Content Cell | Content Cell

Для красоты можно и по бокам линии нарисовать:

 First Header | Second Header |
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
