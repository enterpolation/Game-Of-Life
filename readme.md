# Игра "Жизнь"

Игру «Жизнь» изобрел математик Джон Хортон Конвей в 1970 году. Она пользовалась 
популярностью не только среди его коллег. Об увлекательности игры «Жизнь» свидетельствуют 
результаты множества интересных исследований и многочисленные компьютерные реализации. 
При этом она имеет непосредственное отношение к перспективной области математики --
теории клеточных автоматов.

Правила игры «Жизнь» достаточно простые:
- «Жизнь» разыгрывается на бесконечном клеточном поле.
- У каждой клетки 8 соседних клеток.
- В каждой клетке может жить существо.
- Существо с двумя или тремя соседями выживает в следующем поколении, иначе погибает от 
  одиночества или перенаселённости.
- В пустой клетке с тремя соседями в следующем поколении рождается существо.

Подробнее про игру «Жизнь» можно прочитать в журнале 
[Квант](http://kvant.mccme.ru/1974/09/igra_zhizn.htm).

## Возможности

Настройки игры задаются в конструкторе класса `Game`:

- `height`, `width` - высота и ширина окна в пикселях;
- `cell_size` - размер клетки в пикселях;
- `cell_state` ('custom', 'random') - рандомный / кастомный паттерн;
- `fps` - количество кадров в секунду.

При выборе рандомного паттерна игра начинается сама, при кастомном паттерне 
необходимо
выбрать клетки с помощью `ЛКМ`, а затем нажать `ПРОБЕЛ`. Игрок может в любой момент 
останавливать игру с помощью клавиши `ПРОБЕЛ` и изменять паттерн. Чтобы начать игру, 
необходимо запустить скрипт `main.py`.