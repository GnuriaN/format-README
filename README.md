# Описание разметки файла README.md
Для описания проектов на GitHub используется README.md, который пишется на языке разметки аля - markdown. Что и как поддерживается расписано ниже.

1. Заголовки [Заголовки.md](https://github.com/GnuriaN/format-README.md/blob/master/Заголовки.md)
2. Выделение текста [ВыделениеТекста.md](https://github.com/GnuriaN/format-README.md/blob/master/ВыделениеТекста.md)
3. Подсветка кода [ПодсветкаКода.md](https://github.com/GnuriaN/format-README.md/blob/master/ПодсветкаКода.md)
4. Списки [Списки.md](https://github.com/GnuriaN/format-README.md/blob/master/Списки.md)
5. 

 
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
