# Домашнее задание - Использование браузерных DevTools - анализ сайта

## Вкладка Network

### Записать и сохранить в HAR архив профиль загрузки ресурсов при открытии страницы

Профиль по ссылке https://github.com/Postamentovich/tooling/blob/master/lifehacker.ru-network-profile.har

### Найти неоптимальные места:

- дублирование ресурсов <br>

publishertag.js - загружается два раз подряд
![alt text](/assets/2.png)

- лишний размер ресурса <br>

изображения без сжатия
![alt text](/assets/1.png)

- медленно загружающиеся ресурсы <br>

логотип медленно загружается для своего размера
![alt text](/assets/3.png)

- ресурсы, блокирующие загрузку

Изображения суммарным объемом 2,7мб блокирует загрузку почти на 2с
![alt text](/assets/4.png)

## Вкладка Performance

### записать и сохранить в файл профиль загрузки страницы

Профиль по ссылке https://github.com/Postamentovich/tooling/blob/master/lifehacker.ru-performance-profile.json

### измерить время в миллисекундах от начала навигации до событий First Paint, First Meaningful Paint, DOM Content Loaded, Load

![alt text](/assets/5.png)
![alt text](/assets/6.png)
![alt text](/assets/7.png)
![alt text](/assets/8.png)

### измерить, сколько времени в миллисекундах тратится на разные этапы обработки документа (Loading, Scripting, Rendering, Painting)

![alt text](/assets/9.png)

## Вкладка Coverage

### сохранить скриншот вкладки после загрузки страницы

Только 1,4 МB из 3,1 МB (44%) используется
![alt text](/assets/10.png)

### измерить в килобайтах объём неиспользованного CSS в ходе загрузки страницы

Только 52,4 KB из 443 KB (12%) используется. Большинство файлов совсем не используется
![alt text](/assets/11.png)

### измерить в килобайтах объём неиспользованного JS в ходе загрузки страницы

Только 1,3 МB из 2,7 МB (50%) используется
![alt text](/assets/18.png)

## Вкладка Audit

![alt text](/assets/12.png)