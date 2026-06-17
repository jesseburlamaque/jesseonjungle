# jesseonjungle

[![Hugo](https://img.shields.io/badge/Hugo-FF4088?style=flat&logo=hugo&logoColor=white)](https://gohugo.io/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Alpine.js](https://img.shields.io/badge/Alpine.js-8BC0D0?style=flat&logo=alpine.js&logoColor=black)](https://alpinejs.dev/)
[![PostCSS](https://img.shields.io/badge/PostCSS-DD3A0A?style=flat&logo=postcss&logoColor=white)](https://postcss.org/)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=github-actions&logoColor=white)](https://github.com/features/actions)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=flat&logo=github-pages&logoColor=white)](https://pages.github.com/)

Blog pessoal sobre GIS, sensoriamento remoto, LiDAR, biomassa e carbono florestal, construído com [Hugo](https://gohugo.io/) e tema [Compost](https://github.com/canstand/compost).

## Estrutura do projeto

| Arquivo/Pasta | Descrição |
|---------------|-----------|
| `hugo.toml` | Configuração principal do site (título, descrição, autor, links sociais, tema). |
| `content/_index.md` | **Página inicial** — texto de apresentação e links. |
| `content/posts/` | **Posts do blog** — arquivos `.md` com frontmatter TOML (`+++`). |
| `themes/compost/` | Tema Hugo (submodule). Evite editar diretamente; prefira sobrescrever em `layouts/`. |
| `layouts/partials/` | Templates customizados que sobrescrevem o tema (ex: `recent-articles.html`). |
| `public/` | Site estático gerado pelo Hugo. **Não edite manualmente** — gere com `hugo --gc --minify`. |
| `resources/_gen/` | Assets processados (CSS/JS). Gerados automaticamente. |

## Deploy

O site é publicado automaticamente via **GitHub Actions** a cada push na branch `main`.

- **Workflow:** `.github/workflows/hugo.yml`
- **Domínio:** [https://jesseburlamaque.github.io/jesseonjungle/](https://jesseburlamaque.github.io/jesseonjungle/)
- **Tema:** `compost` (submodule do GitHub)

### Como funciona

1. Você edita os arquivos em `content/` ou `hugo.toml`.
2. Faz commit e push para o `main`.
3. O GitHub Actions executa:
   - Checkout do repositório com submodules
   - Instalação do Hugo (versão latest, extended)
   - Build com `hugo --minify`
   - Deploy para o GitHub Pages

### Como adicionar um novo post

1. Crie um arquivo em `content/posts/nome-do-post.md`.
2. Use o frontmatter TOML:
   ```toml
   +++
   date = '2026-06-16T22:09:28-03:00'
   draft = false
   title = 'Título do Post'
   tags = ['tag1', 'tag2']
   +++
   ```
3. Escreva o conteúdo em Markdown abaixo do frontmatter.
4. Commit e push. O deploy acontece automaticamente.

