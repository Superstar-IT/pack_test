# Pack Tech Test - Profile Screen

## How to use

1. Clone or download the repositories of backend and frontend
- [Backend Repository](https://github.com/Superstar-IT/pack_test_be.git)
- [Frontend Repository](https://github.com/Superstar-IT/pack_test_fe.git)

2. Run Backend server
```bash
git clone --depth 1 https://github.com/Superstar-IT/pack_test_be.git backend
cd backend/
cp env-example .env
```
Create new Postgres DB named `pack_test` in local

Change `DATABASE_HOST=postgres` to `DATABASE_HOST=localhost` <br />
Change `APP_PORT=3000` to `APP_PORT=5000` <br />
Change `BACKEND_DOMAIN=http://localhost:3000` to `BACKEND_DOMAIN=http://localhost:5000` <br />
Change `DATABASE_NAME=api` to `DATABASE_NAME=pack_test`

```bash
npm install

npm run migration:run

npm run seed:run

npm run start:dev
```

Swagger: http://localhost:5000/api/docs

3. Run Frontend
```bash
git clone --depth 1 https://github.com/Superstar-IT/pack_test_fe.git frontend
cd frontend/
cp .env.sample .env
```

Change `REACT_APP_URL_API = http://localhost:3030/api` to `REACT_APP_URL_API = http://localhost:5000/api/v1`

```bash
npm install

npm start
```

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

## Implementation
- Create Login Screen
- Create Profile Screen
- Login Info
```bash
email: john.doe@example.com
password: secret
```