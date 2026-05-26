# AI Agent Guide for my-bingo-mixer

This repository is a small React + Vite + Tailwind CSS app with a teaching/lab focus.
Use this guide to understand the project quickly and avoid common mistakes.

## What this project is
- A React 19 app built with Vite and TypeScript.
- Tailwind CSS v4 is used for styling via `@import "tailwindcss"` in `src/index.css`.
- The game logic is split between `src/hooks/useBingoGame.ts` and `src/utils/bingoLogic.ts`.
- The app is a teaching/demo project with workshop guides in `workshop/`.

## Key commands
- `npm install` — install dependencies
- `npm run dev` — start local Vite development server
- `npm run build` — run TypeScript build and Vite production build
- `npm run lint` — run ESLint on the repository
- `npm test` — run Vitest unit tests

## Important files and directories
- `src/App.tsx` — app shell and entry point
- `src/components/` — UI components like `BingoBoard.tsx`, `BingoModal.tsx`, `GameScreen.tsx`, and `StartScreen.tsx`
- `src/hooks/useBingoGame.ts` — game state management and logic coordination
- `src/utils/bingoLogic.ts` — pure bingo board logic with tests in `src/utils/bingoLogic.test.ts`
- `src/data/questions.ts` — bingo question content
- `src/index.css` — Tailwind v4 import and global styling
- `public/` — static assets, if needed
- `workshop/` — learning guide content; reference it rather than duplicating it

## Style and conventions
- Prefer function components and hooks.
- Keep state handling in `useBingoGame.ts` and keep UI components focused on rendering and interaction.
- Use Tailwind classes directly and leverage CSS variables if needed.
- Keep logic in plain TypeScript modules for easier testing.

## What agents should avoid
- Avoid rewriting the entire app unless asked for a full redesign.
- Avoid introducing a custom Tailwind config, since the project currently uses standard v4 CSS imports.
- Avoid changing workshop docs unless the request is about documentation content.

## Additional guidance
- There is existing agent-focused guidance under `.github/instructions/` for frontend design and Tailwind v4.
- The repo includes a `.devcontainer/devcontainer.json` for Codespaces/dev container support.
- Use `README.md` and `workshop/GUIDE.md` as the authoritative reference for project intent, setup, and contribution expectations.
