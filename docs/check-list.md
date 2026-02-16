# API Testing Checklist - JSONPlaceholder

## /posts endpoint (CRUD operations)

- [x] GET /posts - возвращается список всех постов, статус 200
- [x] GET /posts/1/ возвращает пост с id=1, присутствуют поля userId/id/title/body, статус 200
- [x] GET /posts?userId=1 фильтрация работает, возвращает все посты с userId=1, статус 200
- [x] POST /posts создание работает, title/body/userId совпадают с отправленными, присвоился новый номер id=101, корректный статус 201
- [x] PUT /posts/1 полное обновление работает, значения title/body/userId изменились на отправленные, статус 200
- [x] PATCH /posts/1 частичное обновление работает, значение title изменено, статус 200
- [x] DELETE /posts/1 удаление отрабатывает корректно

## /comments endpoint (query and nested route)
- [x] GET /comments?postId=1 фильтация по postId работает, возвращает комментарии поста 1
- [x] GET /posts/1/comments nested route работает, также возвращает комментарии поста 1

## Negative scenario
- [x] /postss неверный эндпоинт возвращает ошибку (статус 404)
