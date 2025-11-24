# Portfolio - Rafael Barros

Estrutura do projeto e instruções rápidas.

Estrutura proposta:

- `index.html` — Página principal do portfolio (na raiz).
- `assets/`
  - `css/style.css` — Estilos personalizados (complemento ao Tailwind CDN).
  - `js/main.js` — JavaScript do site (mobile menu, animações, utilitários).
  - `img/` — Imagens e screenshots dos projetos (coloque suas imagens aqui).
- `projects/` — Páginas individuais ou demos de projetos.
- `README.md` — Este arquivo.

Como testar localmente:

1. Abrir diretamente `index.html` no navegador (modo estático), ou
2. Servir com um servidor simples (recomendado para evitar problemas de CORS):

```bash
# Python 3
python3 -m http.server 8000
# então abra http://localhost:8000
```

SEO e distribuição (passos rápidos):

- Substitua `https://yourdomain.com/` nas meta tags do `index.html` e no `sitemap.xml` pelo seu domínio real antes de enviar ao Google.
- Envie `https://yourdomain.com/sitemap.xml` ao Google Search Console (menu Sitemaps → inserir URL do sitemap).
- Verifique `robots.txt` em `https://yourdomain.com/robots.txt` após deploy para confirmar acesso.

Imagens e acessibilidade:
- `assets/img/` contém placeholders SVG otimizados usados nas previsualizações de projeto e para Open Graph.
- Adicione versões otimizadas (WebP) para produção e defina `alt` descritivo para todas as imagens.

Próximos passos recomendados (opcional):
- Submeter site ao Google Search Console e monitorar cobertura e performance.
- Configurar uma pipeline de build para gerar imagens otimizadas (ex: WebP) e minificar CSS/JS.
- Implementar per-page metadata (cada projeto com seu title/description/og:image).

Como adicionar um novo projeto:

- Crie um arquivo em `projects/` (ex: `projects/meu-projeto.html`).
- Adicione screenshots em `assets/img/` e referencie nos HTML.
- Atualize a seção de Portfólio em `index.html` para incluir/ligar para o novo projeto.

Se quiser, eu posso:
- Adicionar um pequeno script de build (Parcel/Vite) para suporte a assets.
- Converter para uma SPA com React/Vue/Next.

