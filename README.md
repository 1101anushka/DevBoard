# DevBoard — Fundamentals (UI only)

The DevBoard front end, running **standalone** with no backend. This is the
`fundamentals` branch: it teaches the React UI in isolation — layout shell,
routing, TanStack Query, the kanban board, the command bar, dark mode — before
any services are introduced.

All data comes from an in-memory mock store (`src/mock/store.js`). Creating
tasks and dragging cards between kanban columns works for the lifetime of the
page (state resets on refresh). The `advanced` branch swaps this mock layer for
a real **Go + Postgres** backend without changing any UI component.

## Run it

```bash
npm install
npm run dev      # http://localhost:5173
```

```bash
npm run build    # production build to dist/
npm test         # Vitest component tests
```

## What's here

```
src/
├── components/
│   ├── layout/     AppShell · Sidebar · Topbar · CommandBar · ProfileMenu · ThemeToggle
│   ├── tasks/      TaskCard · TaskList · KanbanBoard · TaskCreateModal
│   └── ui/         Button · Input · Badge · Avatar · Logo
├── hooks/
│   └── useTasks.js     React Query hooks, backed by the mock store
├── mock/
│   └── store.js        in-memory projects + tasks (the stand-in backend)
├── pages/          DashboardPage · ProjectPage
└── styles/         brand tokens, db-* component classes, dark-mode atmosphere
```

## Not on this branch

No login/auth, no AI assistant, no network calls — those live on `advanced`.
The brand kit, component spec, and design tokens match the full DevBoard build.
