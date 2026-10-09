# Vite Vue Template

A starter template for [bolt.diy](https://github.com/stackblitz-labs/bolt.diy).

## Purpose

This template is designed for use with **<https://github.com/stackblitz-labs/bolt.diy>**. bolt.diy fetches
these files at runtime and imports them into a fresh WebContainer project when you ask for a Vite + Vue project,
so everything here needs to install and build with no extra setup.

Modified by [Dustin Loring](https://github.com/Dustinwloring1988) (Dustinwloring1988) in October 2026.

## Stack

| Package | Version |
| --- | --- |
| Vue | ^3.5.43 |
| Vite | ^8.3.4 |
| @vitejs/plugin-vue | ^6.0.9 |
| vue-tsc | ^3.3.12 |
| TypeScript | ^6.0.3 |

Node 20 or newer is required.

## Commands

```bash
npm install   # install dependencies
npm run dev   # vite — dev server
npm run build # vue-tsc -b && vite build — type-check then build
npm run preview # vite preview — local preview server
```

## About this template

A Vite + Vue project with Vue 3 in standalone mode. The build uses `vue-tsc -b` for a full type-check
and `vite build` for production output. `main.ts` bootstraps the app with `standalone: true`.

## Upgraded to Vue 3.5.43, Vite 8, @vitejs/plugin-vue 6 (October 2026)

Moved from Vue 3.2, Vite 5, and @vitejs/plugin-vue 2/3. Each major was upgraded stepwise:
Vue 3.2 → 3.5 → 3.5.43, Vite 5 → 6 → 7 → 8, and @vitejs/plugin-vue was updated in tandem.
TypeScript was bumped from ~5.5.0 to ^6.0.3 to match Vue's peer requirements.

Vue 3.5.43 is the latest 3.x release. Vite 8 requires @vitejs/plugin-vue ^6, which provides Vite 8
compatibility improvements and better `vue-tsc` integration.

## Verification

- `npm install` and `npm run build` pass
- Confirmed the dev server starts with HMR and the app renders correctly
- `npm run preview` serves the production build locally