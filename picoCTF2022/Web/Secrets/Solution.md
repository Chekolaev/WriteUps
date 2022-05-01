# Secrets

The challenge is the following,
___
Задача заключается в следующем,

![image](https://user-images.githubusercontent.com/60939699/160278324-168f0b83-4d67-4ba9-aa02-1a45d630873b.png)

Where we are given [link](http://saturn.picoctf.net:49917/) to a site where you can see three pages, with a detailed study of which there is nothing useful in the content, after checking the site files there is also nothing, but there is a slight oddity. In the main section of the site there is a link to the resources in which index.css lies, namely in the **secret/assets** section. But this is the direct name of the folder in the **sourse** section, that is, there is no **secret** folder.
___
Где нам дается [ссылка](http://saturn.picoctf.net:49917/) на сайт на котором можно видеть три страницы, при детальном изучении которых ничего полезного в содержимом нет, проверив файлы сайта тоже ничего нет, но есть небольшая странность. В головном разделе сайта есть ссылка на ресурсы в которых лежит index.css, а именно в разделе **secret/assets**. Но это прямое название папки в разделе **sourse**, то есть нет папки **secret**.

![image](https://user-images.githubusercontent.com/60939699/160278347-0fc10cd0-1004-4577-9955-b60d3b689145.png)

Trying to access the **secret** folder. Just add */secret/* to the address bar and see what happens.
___
Пробуем получить доступ к папке **secret**. Просто добавим в поисковую строку */secret/* и посмотрим что из этого выйдет.

![image](https://user-images.githubusercontent.com/60939699/166116212-dc17d87a-6486-4355-8017-3dc6ddac07fe.png)

As it turned out, there is such a section and it says that we are on the right way. Next, we proceed in approximately the same way and look for directories further in the **head** section or page files. We see the **hidden** section in which *css* from this page we try to add it to the address bar.
___
Как оказалось такой раздел есть и в нем говорится, что мы на верном пути. Далее действем примерно тем же путем и ищем директории дальше в разделе **head** или файлах страницы. Видим раздел **hidden** в котором лежит *css* от этой страницы и пробуем его добавить в адресную строку.

![image](https://user-images.githubusercontent.com/60939699/160278367-5d659188-afe2-42ca-aa24-c0472cd7c929.png)

We get access to the next page. Next, we try to repeat the action and go to the **superhidden** section.
___
Получаем доступ к следующей странице. Далее пробуем повторить действие и переходим в раздел **superhidden**.

![image](https://user-images.githubusercontent.com/60939699/160278415-bff7c269-cdbd-448a-a5ae-b7e1a0d0c0b8.png)

The website says that we have found the flag, but it still needs to be seen. Open the page code and look, our flag is immediately under the notification of the location.
___
Сайт говорит, что флаг мы нашли, но его еще надо увидеть. Открываем код страницы и смотрим, наш флаг сразу под уведомлением о нахождении.

![image](https://user-images.githubusercontent.com/60939699/160278423-91f1f4af-b301-4311-9553-963342765c55.png)

We can copy it directly from the page code or highlight it on the page itself.
___
Можем скопировать его прямо из кода страницы или выделить на самой странице.

![image](https://user-images.githubusercontent.com/60939699/160278444-5caa9391-8ae7-4d47-bdea-7412ee4b1064.png)
