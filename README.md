# Spotify Clone

## 1. Code Setup
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
