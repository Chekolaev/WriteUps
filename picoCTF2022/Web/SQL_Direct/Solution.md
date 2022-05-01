# SQL Direct

The challenge is the following,
___
Задача заключается в следующем,

![image](https://user-images.githubusercontent.com/60939699/160280696-6a2f54a0-eceb-4f3b-9277-137ab9372ec6.png)

Here we get a string to connect using netcat and a password.

Launching our **instance**. We enter the kali linux command into the command line, then we are required to enter a password.

After authorization, we see that we have connected to the psql 14.2 server on Debian.

Next, we work on the principle of a white box.

Enter the command **\dt** and the server returns us a list of relationships. Here we can see a table with the name **flags**. Now we need to look at contents.

We write a regular SQL query to the table to output everything that is inside. It looks like this: *SELECT * FROM flags* and press *Enter* and nothing happened, because to execute a query to the database, we have to send a command that will execute our last query - *\g*.

We get a table in the console where our flag is in the first row in the *address* attribute.
___
Здесь мы получаем строку для подключения с использованием netcat и пароль.

Запускаем наш **instance**. Вводим в командную строку kali linux команду, затем от нас требуют пароль.

После авторизации видим, что подключились к серверу psql 14.2 на Debian.

Далее работаем по принципу белого ящика.

Вводим команду **\dt** и сервер возвращает нам список отношений. Здесь мы можем видеть таблицу с названием **flags**. Теперь нам надо посмотреть ее содержимое.

Пишем обычный SQL-запрос к таблице для вывода всего, что есть внутри. Выглядит она следующим образом *SELECT * FROM flags* и жмем *Enter* и ничего не произошло, потому что для выполнения запроса в базу данных мы должны отправить команду которая выполнит наш последний запрос - *\g*.

Мы получаем в консоли таблицу, где в первой строке в атрибуте *address* лежит наш флаг.

![image](https://user-images.githubusercontent.com/60939699/160281026-0503b8da-b1ac-4482-89a0-c2746d71f74a.png)
