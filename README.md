# Тестовое задание

### Интеграция с BotAPI VK
Создан бот, который цитирует присланный ему текст

### Запуск
1. Для начала необходимо создать Сообщество, от имени которого бот будет общаться. (https://vk.com/dev/bots_docs)
2. В файле src\main\resources\application.properties указать свои код подтверждения и ключ доступа
3. Так как Callback API будет посылать запрос на события взаимодействия с ботом, необходимо "выложить" наш сервер в интернет. Можно арендовать сервер, а можно воспользоваться ngrok.
Для этого нужно скачать ngrok, зарегистрироваться на сайте и получить токен. Настройку ngroka можно почитать на офиц. сайте.
После настройки ngrok (или деплое приложения на сервере), нужно этот адрес сервера указать в настройках ВК Callback API. На этот адрес и будут отправляться запросы с ВК на события с ботом.
4. Запустить файл Application.kt
<br>


#### Настройки бота
Типы событий - только входящие сообщения. Версия api - 5.236