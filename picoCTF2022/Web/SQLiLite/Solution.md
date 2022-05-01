# SQLiLite

The challenge is the following,
___
Задача заключается в следующем,

![image](https://user-images.githubusercontent.com/60939699/160276977-7260df90-ea65-4aa7-aad4-486c0ad22c74.png)

Here, after launching *instance*, we get a link to the site with an authorization form.

Judging by the name, we need to use SQL injection and, apparently, one of the simplest.
___
Здесь после запуска *instance* мы получаем ссылку на сайт с формой авторизации.

Судя по названию нам нужно использовать SQL-инъекцию и судя по-всему одну из простейших.

![image](https://user-images.githubusercontent.com/60939699/160276995-6cf64a46-74a7-4990-aeec-d5970de75d1a.png)

To begin with, we enter the string - **' or 1 = 1 --** into the login, the password is required, so we write anything.

Click the **Login**
___
Вводим для начала в логин строку - **' or 1 = 1 --**, пароль обязателен, так что пишем что угодно.

Жмем кнопку **Login**

![image](https://user-images.githubusercontent.com/60939699/160277026-ac1743ab-bbe7-4f5a-87a4-b245b59c7118.png)

After that we get the following answer:
___
После чего получаем следующий ответ:

![image](https://user-images.githubusercontent.com/60939699/160277035-80363630-7b61-4baf-94bb-87656365d537.png)

We got access, but there is no flag yet, but there is a hint that it is somewhere here.

The first thing that comes to mind is to open the code of the page where we can see the **<p>** tag with the **hidden** parameter, that is, hidden, revealing its contents we see the flag and take it away.
___
Доступ мы получили, но флага еще нет, зато есть подсказка, что он где-то тут.

Первое что приходит в голову - открыть код страницы, где мы можем увидеть тег **<p>** с параметром **hidden**, то есть скрытый, раскрыв его содержимое видим флаг и забираем его.

![image](https://user-images.githubusercontent.com/60939699/160277057-1ed459f7-86b3-499b-a33f-527977d2121a.png)
