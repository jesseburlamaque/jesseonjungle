---
noteId: "ab39cfc069f611f18bf8c9959cc40ea6"
tags: []

---

# JesseonJungle

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

## Como adicionar um novo post

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
4. Execute `hugo --gc --minify` para gerar o site.
5. Commite e envie para o GitHub.
