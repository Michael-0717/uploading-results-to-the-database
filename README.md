# Загрузка результатов в БД.
## Задание:
Соберите данные о моделях холодильников Саратов с маркетплейса beru.ru: URL, название, цена, размеры, общий объем, объем холодильной камеры.
Создайте соответствующие таблицы в SQLite базе данных и загрузите полученные данные в таблицу beru_goods.
Для парсинга можно использовать зеркало страницы beru.ru с результатами для холодильников Саратов по адресу:
video.ittensive.com/data/018-python-advanced/beru.ru/
___
## Решение:
1) Подключаем необходимые библиотеки и заходим на зеркало страницы beru.ru с результатами для холодильников Саратов.
2) Получаем  html с этой страницы, инициируя объект BeautifulSoup.
3) Используем тег 'table', его id = 'marketDataList'
4) Производим поиск по параметрам холодильников.
5) Форимруем список [link, title, price, width, depth, height, volume, freezer].
6) Перебираем ссылки, ищем ссылки с "Саратов".
7) Создаём таблицу, заносим данные.
8) Закомитем результат.




