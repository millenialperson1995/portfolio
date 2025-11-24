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

Como adicionar um novo projeto:

- Crie um arquivo em `projects/` (ex: `projects/meu-projeto.html`).
- Adicione screenshots em `assets/img/` e referencie nos HTML.
- Atualize a seção de Portfólio em `index.html` para incluir/ligar para o novo projeto.

Se quiser, eu posso:
- Adicionar um pequeno script de build (Parcel/Vite) para suporte a assets.
- Converter para uma SPA com React/Vue/Next.

