# CLAUDE.md — RBSIMPORTGAMES

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** RBSIMPORTGAMES
**Nicho:** Entretenimento
**Keywords:** Me chamo Rodrigo Barbosa tenho 34 anos escrevo para o rbsimportgames e
**Paleta de cores:** gold | **Fonte:** montserrat

Me chamo Rodrigo Barbosa, tenho 34 anos, escrevo para o rbsimportgames e aqui irei contar um pouco das minhas experiências como gamer. Sou um entusiasta com sede de conhecimento. Meu objetivo principal é passar todo minha vivencia ao longo dos anos no mundo dos games. Desde sempre eu gosto de dividir conhecimento e o rbsimportgames é a minha válvula de escape. Aqui é onde eu escrevo tudo que eu sei sobre o nosso mundo. Há 1 ano acabei trabalhando duro para a criação do site e acredito muito que atingirei meu objetivo de trazer muito conteúdo sobre o mundo dos games. Games de todas as idades e dos mais váriados níveis, do iniciante ao avançado são muito bem vindos ao meu site. Com certeza tenho bastante conteúdo para todos. Aqui você sempre terá um incrível portal de comunicação no mundo do games. Você vai poder sempre se manter antenado assinando a minha newsletter.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-J |
| Hero | Hero-F |
| Features | Features-G |
| About Section | About-H |
| Posts | Posts-B |
| Footer | Footer-D |
| Página Sobre | Sobre-A |
| Página Contato | Contato-D |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
