# Дополения к языку разметки MD.

## Оглавление:
1. [Детализация (кат)](#Детализация-кат)
2. [Форматирование текста](#Форматирование-текста)
3. [Имитация клавиатуры](#Имитация-клавиатуры) 
4. [Бэйджики](#Бэйджики)

## Детализация (кат) 
Существует возможность спрятать часть текста под кат. Для этого необходимо использовать тэг HTML5 `<details>` текст `</details>`. Подробнее: [http://htmlbook.ru/html/details](http://htmlbook.ru/html/details) и [http://htmlbook.ru/html/summary](http://htmlbook.ru/html/summary)   
Следующий код:   
    `<details>`    
    `<summary>Подробнее ...</summary>`    
    `Тут текст который вы хотим скрыть`    
    `</details>`   

Дает такой результат:
<details>
<summary>Подробнее ...</summary>
Тут текст который вы хотим скрыть
</details>    
    
    
**Внимание:** это не работает большенстве браузеров.    
[:arrow_up:Оглавление](#Оглавление)    
___

## Форматирование текста
Для форматирования текста можно использовать тэг `<p>`. Подробнее: [http://htmlbook.ru/html/p](http://htmlbook.ru/html/p)   
Варинт использования: `<p align="left | center | right | justify">...</p>`    
<details>
<summary>Текст без форматирования:</summary>
Текст (от лат. textus — «ткань; сплетение, связь, сочетание») — зафиксированная на каком-либо материальном носителе человеческая мысль; в общем плане связная и полная последовательность символов.
</details>
Результат применения тэга:

```
<p align="justify">

</p>
```

<details>
<summary>Текст после форматирования:</summary>
<p align="justify">
Текст (от лат. textus — «ткань; сплетение, связь, сочетание») — зафиксированная на каком-либо материальном носителе человеческая мысль; в общем плане связная и полная последовательность символов.
</p>
</details>    
    
[:arrow_up:Оглавление](#Оглавление)
___

## Имитация клавиатуры
Можно имитировать клавиатуру:
```
<pre>
    <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Esc</kbd> - Высов диспетчера задач
</pre> 
```
<pre>
    <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Esc</kbd> - Вызов диспетчера задач.
</pre>

[:arrow_up:Оглавление](#Оглавление)
___

## Бэйджики

Сожно вставлять сви или готовые бэйджки.
Источник: [https://shields.io/category/build](https://shields.io/category/build)

Пример:
```
Status: ![https://img.shields.io/badge/Status-WIP-red](https://img.shields.io/badge/Status-WIP-red) ![https://img.shields.io/badge/Realese-No-red](https://img.shields.io/badge/Realese-No-red)

Language: ![https://img.shields.io/badge/Python-3.7.5-blue](https://img.shields.io/badge/Python-3.7.5-blue)
```

Результат:  
Status: ![https://img.shields.io/badge/Status-WIP-red](https://img.shields.io/badge/Status-WIP-red) ![https://img.shields.io/badge/Realese-No-red](https://img.shields.io/badge/Realese-No-red)

Language: ![https://img.shields.io/badge/Python-3.7.5-blue](https://img.shields.io/badge/Python-3.7.5-blue)


