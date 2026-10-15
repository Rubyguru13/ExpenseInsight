# ExpenseInsight

A full-stack personal expense tracker built with TypeScript, React, Express, and MongoDB.

## Features and stack

- User registration/login with JWT authentication.
- Expense creation, editing, and deletion.
- User profile and profile-picture upload.
- Currency selection and dark mode.
- React, Redux, Vite, Tailwind CSS/DaisyUI, Express, Mongoose, and TypeScript.

## Local setup

Install Node.js/npm and make a MongoDB database available.

```powershell
git clone https://github.com/Rubyguru13/ExpenseInsight.git
cd ExpenseInsight
Copy-Item .env.example .env
```

Set `MONGO_URI` to your local MongoDB URI and `JWT_SECRET` to a long random secret in `.env`. The code uses `MONGO_URI`, not `MONGODB_URI`.

```powershell
npm ci
npm ci --prefix frontend
npm run dev
```

Frontend: http://localhost:5173. Backend: http://localhost:8000.

## Project structure

- `backend/`: API, controllers, models, authentication middleware, and database configuration.
- `frontend/`: React UI, Redux state, pages, and styles.
- `shared/`: shared TypeScript types and constants.
- `.env.example`: configuration template; do not commit your populated `.env`.

## Import changes

Removed promotional screenshots and replaced the root README with focused setup instructions. Application code is unchanged.

## Ideas for your own extension

Add monthly budgets, recurring expenses, CSV export, charts, and API tests. These are suggestions, not features claimed by this import.

## Source and license

Based on [maciekt07/ExpenseTracker](https://github.com/maciekt07/ExpenseTracker), revision `1023bc22a313dbb5904ad7b7c6e86bedfd02b36c`. Original authorship and copyright notices are retained in `LICENSE` and source files. This is an imported learning/portfolio starting point; original application authorship is not claimed.

## Validation

Files, configuration manifests, and Python syntax were checked during packaging. Dependencies were not installed and the applications were not run end to end.
