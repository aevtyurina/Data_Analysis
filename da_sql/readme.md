# Анализ книжного рынка (SQL)

## Данные

В нашем распоряжении 5 таблиц:

books - содержит данные о книгах:

- book_id — идентификатор книги;
- author_id — идентификатор автора;
- title — название книги;
- num_pages — количество страниц;
- publication_date — дата публикации книги;
- publisher_id — идентификатор издателя.

authors - содержит данные об авторах:

- author_id — идентификатор автора;
- author — имя автора.

publishers - содержит данные об издательствах:

- publisher_id — идентификатор издательства;
- publisher — название издательства;

ratings - содержит данные о пользовательских оценках книг:

- rating_id — идентификатор оценки;
- book_id — идентификатор книги;
- username — имя пользователя, оставившего оценку;
- rating — оценка книги.

reviews - содержит данные о пользовательских обзорах на книги:

- review_id — идентификатор обзора;
- book_id — идентификатор книги;
- username — имя пользователя, написавшего обзор;
- text — текст обзора.
  
## Задача

Компания решила быть на волне и купила крупный сервис для чтения книг по подписке. Основная цель исследования — проанализировать базу данных. В ней — информация о книгах, издательствах, авторах, а также пользовательские обзоры книг. Эти данные помогут сформулировать ценностное предложение для нового продукта.

Исследование будет состоять из нескольких задач-пунктов:

- Посчитайть, сколько книг вышло после 1 января 2000 года;
- Для каждой книги посчитайть количество обзоров и среднюю оценку;
= Определитб издательство, которое выпустило наибольшее число книг толще 50 страниц — так вы исключите из анализа брошюры;
- Определить автора с самой высокой средней оценкой книг — учитывайте только книги с 50 и более оценками;
- Посчитайть среднее количество обзоров от пользователей, которые поставили больше 48 оценок.

## Используемые библиотеки
*pandas*, *sqlalchemy* (*text*, *create_engine*), *SQL*
