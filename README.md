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

```