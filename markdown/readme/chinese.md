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
