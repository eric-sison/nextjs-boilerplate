# 🚀 Next.js + Hono.js Full-Stack Boilerplate

A modern full-stack boilerplate built with **Next.js** (frontend) and **Hono.js** (backend), designed for speed, developer experience, and scalability.  
It comes pre-configured with database, testing, UI components, and deployment-ready Docker support.

---

## ✨ Features

- **Backend**: [Hono.js](https://hono.dev) – Fast, lightweight web framework for building APIs.
- **Frontend**: [Next.js](https://nextjs.org) – React framework for building modern web applications.
- **Database**: [Drizzle ORM](https://orm.drizzle.team/) with **PostgreSQL** – Type-safe queries & migrations.
- **UI**: [shadcn/ui](https://ui.shadcn.com) – Beautiful, accessible components built with Radix UI & Tailwind.
- **Data Fetching**: [TanStack React Query](https://tanstack.com/query/latest) – Async state management for React.
- **Testing**:
  - [Vitest](https://vitest.dev) – Unit testing framework.
  - [Playwright](https://playwright.dev) – End-to-end (E2E) testing.
- **Deployment**: Pre-configured `Dockerfile` for containerized builds.

---

## 📦 Tech Stack

| Layer      | Library/Framework               |
| ---------- | ------------------------------- |
| Frontend   | Next.js, shadcn/ui, React Query |
| Backend    | Hono.js                         |
| Database   | PostgreSQL + Drizzle ORM        |
| Testing    | Vitest (unit), Playwright (e2e) |
| Deployment | Docker                          |

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/eric-sison/nextjs-boilerplate.git
cd nextjs-boilerplate
```

### 2. Install Dependencies

```bash
pnpm install
```

### 3. Set up Environment Variables

```env
NEXT_PUBLIC_HOST=
DB_HOST=
DB_PORT=
DB_USER=
DB_PASS=
DB_NAME=
```

### 4. Start Development Server

```bash
pnpm dev
```

## 🧪 Testing

- Unit Test (Vitest):

```bash
pnpm test
```

- End-to-end Test (Playwright):

```bash
# non-interactive mode
pnpm test:e2e

# interactive mode
pnpm test:e2e-ui
```

## 🐳 Docker

Build and run the app in a container:

```bash
docker build -t nextjs-hono-app .
docker run -p 3000:3000 nextjs-hono-app
```

## 🚧 Roadmap / Future Ideas

- Authentication & authorization (better-auth integration)

- Monitoring & logging integrations

- Example deployment configs (Fly.io, Railway, Vercel)
