# losell.nu
Familjen Losells gemensamma startsida.

Varje familjemedlem kan ha en egen sida på `<namn>.losell.nu`. Lägg till en rad i listan `.members` i `index.html` för att länka till den.

## Publicering
Sidan körs som Cloudflare Workern `losell-nu` (se `wrangler.jsonc`). Workers Builds är kopplat till det här repot, så en push till `main` publicerar sidan med `npx wrangler deploy`. Det som inte är incheckat och pushat hamnar aldrig live. Bara `index.html` laddas upp; övriga filer listas i `.assetsignore`.
