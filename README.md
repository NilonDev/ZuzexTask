# ZuzexTask

Реализовать небольшое CRUD-приложение:

Java модели:
1. Пользователи(Идентификатор, имя, возраст, пароль)
2. Дома(Идентификатор, адрес, идентификатор хозяина)

Структура базы данных должна быть основана на Java моделях, но без ограничений
Структура базы данных должна быть создана при старте приложения миграциями(использовать Liquibase)

Приложение должно предоставлять возможности:
1. Получать, создавать, обновлять, удалять пользователей и дома
2. Добавлять пользователей в дома:
   1. В доме может быть несколько жильцов
   2. В доме должен быть 1 хозяин
   3. Только хозяин может добавлять жильцов к себе в дом
3. Получение JWT-токена(только access, не усложняйте)
4. Все операции, кроме создания пользователя должны быть с проверкой токена

Технологии:
PostgreSQL, Spring Boot(REST, JPA), Liquibase, Maven, Java(11 версии и выше)
