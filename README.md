# Aetrux

[![Vite](https://img.shields.io/badge/Vite-5.x-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![React](https://img.shields.io/badge/React-18.x-149ECA?logo=react&logoColor=white)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.x-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

Aetrux is a cinematic, motion-first portfolio experience built with React, Vite, and TypeScript. It combines immersive sections, interactive UI layers, and media-rich storytelling with a fast static deployment pipeline.

## Overview

The project is a single-page front-end application focused on visual presentation, smooth interaction, and branded storytelling. It uses a componentized React architecture with Tailwind-driven styling and custom animation patterns.

## Features

- Immersive hero and section transitions with motion-optimized rendering
- Data-rich service and project modules for portfolio storytelling
- Video-backed media sections (`public/videos`) for strong visual previews
- Responsive UI primitives based on `shadcn/ui` and Radix components
- Route-level fallback page for robust client-side navigation

## Stack

- Runtime: React 18
- Build tool: Vite 5
- Language: TypeScript
- Styling: Tailwind CSS + custom CSS variables/utilities
- UI primitives: Radix + shadcn/ui patterns
- Testing: Vitest + Testing Library

## Typography

Aetrux intentionally uses a multi-font system loaded from Google Fonts in `src/index.css`:

- `Space Grotesk` for body and interface copy
- `Termina Test` (local OTF via `@font-face`) for display/headline moments
- `JetBrains Mono` for data-like technical labels
- `Instrument Serif` for stylistic accent text

Local font assets are stored in `font/termina-test/` and mapped with `font-display: swap`.

## Project Structure

```text
src/
  components/
  data/
  hooks/
  lib/
  pages/
public/
  videos/
assets/
```

## Local Development

```bash
npm install
npm run dev
```

App runs on `http://127.0.0.1:4444` (strict port).

## Build and Preview

```bash
npm run build
npm run preview
```

## Testing

```bash
npm run test
```

## Preview

### Social Preview

![Aetrux Open Graph Preview](./public/og-preview.jpg)

### Media Included

- `public/videos/lab-secure.mp4`
- `public/videos/lab-telemetry.mp4`
- `public/videos/lab-archive.mp4`
- `assets/footer.png`

## Deployment

This project is production-deployed on Vercel and configured for static front-end hosting from the repository root.

## Repository Hygiene

Generated directories and caches are excluded from version control (`node_modules`, `dist`, `.vercel`, `*.tsbuildinfo`). Large video assets are tracked with Git LFS.
