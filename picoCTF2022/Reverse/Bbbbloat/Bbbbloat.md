# Bbbbloat

The challenge is the following,
___
Задача заключается в следующем,

![img](https://user-images.githubusercontent.com/60939699/166116624-cd0622ff-245c-4db3-89fa-3d9193d5c270.png)

We are given an executable file (attached) in the **.elf** format. Having studied the processes taking place in the program using *GHydra*, you can understand that the key has a fixed and generated in the file itself.
Open the debugger **edb** and open our file with it. Scroll down to the entry point of the program.
___
Нам дается исполняемый файл (прилагается) формата **.elf**. Изучив процессы происходящие в программе при помощи *GHydra* можно понять, что ключ имеет фиксированную и генерируемую в самом файле.
Открываем дебаггер **edb** и открываем им наш файл. Пролистываем lj точки входа в программу.

![img](https://user-images.githubusercontent.com/60939699/166116457-6c131848-d3f1-4c92-a7c6-749f559ce83b.jpg)

They are asking for a key from us. We don't know it, so we'll try to find it inside the program code to understand what it compares to. Enter a random string and press **ENTER**.
Flipping through and simultaneously studying the contents of the registers. At some point we see the beginning of the flag, so we are on the right way.
___
От нас просят ключ. Мы его не знаем поэтому попробуем найти его внутри кода программы чтобы понять с чем он сравнивается. Вводим случайную строку и жмем **ENTER**.
Листаем и попутно изучаем содержимое регистров. В какой-то момент видим начало флага, значит мы на верном пути.

![img](https://user-images.githubusercontent.com/60939699/166116458-50eaf9aa-124e-424a-beb3-9fb0e5ead0c7.jpg)

Click to track the memory dump by the output beginning of the key.
We continue to scroll further, now watching the register and dump.
Further, after 10-15 minutes of persistent pressing on **F7**, we see how characters begin to be appended to the line with the beginning of the key, now we carefully scroll through so as not to miss the end of string generation, because after exiting the key creation operation, we will exit the current dump section.
___
Жмем отслеживать дамп памяти по выведенному началу ключа.
Продолжаем листать дальше теперь наблюдая за регистром и дампом.
Далее минут через 10-15 упорного нажатия на **F7** мы видим как к строке с началом ключа начинают дописываться символы, теперь аккуратно листаем чтобы не пропустить окончание генерации строки, ибо после выхода из операции создания ключа мы выйдем из текущего раздела дампа.

![img](https://user-images.githubusercontent.com/60939699/166116461-a17c0955-5ab4-46c0-9984-6bc77eec840b.jpg)

That's our key, as soon as the process of creating it ends, we will immediately return to the process of comparing the value we entered.
___
Вот и наш ключ, как только кончится процесс его создания нас сразу вернет к процессу сравнения введенного нами значения.

![img](https://user-images.githubusercontent.com/60939699/166116462-0dca96d8-d16c-4902-a94b-3c0fb7c19219.jpg)

The program will say that we entered the wrong key, which is logical, because we didn't know it. We are trying to enter a flag on the site, it is suitable, so this is the end of the solution.
___
Программа скажет, что мы ввели неверный ключ, что логично, ведь мы его не знали. Пробуем ввести флаг на сайте, он подходящий, так что на этом решение заканчивается.

