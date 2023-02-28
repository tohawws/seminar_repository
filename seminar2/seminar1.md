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

> ## This is a header.
>
> 1. This is the first list item.
> 2. This is the second list item.
>
> > Вложенная цитата.

