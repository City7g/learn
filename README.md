# learn

psql -U пользователь -d база - подключение к базе

\du - список ползователей
\dt - список таблиц
\dp - список привелегий
\d "таблица" - увидеть всю инфу про таблицу
\c - кто и где я
\c "база" - перейти в другую базу
\z "таблица" - кто и какие права имеет
\q - выйти

CREATE DATABASE mydatabase - создать таблицу


Действия с пользователем
CREATE ROLE "юзер";
CREATE ROLE "юзер" WITH "права";
ALTER ROLE имя_пользователя WITH CREATEDB;
DROP ROLE "юзер";
GRANT ALL ON TABLE "таблица" TO "юзер";
REVOKE ALL ON TABLE "таблица" FROM "юзер";


Права:
SUPERUSER - понятно
CREATEDB - создавать и удалять базы
CREATEROLE - создавать и удалять роли
PASSWORD - задать пароль
VALID UNTIL - работает до...
