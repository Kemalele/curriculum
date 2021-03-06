# Integer, float, string
В Python, как и во многих языках программивания есть несколько типов данных: 
- integer - целые цисла (-110001, -10, 0, 15, 1000001)
- float - вещественные числа (-1001,10, -1,00, 0, 3.14159265358, 3.333, 111111)
- string - строки ("", "hello", etc.)

### Числа
С числами можно делать все стандартные математические операции, +, -, /, \*, а также //, **.

Стоит заметить, что деление оператором **/** делит без остатка, т.е. 9 / 2 = 4, округление идет в нижнюю сторону.   
Чтобы делить с остатком, нужно использовать оператор //, т.е. 9 // 2 = 4.5   
Оператор ** означает возведение в степень, т.е. 3**4 = 81  

### Строки 
Строки состоят из букв, и к каждой из этих букв можно обратиться если знать порядковый номер буквы в строке. Например, слово str = "Hello, World!" состоит из 13 букв, 
и так как отсчет в строках начинается с **0**, к букве 'H' можно обратиться с помощью str[0], к последнему элементу строки можно обратиться str[12], заметь что индекс последнего
элемента на 1 меньше чем размер строки, так как отчет начинается с **0**.   
К элементам строки можно обращаться чтобы получить информацию, но изменять ее нельзя, так как строки в Python неизменяются.

Со строками можно проводить операции "+", "*", "in", "not in", [:]  
<a href="https://www.tutorialsteacher.com/python/python-string" target="_blank">Подробнее расписано тут.</a>   


**Обязательно посмотри видео по присвоению переменной других переменных.**   
<iframe width="100%" height="315" src="https://www.youtube.com/embed/_OZIAHg5i7M" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<a href="https://www.tutorialsteacher.com/python/python-data-types" target="_blank">Полезная ссылка</a> по данной теме с иллюстрациями.


<a href="https://www.tutorialsteacher.com/python/python-string" target="_blank">Примеры использования.</a>  


Слабая типизация  
Python является слабо типизированным языком программирования, это означает что если переменная содержала в себе некий тип данных, ничего ей не мешает присвоить другой тип данных, например:  


<iframe height="400px" width="100%" src="https://repl.it/@SakenMukanov/TenseCarefreeCubase?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>


В данной программе нет ничего криминального, Python позволяет такие операции. 


**Для успешной сдачи данного урока, напиши код:**

- <a href="https://github.com/alem-classroom/student-python-introduction-${GITHUB_LOGIN}/blob/master/variables-and-types" class="repo-button">Калькулятора</a>   

- <a href="https://github.com/alem-classroom/student-python-introduction-${GITHUB_LOGIN}/blob/master/variables-and-types" class="repo-button">Управления строками</a>   


Если Github возвращает 404 ошибку, тебе нужно зарегистрироваться в <a href="https://classroom.github.com/a/c9J3nA9U">Github classroom</a>   
   
