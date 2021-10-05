<h1 align="center" style="border-bottom: none">
    <b>
        <a href="https://www.nocodb.com">NocoDB </a><br>
    </b>
    ✨ 开源 Airtable 替代品 ✨ <br>

</h1>
<p align="center">
将任何MySQL，PostgreSQL，SQL Server，SQLite＆MariaDB转换为智能电子表格。
</p>
<div align="center">

[![Build Status](https://travis-ci.org/dwyl/esta.svg?branch=master)](https://travis-ci.com/github/NocoDB/NocoDB)
[![Node version](https://badgen.net/npm/node/next)](http://nodejs.org/download/)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/NocoDB.svg?style=social&label=Follow%20%40NocoDB)](https://twitter.com/NocoDB)

</div>





<p align="center">
    <a href="http://www.nocodb.com"><b>Website</b></a> •
    <a href="https://discord.gg/5RgZmkW"><b>Discord</b></a> • 
    <a href="https://twitter.com/nocodb"><b>Twitter</b></a>
</p>  

![OpenSourceAirtableAlternative](https://user-images.githubusercontent.com/5435402/133762127-e94da292-a1c3-4458-b09a-02cd5b57be53.png)


<img src="https://static.scarf.sh/a.png?x-pxid=c12a77cc-855e-4602-8a0f-614b2d0da56a" />

<a href="https://www.producthunt.com/posts/nocodb?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-nocodb" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=297536&theme=dark" alt="NocoDB - The Open Source Airtable alternative | Product Hunt" style="width: 250px; height: 54px;" width="250" height="54" /></a>


# 快速尝试
### 一键式部署

#### Heroku
<a href="https://heroku.com/deploy?template=https://github.com/npgia/nocodb-seed-heroku">
    <img 
    src="https://www.herokucdn.com/deploy/button.svg" 
    width="300px"
    alt="Deploy NocoDB to Heroku with 1-Click" 
    />
</a>
<br>

### 使用Docker
```bash
docker run -d --name nocodb -p 8080:8080 nocodb/nocodb:latest
```

> 为了持久化数据，你可以挂载`/usr/app/data/`。

### 使用NPM
```
npx create-nocodb-app
```
### 使用git
```
git clone https://github.com/nocodb/nocodb-seed
cd nocodb-seed
npm install
npm start
```

### GUI

使用仪表板使用 : [http://localhost:8080/dashboard](http://localhost:8080/dashboard)


# 加入我们的社区
<a href="https://discord.gg/5RgZmkW">
<img src="https://discordapp.com/api/guilds/661905455894888490/widget.png?style=banner3" alt="">
</a>
<br>
<br>

# 截图

![1](https://user-images.githubusercontent.com/86527202/136064527-86ef8e8c-0f54-4779-aa05-c187ba1faa3e.png)
<br>

![2](https://user-images.githubusercontent.com/86527202/136064539-2a6cc35f-7c0b-47bc-8b15-22dc51768c55.png)
<br>

![5](https://user-images.githubusercontent.com/86527202/136064547-a6c9255b-f7e0-4b77-a37d-320e8ed92481.png)
<br>

![6](https://user-images.githubusercontent.com/86527202/136064551-58edf778-7e50-49ed-b64a-57d87d3a767e.png)
<br>

![7](https://user-images.githubusercontent.com/86527202/136064557-1d38e2fd-708d-4898-82f1-0abe961178fe.png)
<br>

![8](https://user-images.githubusercontent.com/86527202/136064560-4ecf7b08-8d22-483d-9067-1f78993440cd.png)
<br>

![9](https://user-images.githubusercontent.com/86527202/136064561-298da35a-eee6-4f89-b219-e187d1b550a0.png)
<br>

![9a](https://user-images.githubusercontent.com/86527202/136064563-5eb52802-1708-48be-ad6f-5b315246946f.png)
<br>

![9b](https://user-images.githubusercontent.com/86527202/136064568-5ce388b8-b1ff-4243-8d60-0e67ce680d37.png)
<br>

![10](https://user-images.githubusercontent.com/86527202/136064571-2b2b4c03-575b-4038-bb33-457b79437791.png)
<br>

![11](https://user-images.githubusercontent.com/86527202/136064574-dc88669e-c893-4379-8e4a-38a8016db89e.png)
<br>






# 特征
### 丰富的电子表格接口

- ⚡ 搜索，排序，过滤，隐藏uber轻松的列
- ⚡ 创建视图：网格，画廊，卡班，甘特，形式
- ⚡ 分享视图：公共和密码保护
- ⚡ 个人和锁定视图
- ⚡ 将图像上传到单元格（使用S3，Minio，GCP，Azure，Dimitedocean，Linode，OVH，Backblaze）!!
- ⚡ 角色：所有者，创建者，编辑器，评论者，查看器，评论者，自定义角色。
- ⚡ 访问控制：即使在数据库，表和列级别也是细粒度的访问控制。

### 工作流自动化应用商店：
- ⚡ 聊天：微软团队，松弛，不和谐，最重要的
- ⚡ 电子邮件：SMTP，SES，MailChimp
- ⚡ 短信：Twilio
- ⚡ whatsapp
- ⚡ 任何第三方API

### Programmatic API访问通过：
- ⚡ 休息apis（播开）
- ⚡ GraphQLAPI。
- ⚡ 包括JWT身份验证和社交验证
- ⚡ 与Zapier，Integromat集成的API标记。


# 生产安装
NoCodb要求数据库存储电子表格视图和外部数据库的元数据。可以在NC_DB环境变量中指定此数据库的连接参数。

## Docker

#### MySQL 示例
```bash
docker run -d -p 8080:8080 \
    -e NC_DB="mysql2://host.docker.internal:3306?u=root&p=password&d=d1" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

#### Postgres 示例
```bash
docker run -d -p 8080:8080 \
    -e NC_DB="pg://host:port?u=user&p=password&d=database" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

#### SQL Server 示例
```bash
docker run -d -p 8080:8080 \
    -e NC_DB="mssql://host:port?u=user&p=password&d=database" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

## Docker Compose
```bash
git clone https://github.com/nocodb/nocodb
cd docker-compose
cd mysql or pg or mssql
docker-compose up
```


## 环境变量
| 变量                | 强制 | 注释                                                                         | 如果缺少                                  |
|-------------------------|-----------|----------------------------------------------------------------------------------|--------------------------------------------|
| NC_DB                   | Yes       | 查看我们的数据库 URL                                                | 将在根文件夹中创建本地 SQLite  |
| DATABASE_URL            | No        | JDBC URL 格式。 可以代替 NC_DB 使用。 用于一键式 Heroku 部署|   |
| DATABASE_URL_FILE       | No        | 包含 JDBC URL 格式的文件的路径。 可以代替 NC_DB 使用。 用于一键式 Heroku 部署|   |
| NC_PUBLIC_URL           | Yes       | 用于发送电子邮件邀请                   | 从 http 请求参数的最佳猜测        |
| NC_AUTH_JWT_SECRET      | Yes       | 用于认证和存储其他 secret 的 JWT secret                           | 将会产生一个随机的 secret          |
| NC_SENTRY_DSN           | No        | 用于 Sentry 监控                                                     |   |
| NC_CONNECT_TO_EXTERNAL_DB_DISABLED | No | 禁止使用外部数据库创建项目                              |   |
| NC_DISABLE_TELE | No | 禁用 telemetry                              |   |
| NC_BACKEND_URL | No | 自定义后端URL                              | 将使用`http://localhost:8080`  |

# 开发安装

```bash
git clone https://github.com/nocodb/nocodb
cd nocodb

# 运行后端
cd packages/nocodb
npm install
npm run watch:run

# 在浏览器打开 localhost:8080/dashboard

# 运行前端
cd packages/nc-gui
npm install
npm run dev

# 在浏览器打开 localhost:3000/dashboard
```

对代码所做的更改会自动重新启动。

## 在本地运行 Cypress 测试

```bash
# 安装开发依赖(cypress)
npm install

# 使用 docker compose 运行所需的服务
docker-compose -f ./docker-compose-cypress.yml up

# 等到 3000 和 8080 端口都可用时，使用以下命令运行Cypress测试
npm run cypress:run

# 或运行以下命令在图形用户界面上运行它
npm run cypress:open
```

# 贡献

- 请看一下 ./contribute/HowToApplyLicense.md
- 忽略为 .json 或 .md 或 .yml 添加标头

# 🎯  为什么我们建立这个？

大多数互联网业务都配备了电子表格或数据库以解决其业务需求。电子表格每天都会合作地使用十亿+人类。但是，我们在数据库上运行类似速度的方式，这在计算时更强大的工具。用SaaS产品解决此问题的尝试已经意味着可怕的门禁控制，供应商锁定，数据锁定，突然的价格变化，最重要的是将来有可能的玻璃天花板。

# ❤ 我们的任务 ：

我们的使命是为数据库提供最强大的无码界面，该界面是世界上每一个互联网业务的开源。这不仅将民主化进入强大的计算工具，而且还带来了一十亿+人，他们将在互联网上具有根本修补和建筑能力。
