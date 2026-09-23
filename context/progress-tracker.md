# Progress Tracker

Update this file whenever the current phase, active feature, or implementation state changes.

## Current Phase

- Design system ✓

## Current Goal

- Define the next implementation unit.

## Completed

- **Feature spec 01 — Design system and UI primitives**
  - Installed and configured `shadcn/ui` (style: `base-nova`, Tailwind v4, CSS variables).
  - Added all required shadcn components: `Button`, `Card`, `Dialog`, `Input`, `Tabs`, `Textarea`, `ScrollArea` → `components/ui/`.
  - Installed runtime dependencies: `@base-ui/react`, `class-variance-authority`, `cn`, `lucide-react`, `clsx`, `tailwind-merge`, `tw-animate-css`.
  - Created `lib/utils.ts` with a `cn()` helper (clsx + tailwind-merge).
  - Wrote `app/globals.css` with the full dark-only design token system:
    - App custom tokens (`--bg-base`, `--text-primary`, `--accent-primary`, etc.).
    - shadcn semantic tokens mapped to app palette (`--background`, `--foreground`, `--card`, etc.).
    - `@theme inline` block exposing all tokens as Tailwind utilities (`bg-base`, `text-copy-primary`, `text-brand`, `bg-accent-dim`, etc.).
  - Pinned `class="dark"` on `<html>` in `app/layout.tsx` — all `dark:*` shadcn variants are always active.
  - TypeScript type-check: zero errors.

## In Progress

- None.

## Next Up

- Add the next planned feature unit here.

## Open Questions

- Add unresolved product or implementation questions here.

## Architecture Decisions

- shadcn base is `base-nova` (uses `@base-ui/react` primitives instead of Radix UI).
- Generated `components/ui/*` files are untouched post-install; app-level styling lives in `globals.css` and app-level components.
- The app is permanently dark: no light theme, no theme toggle. `class="dark"` is hardcoded on `<html>`.

## Session Notes

- Feature spec 01 complete. All spec checklist items pass.
- Next session should start by picking up the next feature unit from `context/feature-specs/`.
