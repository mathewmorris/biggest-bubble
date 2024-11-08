# Biggest Bubble - Twitch Chat

## Tech Stack
- NestJS (API)
    - Prisma (ORM)
    - Passport (auth)
    - Websocket (Twitch Messages)
- NextJS (Frontend
    - Tailwind CSS
    - ThreeJS (bubble 3D rendering)

## Getting Started
### Development
#### API
`cd api && npm run start:dev`

#### Frontend
`cd frontend && npm run dev`

#### Database
`docker run --name biggest-bubble-db -e POSTGRES_PASSWORD=wingardiumleviosa -d -p 5432:5432 postgres`

Going to use Docker to containerize the application and database in the future.
- `docker compose up` (you can add `-d` to detach and run in the backround)
This will build and start the database, API, and frontend locally.

### Testing
This should be conducted locally, will be in CI/CD at some point

#### [API](https://docs.nestjs.com/fundamentals/testing)
`cd api && npm run test`

#### [Frontend](https://nextjs.org/docs/app/building-your-application/testing)

