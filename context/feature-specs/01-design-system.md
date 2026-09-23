Read the Agents.md before starting.

We are adding the design system and UI primitive components.

Install and configure 'shadcn/ui'.

Add these shadcn components:

- Button
- Card
- Dialog
- Input
- Tabs
- Textarea
- ScrollArea

Do not modify the generate 'components/ui/*' files after installation.

Also install `lucide-react`.

Create `lib/utils.ts` with a reusable `cn()` heler for merging Tailwind classes.

Ensure all componets match the existing dark theme in global.css.

### Check when done
- All components import without errors
- `cn()` works properly
- No default light styling appears