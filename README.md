# Описание разметки файла README.md
Для описания проектов на GitHub используется README.md, который пишется на языке разметки markdown. Что и как поддерживается расписано ниже.

## Список используемых эмодзи (emoji)

[emoji.md](https://github.com/GnuriaN/format-README.md/blob/master/emoji.md)

:ru: :speech_balloon: :white_check_mark:
## Заголовки
Заголовки задаются значками решётки - сколько их, такого уровня заголовок. Как и в HTML возможен уровень от 1 до 6.

```
# h1 Заголовок
```
# h1 Заголовок
```
## h2 Заголовок
```
## h2 Заголовок
```
### h3 Заголовок
```
### h3 Заголовок
```
#### h4 Заголовок
```
#### h4 Заголовок
```
##### h5 Заголовок
```
##### h5 Заголовок
```
###### h6 Заголовок
```
###### h6 Заголовок


## Списки
#### Маркированный
Задать маркированный список можно несколькими символами:
```
- ul
+ ul
  + ul - для вложенных списков нужно поставить 2 пробела
    + ul - третий уровень
      + ul - четвёртый уровень
        + ul - пятый и т.д.
```
- ul
+ ul
  + ul - для вложенных списков нужно поставить 2 пробела
    + ul - третий уровень
      + ul - четвёртый уровень
        + ul - пятый и т.д.
```
* ul
 * ul
  * ul - если ставить по одному пробелу, то выше второго уровня не подняться
```
* ul
 * ul
  * ul - если ставить по одному пробелу, то выше второго уровня не подняться

#### Нумерованный
Нумерованным спискам безразлично с какого числа вы начнёте его - он начнёт с единицы. Точка после числа обязательна. Работа с вложенностями аналогична маркированному списку.
```
1. Первый уровень 1
  1. Второй уровень 1
    1. Третий уровень 1
      1. Четвертный уровень 1 (но реально это третий 2)
2. Первый уровень 2
2. Первый уровень (должно быть 3)
```
1. Первый уровень 1
  1. Второй уровень 1
    1. Третий уровень 1
      1. Четвертный уровень 1 (но реально это третий 2)
2. Первый уровень 2
2. Первый уровень (должно быть 3)

``` Это работает в Haroopad, но почемуто не работает на Github. А еще если взять код:```
[https://help.github.com/articles/basic-writing-and-formatting-syntax/](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
```
1. Make my changes
  1. Fix bug
  2. Improve formatting
    * Make the headings bigger
2. Push my commits to GitHub
3. Open a pull request
  * Describe my changes
  * Mention all the members of my team
    * Ask for feedback
```
1. Make my changes
  1. Fix bug
  2. Improve formatting
    * Make the headings bigger
2. Push my commits to GitHub
3. Open a pull request
  * Describe my changes
  * Mention all the members of my team
    * Ask for feedback

```То он тоже не работает ^_^ ```

Если же Вам нужно число с точкой, но не нужен список, то можно сделать так:
```
1961\. Текст
```
1961\. Текст

#### Смешанный
Нумерованный и маркированный списки можно смешивать:
```
* ul
  1. ol
  1. ol

1. ol
  * ul
  * ul
```
* ul
  1. ol
  1. ol

1. ol
  * ul
  * ul
 
## Ссылки
Либо просто вставить ссылку, либо дополнительно задать текст ссылки (пробела между скобками быть не должно):
```
http://sabaka.net
[sabaka.net](http://sabaka.net)
```
http://sabaka.net

[sabaka(DOT)net](http://sabaka.net)

Можно выводить через "константу", которую можно задать в любом месте, обычно их задают в конце документа.
```
[Sabaka(DOT)Net]
[Sabaka(DOT)Net]:http://sabaka.net
```
[Sabaka(DOT)Net]
[Sabaka(DOT)Net]:http://sabaka.net


## Цитаты
```
> Цитата
> > Вложенная цитата

> Продолжение цитаты
```
> Цитата
> > Вложенная цитата

> Продолжение цитаты

##Начертание шрифта
```
~~Strikethrough~~
```
~~Strikethrough~~
```
**bold**
```
**bold**
```
*italic*
```
*italic*
```
***bold italic***
```
***bold italic***
```
_italic too_
```
_italic too_

```
**Можно использовать _курсив_ внутри жирного текста.**
```
**Можно использовать _курсив_ внутри жирного текста.**

## Вставки кода
Если нужно выделить слово или фразу внутри строки, то используются одинарные обратные апострофы (`), для выделения в блоки - тройные. Дополнительно можно задавать язык кода внутри блока:
```
Можно использовать `light-code` внутри строки
'''
code block
'''
```

```
code block
```
Можно указать конкретный язык
```
'''C#
using MarkdownSharp;
using MarkdownSharp.Extensions.Mal;

Markdown mark = new Markdown();

// Short link for MAL - 
// http://myanimelist.net/people/413/Kitamura_Eri => mal://Kitamura_Eri
mark.AddExtension(new Articles()); 
mark.AddExtension(new Profile());

mark.Transform(text);
'''
```

```C#
using MarkdownSharp;
using MarkdownSharp.Extensions.Mal;

Markdown mark = new Markdown();

// Short link for MAL - 
// http://myanimelist.net/people/413/Kitamura_Eri => mal://Kitamura_Eri
mark.AddExtension(new Articles()); 
mark.AddExtension(new Profile());

mark.Transform(text);
```

## Вставки изображения
```
![Alt-текст](https://avatars1.githubusercontent.com/u/5384215?v=3&s=460 "Орк")
```
![Alt-текст](https://avatars1.githubusercontent.com/u/5384215?v=3&s=460 "Орк")

## Вставка таблиц
```
| LEFT | CENTER | RIGHT |
|----------------|:---------:|----------------:|
| По левому краю | По центру | По правому краю |
| текст | текст | текст |
```
| LEFT | CENTER | RIGHT |
|----------------|:---------:|----------------:|
| По левому краю | По центру | По правому краю |
| текст | текст | текст |


## Список задач (Task List)
Можно создавать "Списки задач"
```
- [X] Предумать внешний вид резюме.
- [ ] Написать основные категории
- [ ] Опубликовать
- [ ] \(Optional) Open a followup issue
```
- [X] Предумать внешний вид резюме.
- [ ] Написать основные категории
- [ ] Опубликовать
- [ ] \(Optional) Open a followup issue
