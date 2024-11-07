# Setup Cook Environment
git clone [cook repo]<br/>
git submodule init<br/>
git submodule update<br/>

under cook-backend directory<br/>
-> create .env file containing DATABASE_URL=postgresql://postgres:group18@localhost:5432/mydb?schema=public

under cook-frontend directory<br/>
-> create .env file containing API_URL=http://localhost:4000/graphql

### Start the cook-backend container
docker compose up 

### View Database
cd cook-backend  
npx prisma migrate dev
npx prisma studio

### View API testing page
http://localhost:4000/graphql

### View Frontend App
cd cook-frontend  
npm install  
npx expo start



