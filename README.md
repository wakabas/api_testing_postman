# QA portfolio: testing open-source API jsonplaceholder.typicode.com (Postman)

## Что из себя представляет
Postman коллекция для тестирования REST API (JSONPlaceholder):

9 позитивных и 1 негативный сценарий, проверки статус кодов и структуры JSON.
Используются эндпоинты /posts и /comments

## Что внутри
- `postman/JSONPlaceholder testing.json` - коллекция запросов + тесты
- `postman/jsonplaceholder_enviroment.json` - окружение в котором добавлена переменная baseUrl с значением https://jsonplaceholder.typicode.com для того чтобы упростить обращение к эндпоинтам.
- `docs/check-list.md` - чек-листы API проверок
- `docs/test-cases` - примеры тест-кейсов (позитивный/негативный)

## Как запустить
1. Импорт коллекции запросов 
    Открыть Postman - Import - выбрать файл `JSONPlaceholder testing.json`
2. Импорт окружения
    Import - выбрать файл `jsonplaceholder_enviroment.json`
3. Выбор окружения в коллекции
    Перейти в коллекцию - выбрать окружение `jsonplaceholder`


