
start

? Функция деления через цикл: quot = a / b и rem = a % b
? Входные параметры: a — делимое, b — делитель
? Результат: переменная quot содержит частное, rem — остаток

new a number       ? что делим
new b number       ? на что делим
new quot number    ? результат
new rem number     ? остаток от деления %
new i_div number   ? помощник для цикла

? Пример
set a 37
set b 5

? Подготовка к самому loop
set quot 0
set rem a          ? сохраняем то, что делим в rem
set i_div 0
new temp number

? Цикл вычитания b из rem, считая количество вычитаний (quot)
loop div_loop (rem > i_div)
    ? проверяем, чтобы rem был больше b, т.к. если нет, то пора нам сворачиваться уже (наши вычисления)
    set temp rem
    set temp temp - b
    if (temp > -1)
        set rem temp
        set quot quot + 1
    close
    set i_div i_div + 1
end div_loop

? Вывод
log string "Частное: " >> quot
log string "Остаток: " >> rem

finish
