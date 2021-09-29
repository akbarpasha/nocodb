<h1 align="center" style="border-bottom: none">
    <b>
        <a href="https://www.nocodb.com">NocoDB </a><br>
    </b>
    ✨ L'alternative Open Source Airtable ✨ <br>

</h1>
<p align="center">
Tournez n'importe quel MySQL, PostgreSQL, SQL Server, SQLite & Mariadb dans une feuille de calcul intelligente. 
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


# Essayer rapidement
### 1-Click Deploy

#### Heroku
<a href="https://heroku.com/deploy?template=https://github.com/npgia/nocodb-seed-heroku">
    <img 
    src="https://www.herokucdn.com/deploy/button.svg" 
    width="300px"
    alt="Deploy NocoDB to Heroku with 1-Click" 
    />
</a>
<br>

### Utiliser Docker
```bash
docker run -d --name nocodb -p 8080:8080 nocodb/nocodb:latest
```

> To persist data you can mount volume at `/usr/app/data/`.

### En utilisant npm
```
npx create-nocodb-app
```
### En utilisant git
```
git clone https://github.com/nocodb/nocodb-seed
cd nocodb-seed
npm install
npm start
```

### GUI

Accès au tableau de bord en utilisant : [http://localhost:8080/dashboard](http://localhost:8080/dashboard)


# Rejoignez notre communauté
<a href="https://discord.gg/5RgZmkW">
    <img 
    src="https://invidget.switchblade.xyz/5RgZmkW" 
    alt="Join NocoDB : Free & Open Source Airtable Alternative"
    >
</a>
<br>

# Captures d'écran

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



# Caractéristiques
### Interface de feuille de calcul riche

- ⚡ Recherche, trier, filtrer, masquer les colonnes avec Uber Facile
- ⚡ Créer des vues: grille, galerie, kanban, gantt, forme
- ⚡ Partager des vues: Public & Mot de passe protégé
- ⚡ Vues personnelles et verrouillées 
- ⚡ Télécharger des images sur les cellules (fonctionne avec S3, Minio, GCP, Azure, DigitalOcean, Linode, Ovh, Backblaze) !!
- ⚡ Rôles: propriétaire, créateur, éditeur, commentateur, spectateur, commentateur, rôles personnalisés.
- ⚡ Contrôle d'accès: contrôle d'accès à grain fin, même à la base de données, au niveau de la table et de la colonne.

### App Store for Workflow Automation:
- ⚡ Chat: équipes de Microsoft, relais, discorde, la plus grande
- ⚡ Email: SMTP, SES, MailChimp
- ⚡ SMS: Twilio
- ⚡ WhatsApp
- ⚡ Toute API tierce

### Accès d'API programmatique via:
- ⚡ Apis de repos (Swagger)
- ⚡ API GraphQL.
- ⚡ inclut l'authentification JWT et l'authentification sociale
- ⚡ Jetons API à intégrer avec Zapier, Integromat.


# Configuration de la production 
NocoDB nécessite une base de données pour stocker les métadonnées des vues des feuilles de calcul et des bases de données externes. Et les paramètres de connexion pour cette base de données peuvent être spécifiés dans la variable d'environnement `NC_DB`. 

## Docker 

#### Exemple MySQL
```
docker run -d -p 8080:8080 \
    -e NC_DB="mysql2://host.docker.internal:3306?u=root&p=password&d=d1" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

#### Exemple Postgres
```
docker run -d -p 8080:8080 \
    -e NC_DB="pg://host:port?u=user&p=password&d=database" \
    -e NC_AUTH_JWT_SECRET="569a1821-0a93-45e8-87ab-eb857f20a010" \
    nocodb/nocodb:latest
```

#### Exemple SQL Server
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


## Variables d'environnement
| Variable                | Mandatory | Comments                                                                         | If absent                                  |
|-------------------------|-----------|----------------------------------------------------------------------------------|--------------------------------------------|
| NC_DB                   | Yes       | See our database URLs                                                            | A local SQLite will be created in root folder  |
| DATABASE_URL            | No        | JDBC URL Format. Can be used instead of NC_DB. Used in 1-Click Heroku deployment|   |
| DATABASE_URL_FILE       | No        | path to file containing JDBC URL Format. Can be used instead of NC_DB. Used in 1-Click Heroku deployment|   |
| NC_PUBLIC_URL           | Yes       | Used for sending Email invitations                   | Best guess from http request params        |
| NC_AUTH_JWT_SECRET      | Yes       | JWT secret used for auth and storing other secrets                               | A Random secret will be generated          |
| NC_SENTRY_DSN           | No        | For Sentry monitoring                                                     |   |
| NC_CONNECT_TO_EXTERNAL_DB_DISABLED | No | Disable Project creation with external database                              |   |
| NC_DISABLE_TELE | No | Disable telemetry                              |   |
| NC_BACKEND_URL | No | Custom Backend URL                              | ``http://localhost:8080`` will be used  |

# Paramétrage du développement
```
git clone https://github.com/nocodb/nocodb
cd nocodb

# run backend
cd packages/nocodb
npm install
npm run watch:run

# open localhost:8080/dashboard in browser

# run frontend 
cd packages/nc-gui
npm install
npm run dev

# open localhost:3000/dashboard in browser
```

Changes made to code automatically restart.


## Exécuter des tests Cypress localement

```shell
# install dependencies(cypress)
npm install

# run required services by using docker compose 
docker-compose -f ./docker-compose-cypress.yml up



# wait until both 3000 and 8080 porta are avalable
# and run cypress test using following command
npm run cypress:run

# or run following command to run it with GUI
npm run cypress:open
```

# Contribuant
- S'il vous plaît jeter un oeil à ./contribute/HowToApplyLicense.md 
- Ignorer l'ajout d'en-têtes pour .json or .md or .yml   

# 🎯  Pourquoi construisons-nous cela ?
La plupart des entreprises Internet s'équipent d'un tableur ou d'une base de données pour répondre à leurs besoins commerciaux. Les feuilles de calcul sont utilisées par plus d'un milliard d'humains en collaboration chaque jour. Cependant, nous sommes loin de travailler à des vitesses similaires sur des bases de données qui sont des outils beaucoup plus puissants en matière de calcul. Les tentatives pour résoudre ce problème avec les offres SaaS ont entraîné des contrôles d'accès horribles, le verrouillage des fournisseurs, le verrouillage des données, des changements de prix brusques et, surtout, un plafond de verre sur ce qui est possible à l'avenir.

# ❤ Notre mission :  
Notre mission est de fournir l'interface sans code la plus puissante pour les bases de données qui soit open source pour chaque entreprise Internet dans le monde. Cela démocratiserait non seulement l'accès à un outil informatique puissant, mais ferait également émerger plus d'un milliard de personnes qui auront des capacités radicales de bricolage et de construction sur Internet. 

