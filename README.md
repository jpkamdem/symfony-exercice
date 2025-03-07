Veuillez créer un .env à la racine du projet et y coller les propriétés suivantes :

```env
APP_ENV=dev
APP_SECRET=1fb4b932035f545d680f9f5db7779d06
HOST=localhost
DB_HOST=127.0.0.1

DB_PORT=5432
DB_PASSWORD=root
DB_USER=root
DB_DATABASE=app
DATABASE_URL=postgresql://${DB_USER}:${DB_PASSWORD}@${DB_HOST}:${DB_PORT}/${DB_DATABASE}?schema=public

PGADMIN_DEFAULT_EMAIL=johndoe@gmail.com
PGADMIN_DEFAULT_PASSWORD=johndoe

```

Voici le lien GET :
```bash
http://127.0.0.1:8000/task/datas
```

### Comment lancer le projet
- git clone https://github.com/jpkamdem/symfony-exercice.git
- cd symfony-exercice
- composer install
- créez le .env
- docker compose up -d
- php bin/console doctrine:migrations:migrate
- symfony serve
```bash
http://127.0.0.1:8000/task
```