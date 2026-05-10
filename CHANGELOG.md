# Changelog

## 0.7.0

- **`<GameShell>`** — layout container (eyebrow, title, tagline, theme, footerLinks) replacing per-game App shells.
- **`<GameTheme>`** / **`useGameTheme()`** — context provider that applies a per-game color theme.
- **`createBus<E>()`** — generic typed pub/sub factory with `on`, `emit`, `off`.
- **`useGameTimer({ paused })`** — 250 ms tick timer returning `{ ms, reset, pause, resume }`.
- **`useVisibilityPause(onPause, onResume)`** — wires `visibilitychange` once.
- **`styles/game-tokens.css`** — canonical Apple-grade design tokens (ink/paper, cell states, marks, motion, Minesweeper extras).
- **`styles/sudoku-token-aliases.css`** — back-compat shim mapping `--digit-*` → `--mark-*` for Sudoku v0.6 consumers.
- **`bilko-host-kit emit-manifest`** — CLI that writes `dist/manifest.json` matching platform ManifestSchema.

## 0.6.0

- `useLeaderboard`, `useSaveState`, `useUnlocks` — game services hooks.

## 0.3.0

- Telemetry SDK: `initTelemetry`, `log`, `logError`, `flush`.
- `/testing` subpath: Playwright harness + golden-path template.
