# API_YATUBE
API для социальной сети блогеров
## Основные функции:
- Публикация личных дневников;
- Подписка на других авторов и комментирование их записей;
- Поиск новых друзей по интересам.

## Для запуска Вам понадобиться:
- Клонировать репозиторий
```
git clone git@github.com:Pe4enka5/api_final_yatube.git
``` 
- Перейти в папку 
```
cd <ваш путь>/api_final_yatube
``` 
- установить и активировать виртуальное окружение;
```
python3 -m venv venv
source venv/bin/activate
``` 
- установить зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 
- Выполнить миграции
```
python manage.py migrate
```
- Запустить проект
```
python manage.py runserver
```
- заварите чай/кофе, возмите  что-нибудь перекусить и поехали!
## Некоторые примеры запросов к API.
- При запросе @Get к http://127.0.0.1:8000/api/v1/posts/{id}/ получаем:
```
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
```
- При запросе @Post к http://127.0.0.1:8000/api/v1/posts/ получаем:
```
{
  "text": "string",
  "image": "string",
  "group": 0
}
```
```
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
```
- Более подробная документация находится по адресу: http://127.0.0.1:8000/redoc/

### Автор: 
[Андрей Pe4enka Печерица](https://github.com/Pe4enka5)
Всем добра и печенек!
