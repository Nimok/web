# Web

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                    | Action                                           |
| :------------------------- | :----------------------------------------------- |
| `pnpm install`             | Installs dependencies                            |
| `pnpm run dev`             | Starts local dev server at `localhost:3000`      |
| `pnpm run build`           | Build your production site to `./dist/`          |
| `pnpm run preview`         | Preview your build locally, before deploying     |
| `pnpm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `pnpm run astro -- --help` | Get help using the Astro CLI                     |

## DB

1. Update `db/schema.ts`
2. Run `pnpm run generate`
3. Run migrations
    * Locally: `wrangler d1 execute stormgateworld-web-production --local --file db/migrations/0000_uneven_naoko.sql`
    * Production: `wrangler d1 execute stormgateworld-web-production --file db/migrations/0000_uneven_naoko.sql`
