# Космический Телеграм


Программа скачивает картинки на околокосмическую тематику с сайтов SPACEX и NASA
и публикует их в телеграм канал


## Как установить

Python3 должен быть уже установлен. Затем используйте pip (или pip3, есть есть конфликт с Python2) для установки зависимостей:

```
pip install -r requirements.txt
```

Необходимо зарегистрировать бота и получить токен для доступа к API Телеграма. 
Подробная инструкция [как зарегистрировать бота](https://way23.ru/%D1%80%D0%B5%D0%B3%D0%B8%D1%81%D1%82%D1%80%D0%B0%D1%86%D0%B8%D1%8F-%D0%B1%D0%BE%D1%82%D0%B0-%D0%B2-telegram.html)


## Переменные окружения

Создайте в папке проекта файл .env и положите в него переменные по образцу:
* NASA_API_KEY=ключ для API NASA
* TG_BOT_TOKEN=токен бота, публикующего телеграм картинки
* TG_CHAT_ID=id канала, где будут публиковаться картинки
* POSTING_INTERVAL=интервал публикации картинок(в секундах)

## Запустить

Скачайте картинки:

```
python fetch_spacex.py
``` 

и/или 

```
python fetch_nasa.py
```

Автоматически создастся папка `images`, куда будут скачены картинки.

Далее запустите программу для публикации картинок:

```
python main.py
```


## Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](dvmn.org)
