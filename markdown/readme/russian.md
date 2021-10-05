<h1 align="center" style="border-bottom: none">
    <b>
        <a href="https://www.nocodb.com">NocoDB </a><br>
    </b>
    ✨ Альтернатива Airtable с открытым исходным кодом ✨ <br>

</h1>
<p align="center">
Превращает любой MySQL, PostgreSQL, SQL Server, SQLite & Mariadb в смарт-таблицу. 
</p>
<div align="center">

[![Build Status](https://travis-ci.org/dwyl/esta.svg?branch=master)](https://travis-ci.com/github/NocoDB/NocoDB)
[![Node version](https://badgen.net/npm/node/next)](http://nodejs.org/download/)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/NocoDB.svg?style=social&label=Follow%20%40NocoDB)](https://twitter.com/NocoDB)

</div>





<p align="center">
    <a href="http://www.nocodb.com"><b>Вебсайт</b></a> •
    <a href="https://discord.gg/5RgZmkW"><b>Discord</b></a> • 
    <a href="https://twitter.com/nocodb"><b>Twitter</b></a>
</p>  

![OpenSourceAirtableAlternative](https://user-images.githubusercontent.com/5435402/133762127-e94da292-a1c3-4458-b09a-02cd5b57be53.png)


<img src="https://static.scarf.sh/a.png?x-pxid=c12a77cc-855e-4602-8a0f-614b2d0da56a" />

<a href="https://www.producthunt.com/posts/nocodb?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-nocodb" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=297536&theme=dark" alt="NocoDB - The Open Source Airtable alternative | Product Hunt" style="width: 250px; height: 54px;" width="250" height="54" /></a>


# Быстрый старт
### 1-Нажмите на Deploy

#### Heroku
<a href="https://heroku.com/deploy?template=https://github.com/npgia/nocodb-seed-heroku">
    <img 
    src="https://www.herokucdn.com/deploy/button.svg" 
    width="300px"
    alt="Deploy NocoDB to Heroku with 1-Click" 
    />
</a>
<br>

### Используя Docker
```bash
docker run -d --name nocodb -p 8080:8080 nocodb/nocodb:latest
```

> Для сохранения данных, вы можете установить том в `/usr/app/data/`.

### Используя NPM
```
npx create-nocodb-app
```
### Используя git.
```
git clone https://github.com/nocodb/nocodb-seed
cd nocodb-seed
npm install
npm start
```

### GUI

Получите доступ к панели управления, используя : [http://localhost:8080/dashboard](http://localhost:8080/dashboard)


# Присоединяйтесь к нашему сообществу
<a href="https://discord.gg/5RgZmkW">
    <img 
    src="https://discordapp.com/api/guilds/661905455894888490/widget.png?style=banner3" 
    alt="Join NocoDB : Free & Open Source Airtable Alternative"
    >
</a>
<br>

# Скриншоты

![2](https://user-images.githubusercontent.com/5435402/133759229-4275b934-873b-4a9b-9f23-96470fec9775.png)
<br>

![1](https://user-images.githubusercontent.com/5435402/133759218-f8b0bffc-707f-451c-82f2-b5ba2573d6a6.png)
<br>

![7](https://user-images.githubusercontent.com/5435402/133759245-a536165b-55f1-46a8-a74e-1964e7e481c6.png)
<br>

![5](https://user-images.githubusercontent.com/5435402/133759240-dd3f2509-aab7-4bd1-9a58-4c2dff08f2f2.png)
<br>

![6](https://user-images.githubusercontent.com/5435402/133759242-2311a127-17c8-406c-b865-1a2e9c8ee398.png)
<br>

![3](https://user-images.githubusercontent.com/5435402/133759234-9b539029-be36-4a35-b55a-bee3ebd0e010.png)
<br>

![4](https://user-images.githubusercontent.com/5435402/133759236-dc182129-3768-4e23-874e-98f5f32e962c.png)
<br>

![11](https://user-images.githubusercontent.com/5435402/133759253-bb9bc729-ee28-4f86-ab95-7d112c0815f2.png)
<br>

![10](https://user-images.githubusercontent.com/5435402/133759250-ebd75ecf-31db-4a17-b2d7-2c43af78a54e.png)
<br>

![8](https://user-images.githubusercontent.com/5435402/133759248-3a7141e0-4b7d-4079-a5f9-cf8611d00bc5.png)
<br>

![9](https://user-images.githubusercontent.com/5435402/133759249-8c1a85c2-a55c-48f6-bd58-aa6b4195cce7.png)









# Функции
### Богатый интерфейс электронной таблицы

- ⚡ Поиск, сортировка, фильтр, скрыть столбцы с невероятной легкостью
- ⚡ Создание видов: сетка, галерея, канбан, Гантт, форма
- ⚡ Делиться видами: публичный & защищенный паролем
- ⚡ Личные и заблокированные виды
- ⚡ Загрузить изображения в ячейки (работает с S3, Minio, GCP, Azure, Digitalocean, Linode, Ovh, BackBlaze)
- ⚡ Роли: владелец, создатель, редактор, зритель, комментатор, пользовательские роли.
- ⚡ Контроль доступа: тонкозернистый контроль доступа даже в базе данных, уровень таблицы и столбца.

### App Store для автоматики рабочего процесса:
- ⚡ Чат: Microsoft Teams, Slack, Discord, Mattermost
- ⚡ Электронная почта: SMTP, SES, MailChimp
- ⚡ SMS: Twilio
- ⚡ WhatsApp
- ⚡ Любая API третьей стороны

### Программный доступ API через:
- ⚡ REST API (Swagger)
- ⚡ GraphQL API
- ⚡ Включает в себя JWT Authentication & Social Auth
- ⚡ токены API для интеграции с Zapier, Integomat.


# Настройка производства
NocoDB требует базу данных для хранения метаданных видов электронных таблиц и внешних баз данных. Подключения параметров для этой базы данных можно указать в переменной среды NC_DB.

## Docker

#### Пример MySQL
```
docker run -d -p 8080:8080 \
    -e NC_DB="mysql2://host.docker.internal:3306?u=root&p=password&d=d1" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

#### Пример Postgres
```
docker run -d -p 8080:8080 \
    -e NC_DB="pg://host:port?u=user&p=password&d=database" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

#### Пример SQL Server
```
docker run -d -p 8080:8080 \
    -e NC_DB="mssql://host:port?u=user&p=password&d=database" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

## Docker Compose
```
git clone https://github.com/nocodb/nocodb
cd docker-compose
cd mysql or pg or mssql
docker-compose up
```


## Переменные среды
| Переменная                | Обязательна | Комментарии                                                                         | Если отсутствует                                  |
|-------------------------|-----------|----------------------------------------------------------------------------------|--------------------------------------------|
| NC_DB                   | Да       | Посмотрите наши URL-адреса базы данных                                                            | В корневой папке будет создан локальный SQLite  |
| DATABASE_URL            | Нет        | Формат URL JDBC. Может использоваться вместо NC_DB. Используется при развертывании Heroku в один клик|   |
| DATABASE_URL_FILE       | Нет        | путь к файлу, содержащему формат URL JDBC. Может использоваться вместо NC_DB. Используется при развертывании Heroku в один клик|   |
| NC_PUBLIC_URL           | Да       | Используется для отправки email приглашений                   | Лучшее предположение из параметров HTTP-запроса        |
| NC_AUTH_JWT_SECRET      | Да       | Секрет JWT, используемый для аутентификации и хранения других секретов                               | Будет сгенерирован случайный секрет          |
| NC_SENTRY_DSN           | Нет        | Для сторожевого мониторинга                                                     |   |
| NC_CONNECT_TO_EXTERNAL_DB_DISABLED | Нет | Отключить создание проекта с внешней базой данных                              |   |
| NC_DISABLE_TELE | Нет | Отключить телеметрию                              |   |
| NC_BACKEND_URL | Нет | Пользовательский Backend URL                              | будет использоваться ``http://localhost:8080`` |

# Настройка разработки
```
git clone https://github.com/nocodb/nocodb
cd nocodb

# запустить бэкэнд
cd packages/nocodb
npm install
npm run watch:run

# открыть localhost:8080/dashboard в браузере

# запустить фронтэнд 
cd packages/nc-gui
npm install
npm run dev

# открыть localhost:3000/dashboard в браузере
```

Изменения, внесенные в код, автоматически перезапускаются.


## Локальный запуск Cypress-тестов

```shell
# установить зависимости (cypress)
npm install

# запустить необходимые службы с помощью docker compose 
docker-compose -f ./docker-compose-cypress.yml up



# подождите, пока станут доступны порты 3000 и 8080
# и запустите тест cypress, используя следующую команду
npm run cypress:run

# или запустите следующую команду, чтобы запустить ее с графическим интерфейсом
npm run cypress:open
```

# Содействие
- Пожалуйста, посмотрите ./contribute/HowToApplyLicense.md
- Игнорировать добавление заголовков для .json, .md или .yml.

# 🎯  Почему мы строим это?
Большинство интернет-компаний используют электронные таблицы или базы данных для решения своих бизнес-задач. Таблицы ежедневно используют более миллиарда человек. Однако мы далеко не работаем с аналогичной скоростью над базами данных, которые являются более мощными инструментами, когда дело доходит до вычислений. Попытки решить эту проблему с помощью предложений SaaS означали ужасный контроль доступа, блокировку поставщиков, блокировку данных, резкие изменения цен и, самое главное, стеклянный потолок для того, что возможно в будущем.

# ❤ Наша миссия :
Наша миссия - предоставить самый мощный интерфейс без кода для баз данных с открытым исходным кодом для каждого интернет-бизнеса в мире. Это не только демократизирует доступ к мощному вычислительному инструменту, но и приведет к появлению более миллиарда человек, которые будут иметь радикальные способности возиться и строить в Интернете.