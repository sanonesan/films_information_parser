# Simple `Scrapy` Parser for movies / films in Python
## Information about films
- Name
- Director
- Country
- Year
- IMDB id
- IMDB rating

## Stack
- Scrapy

## Parsed web-sites
- Wikipedia: Фильмы по алфавиту (link: https://ru.wikipedia.org/wiki/Категория:Фильмы_по_алфавиту)
- IMDB (link: https://www.imdb.com/title/MOVIE_ID_HERE/ratings/)

## Project structure:
```bash
.
├── movie_parser_project
│   ├── films_data.csv
│   ├── movie_parser
│   │   ├── __init__.py
│   │   ├── items.py
│   │   ├── middlewares.py
│   │   ├── pipelines.py
│   │   ├── settings.py
│   │   └── spiders
│   │       ├── films_by_alphabet.py
│   │       └── __init__.py
│   └── scrapy.cfg
├── README.md
└── requirements.txt
```

## Running `Scrapy`-crawler  
To run this code:
1. Install `scrapy`:
```bash
pip3 install scrapy
```
2. In `settings.py` set your `USER_AGENT`.
3. Change dir to `movie_parser_project` and run folowing `bash`-code:
```bash
scrapy crawl films_by_alphabet -o films_data.csv
```
Result is stored in .csv format

## P.S. 
To parse all pages, in file `films_by_alphabet.py` comment variable `custom_settings`.


# Простой парсер на `Scrapy` для информации о фильмах (Python)
## Полученная информация о фильмах
- Название
- Режиссер
- Страна
- Год
- Идентификатор IMDB
- Рейтинг IMDB

## Использованные библиотеки
- Scrapy

## Использованные веб-сайты
- Википедия: Фильмы по алавиту (ссылка: https://ru.wikipedia.org/wiki/Категория:Фильмы_по_алфавиту)
- IMDB (ссылка: https://www.imdb.com/title/MOVIE_ID_HERE/ratings/)

## Структура проекта:
```bash
.
├── movie_parser_project
│   ├── films_data.csv
│   ├── movie_parser
│   │   ├── __init__.py
│   │   ├── items.py
│   │   ├── middlewares.py
│   │   ├── pipelines.py
│   │   ├── settings.py
│   │   └── spiders
│   │       ├── films_by_alphabet.py
│   │       └── __init__.py
│   └── scrapy.cfg
├── README.md
└── requirements.txt
```

## Запуск парсера на `scrapy`
Для запуска кода необходимо:
1. Установить `scrapy`:
```bash
pip3 install scrapy
```
2. В файле `settings.py` установить ваш `USER_AGENT`.
3. Перейти в директорию `movie_parser_project` и запустить следующий `bash`-код:
```bash
scrapy crawl films_by_alphabet -o films_data.csv
```
Результат будет сохранен в csv формате.

## P.S. 
Чтобы не ограничивать время работы парсера, в файле `films_by_alphabet.py` закоментируйте переменную `custom_settings`.


