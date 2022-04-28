The challenge is the following,
---
Задача заключается в следующем,

![image](https://user-images.githubusercontent.com/60939699/160278956-66ae3d19-9d3e-48c2-b232-2cd269afa4d2.png)

Where we are also given [link](http://saturn.picoctf.net:64710/) to a resource for research.
It looks like a regular landing page, there is nothing unusual both in the content of the page itself and inside the contents of all files. It uses of the same name as the task name.
The key to the solution lies in the name of the challenge. For those who are familiar with web pages, it is no secret that many sites have a text file containing site indexing parameters for search engine robots, which is called ***Robots.txt*** . The first thing that comes to mind based on the name of the task is to check if such a file exists.
---
Где нам так же дается [ссылка](http://saturn.picoctf.net:64710/) на ресурс для исследования.
Выглядит как обычный сайт-визитка, ничего необычного как в содержимом самой страницы, так и внутри содержимого всех файлов. В нем используется шрифт одноименный названию задания.
Подсказка к решению лежит в названии к заданию. Для тех кто знаком с web-страницами - не секрет, что у многих сайтов существует текстовый файл, который содержит параметры индексирования сайта для роботов поисковых систем, который называется ***Robots.txt***. Первым, что приходит в голову исходя из названия задания - проверить есть ли такой файл.

![image](https://user-images.githubusercontent.com/60939699/160278982-fee7fb5b-e132-405d-a2c8-16803f956c56.png)

And there is such a page, which means, most likely, we are moving in the right direction.
After examining the content, you can see a comment that we have either already seen the flag, or we want to continue the search.
Then there are lines with seemingly incomprehensible content. At the end of one of the lines on **==** we can understand that it is ***base64***.
Open the decoder of this encoding.
---
И такая страница есть, а значит,скорее всего, мы движемся в верном направлении.
Изучив содержимое, можно увидеть комментарий, что флаг мы либо уже видели, либо хотим продолжить искать.
Далее идут строки с непонятным на первый взгляд содержимым. По окончанию одной из строк на **==** мы можем понять, что это ***base64***.
Открываем расшифровщик этой кодировки.

![image](https://user-images.githubusercontent.com/60939699/160279579-003adb6e-ab98-4f68-ae23-e002f2427a17.png)


![image](https://user-images.githubusercontent.com/60939699/160279570-b1e19e8a-ef50-4ab8-980f-038385da2140.png)
