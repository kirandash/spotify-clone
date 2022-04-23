# Spotify Clone

## 1. Code Setup
- Resources: https://github.com/Hendrixer/fullstack-music
### 1.1 Setup
- Tech: Node.js, React.js, Postgres, Prisma, Next.js, Vercel (hosting), Heroku (for DB), and various component libraries.
- Notes: https://tinted-gym-f99.notion.site/Fullstack-course-notes-Students-3202660c315b438aba6c1ae051963572
- `npx create-next-app client`
- `npm run dev`

### 1.2 Setup Next.js, ESLint & TypeScript

## 2 App Layout
### 2.1 Setup Chakra UI
- `import reset-css`: to reset css for different browsers
- Use chakra library
- While selecting a UI/Component library it's better if CSS can be scoped to JS file and not imported globally

### 2.2 Creating Player Layout
- A box in Chakra is equivalent to a div
- But it' better to use Box so that we can use Chakra's primitive option to style and not use inline style or stylesheet

### 2.4 Creating the Sidebar
- Icons library:
    - https://react-icons.github.io/react-icons/
### 2.5 Adding the Logo
- use `NextImage` to optimize the image component. Ex: removing unnecessary info from svg or jpeg ex: meta, geolocation etc
## 3 Navigation
- `LinkBox`, `LinkOverlay`

### 3.1 Create a List Nav with LinkBox

### 3.2 Create Playlist Menu

## 4 Data Modelling
### 4.1 Setup Prisma & PostgreSQL on Heroku
- Prisma:
    - https://www.prisma.io/
    - Node.js and TypeScript ORM.
    - Easy to use
    - `npx prisma init`
    - Creates a prisma folder in project
    - Install Prisma extension
    - In .env file, update DATABASE_URI with URI of database from heroku (pick anyone of the two db created)
- Postgres:
    - SQL Database
    - Setup heroku app
    - add Heroku postgres adon under Resources
    - add twice for two Database - one fore real and one for shadow (to fix permission issue on heroku)
    - The shadow DB is needed because: Prisma needs access to create DB on fly but heroku's one DB doesn't give access to prisma to do that. So the workaround is to ask prisma to use a shadow DB for credentials and other things and one main DB
- Prisma is independent of heroku. Any other DB also should be fine
