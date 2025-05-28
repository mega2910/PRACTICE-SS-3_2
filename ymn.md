start

? умножения через цикл, допустим я хочу result = a * b

new a number      ? что умножаем
new b number      ? насколько умножаем
new result number ? Ответ
new i number      ? счётчик для цикла loop

? Пример хотим 7 умножить на 5
set a 7
set b 5

? подготовка к циклу
set result 0
set i 0

? Цикл + a, b раз
loop ymn (b > i)
    set result result + a
    set i i + 1
end ymn

? Вывод результата
log number result

finish
