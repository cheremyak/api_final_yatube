Описание: API для социальной сети Yatube

Примеры обрабатывемых запросов:

POST-запрос по адресу: http://127.0.0.1:8000/api/v1/posts/
Содержние:
{
  "text": "string",
  "image": "string",
  "group": 0
}
Ответ:
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}

GET-запрос по адресу: http://127.0.0.1:8000/api/v1/posts/
Пример ответа:
[
  {
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0
  }
]

Для просмотра других примеров запросов, после запуска сервера, перейдите по адресу:
http://127.0.0.1:8000/redoc


Установка:

Клонируйте репозиторий git@github.com:cheremyak/api_final_yatube.git

Создайте и активируйте виртуальное окружение:
python3 -m venv env source env/bin/activate

Установите зависимости из requirements.txt:
pip install -r requirements.txt 

Выполните миграции:
python3 manage.py migrate

Запустите сервер:
python3 manage.py runserver