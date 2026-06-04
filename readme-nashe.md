Как запустить локально в режиме разработчика

1. контейнер docker compose up -d db (перед этим создать файл env и заполнить ) 
DATABASE_URL=postgresql://postgres:test@127.0.0.1:5432/brain_test  (пример)

2. 
cd backend
npm install
npx prisma generate
npx prisma migrate deploy

3. 
cd ../frontend
npm install

4. 
cd backend
npm run dev

cd frontend
npm start

должно работать =) 