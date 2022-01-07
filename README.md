## Авторизация 
# Написать REST API на базе ExpressJs для регистрации/логина на базе JWT токенов. 
- `sign_up` &mdash; регистрирует пользователя 
- `login` &mdash; логинит и выдает токен доступа с TTL (time to live) от 30 до 60 секунд(рандомно)
- `refresh` &mdash; перевыпускает новый токен доступа 
- `me[0-9]` &mdash; отдает mock данные пользователя и отдельным полем
номер запроса если токен заэкспайрился(вышло время его TTL) отвечаем 401 Unauthorised.
Для хранения данных пользователя используем MongoDB, голый драйвер без Mongoose
