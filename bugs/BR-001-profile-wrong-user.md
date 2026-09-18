ID

BR-001

Summary

При передаче accessToken нового зарегистрированного пользователя GET/profile возвращает данные пользователя name=admin

Environment

1. ноутбук Lenovo
2. ОС: Windows 11
3. Postman Version 12.25.1 Architecture x64
4.  Local API server (127.0.0.1:8000)

Preconditions

Пользователь Nika зарегистрирован и успешно авторизован в системе. Получен действительный accessToken

Steps to Reproduce

1. Выбрать HTTP-метод GET
1. Вставить URL - http://127.0.0.1:8000/profile
1. Во вкладке Authorization выбрать Type →Bearer Token
1. Ввести в поле Token полученное при авторизации значение – admin-token
1. Нажать Send

Actual Result

1. Сервер возвращает код статус 200
1. В теле ответа содержатся данные пользователя name=admin

Expected Result

1. Сервер возвращает код статус 200
1. В теле ответа содержатся данные нового зарегистрированного и авторизованного пользователя name=Nika

Severity

Critical

Priority

High

Reproducibility

4 из 4

Attachments

Отсутствуют
