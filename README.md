# tt-game
https://github.com/V0l9emar/tt-game_repo

## Игра с картинками, которые надо кликать в хронологическом порядке на время.

## Задания:
### 1. Сверстать рабочий стол с игрой.✅
Прилагается картинка. 
### 2. Сделать динамическое начало игры -
Создать массив. К примеру из 10 элементов текста от 1 до 10. Например : ['1','2', и т.д.].
При нажатии на кнопку "СТАРТ" - динамически сверстать блоки одинакового размера. Пока можно вручную расчитать.
Так, чтобы они поместились внутри игрового поля. Можно окрасить бэкграунд каждого блока в один цвет, чтобы было видно и сделать между ними отступы.
У нас поле определенного размера в высоту и ширину. Кол-во карточек будет всегда разным. Пока можно вручную высчитать максимальный предел этого поля, и определённый размер карточек, чтобы они помещались вместе с отступами, возможно  или добавлять скролл. 
Например так:
![task2](https://user-images.githubusercontent.com/74174349/231150573-e466a9c8-50c4-47f8-8e7f-66f4e1d905b8.png)

Кнопка "СТАРТ" после клика становится неактивной и написано на ней "ИГРА НАЧАТА"
Поиграться разными размерами массивов, разными стилями отображения, и подумать как это оптимизировать потом для атоматического расчёта размеров блоков и отступов, когда кол-во элементов массива будет неизвестным.
### 3. Отработать нажатие на блоки
Нажатие на 1 блок - выплывает сообщение "блок 1 нажат" и т.п.
### 4. Придумать как сохранять прогресс игры (массив или объект)
Например: нажат блок №1  и в массив залетает номер этого блока. Также в этом пункте, как-то помечать эти блоки с помощью CSS (можно к примеру рамочку делать или фон).

![task4](https://user-images.githubusercontent.com/74174349/231150742-92272c83-ed50-4fea-b1cf-3402faa1e81c.png)

### 5. Добавить время ( счётчик ),
Когда нажимаешь клавишу "СТАРТ"  - то начинается отсчет времени. Хранить это время в переменной. Обнулять при старте игры, останавливать при завершении.
### 6. Функцию расчёта оптимального места в игровом поле.
При превышении предела игрового поля высчитывать размер карточек в зависимости от кол-ва.
### 7. Взять картинки с git.door43
Взять url одной  Библейской истории и поключить в проект файл markdown .(https://git.door43.org/ru_gl/rsl_obs/raw/branch/master/15.md)
### 8.Функция рандомного порядка.
Написать функцию, которая рандомно меняет порядок картинок.
### 9. Спарсить картинки из markdown
Вырезать из markdown все ссылки на картинки и добавить их в массив блоков, который рандомно будет верстаться как в пункте 2. Подключить функцию из пункта 8
### 10. Правила игры
Игра успешно завершается, если игрок хронологически правильно нажимает на картинки.
У нас есть массив, куда сохраняются результаты. И есть массив, который следит за очередностью(массив из картинок, спарсенный из markdown)
У каждой картинки есть название и последние 2 цифры - это очередность. Нужно проверять правильно ли хронологически игрок нажимает на эти блоки. К примеру массив который рисуется [{name:picture02.jpg},{name:picture01.jpg},{name:picture03.jpg}]. Отыгравшие блоки делать некликабельными и выделять их
Если игра успешно завершается - кнопка "Старт" становится доступной для начала новой игры, время останавливается и появляется окошко - "Игра успешно завершена, ваше время: 00,00"
Если порядок нарушается - то писать сообщение - "неправильный ответ попробуйте ещё"
### 11. Добавить сохранение результата (время, затраченное на поиск)
Работа с localstorage. Запись и вывод списка лучшего времени рядом с полем игры.

### 12. Усложнить игру -
При неправильном порядке нажатии - заканчивать игру с обнулением результата (не записывать в localstorage))
### 13. Усложнить игру -
Cделать выбор истории с помощью тега "select" ( подсказка - url будет только отличаться названием файла от 01.md до 50.md в url https://git.door43.org/ru_gl/rsl_obs/raw/branch/master/15.md)

### Фото
![Project_Photo](https://github.com/V0l9emar/tt-game/blob/main/img/game.png)
