PRIVACIDADE — LP NO VERCEL (SEM SEO)
====================================

ARQUIVOS INCLUSOS
- robots.txt        → Bloqueia o rastreamento de todas as páginas (Disallow: /)
- vercel.json       → Envia cabeçalho X-Robots-Tag (noindex, nofollow, noarchive) + cache leve
- README_privacidade.txt → Este guia

ONDE COLOCAR
1) Suba estes arquivos na RAIZ do seu repositório (mesma pasta do index.html).
2) Faça commit no GitHub (branch usada pela Vercel).
3) A Vercel fará redeploy automático. Se não fizer, force 'Redeploy' no painel.

OBS IMPORTANTES
- Estes bloqueios NÃO afetam Google Ads, GA4, nem seus eventos de conversão.
- O objetivo é apenas evitar indexação orgânica pelos buscadores.
- Se no futuro quiser voltar ao SEO, remova as linhas de privacidade e redeploy.

TESTE RÁPIDO
- Acesse: https://SEU_DOMINIO/robots.txt  → Deve mostrar 'Disallow: /'
- Inspecione no DevTools (Network → Response Headers) → deve existir 'X-Robots-Tag: noindex, nofollow, noarchive'.
