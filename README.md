# Brabastore

Site estático (consulta de preços) hospedado no **Cloudflare Workers** (static assets, plano gratuito).

- `public/index.html` — página de preços
- `public/_redirects` — redireciona os links antigos `/precos.html` para `/`
- `wrangler.jsonc` — configuração do Cloudflare

## Deploy

**Pelo painel (recomendado):** Cloudflare → Workers & Pages → Create → Import a repository →
escolha `marcato-app/brabastore`. Deixe o build command vazio e o deploy command como
`npx wrangler deploy`. Cada push na branch de produção publica automaticamente.

**Pela linha de comando:** `npx wrangler deploy`
