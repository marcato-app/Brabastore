# Brabastore

Site da Braba da Apple (www.ibrabastore.com.br), hospedado no **Cloudflare Workers** (static assets, plano gratuito).

- `public/index.html`: bio / link na bio (página principal)
- `public/precos.html`: consulta de preços (abre em `/precos`)
- `public/assets/`: logo e foto de capa
- `wrangler.jsonc`: configuração do Cloudflare

## Deploy

**Pelo painel:** Cloudflare → Workers & Pages → Create → Import a repository →
escolha `marcato-app/brabastore`. Build command vazio, deploy command `npx wrangler deploy`.
Cada push na branch de produção publica automaticamente.

**Pela linha de comando:** `npx wrangler deploy`
