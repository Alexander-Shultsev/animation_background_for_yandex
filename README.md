# Анимация элементов на заднем фоне JavaScrips

Создании анимации элементов на заднем фоне сайта при помощи JavaScript. Задача была реализована в рамках изучения синтаксиса языка JavaScript.
Результат: https://alexander-shultsev.github.io/animation_background_for_yandex/ 

Интересные моменты реализации:
1) Скорость элементов меняется в зависимости от отдалённости мыши относительно центра экрана.
2) Символы в каждом элементе генерируются случайно.
3) Для реализации вращения элемента вокруг своей оси была разработана функция, которая в зависимости от расстояния мыши до центра экрана по осям X и Y возвращала угол относительно центральной горизонтальной оси X. Для её создания использовалась тригонометрическая функция вычисления арктангенса. Также для расчета учитывалось, в какой четверти экрана находится мышка.
4) Каждый элемент является объектом класса, расположенным в массиве. Поскольку после захода элемента за границу экрана необходимо его удалять и создавать новый, было принято решение для оптимизации ресурсов не создавать, а переносить его в новое место, изменяя координаты X и Y.

