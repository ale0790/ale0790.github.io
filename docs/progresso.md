# Progresso

## 2026-08-17 (-03) — Reformulação completa

### Estrutura
- CSS e JS extraídos para `assets/styles.css`, `assets/cv.css` e `assets/main.js`.
- Site agora tem 4 páginas (PT/EN como páginas reais, não toggle via JS — necessário para SEO):
  - `index.html` (PT) e `en/index.html` (EN) — portfólio.
  - `curriculo.html` (PT) e `en/resume.html` (EN) — currículo em coluna única, otimizado para impressão/PDF e parsing por ATS.
- CVs `.docx` copiados para `cv/` e disponíveis para download.

### Conteúdo
- Adicionados: seção "Resultados em produção" (thread dump JVM 200+ threads, slow query log MySQL 85 mil+ queries, CI/CD + APM, IA no ciclo de desenvolvimento), timeline de experiência com 4 cargos e datas, projetos Torneyo e Panel4You, seção de idiomas.
- Removidos: BetScope.app, Saúde no País, OCampeonato.com, Clube do Micro SaaS, Plantões Médicos Brasil.
- E-mail de contato alterado para `webhouse01@gmail.com` (mesmo dos currículos).

### SEO e metadados
- `<title>`, `description`, `canonical`, `robots`, Open Graph e Twitter Card em todas as páginas.
- `hreflang` pt-BR / en / x-default cruzando as versões de idioma.
- JSON-LD Schema.org (`Person` + `ProfilePage`) com cargo, skills, formação e `sameAs`.
- `robots.txt` e `sitemap.xml` criados.

### UX e acessibilidade
- Dark mode com `prefers-color-scheme` + toggle persistido em `localStorage`, sem flash de tela clara.
- Skip link, `aria-label`/`aria-expanded` na navegação, `:focus-visible`, suporte a `prefers-reduced-motion`.
- CSS de impressão com `@page A4` e quebras de página controladas.

## 2025-10-03 14:13 (-03)
- Corrigido `index.html`: removido bloco de CSS solto antes do `<!DOCTYPE html>` que estava sendo renderizado como texto na página.

## 2025-10-03 13:42 (-03)
- Melhorado espaçamento em `#soft-skills` no `index.html`:
  - Aumentado `gap` da grid (`.soft-skills-grid`).
  - Aumentado `padding` e `gap` dos cards (`.soft-skill`).
  - Aumentado tamanho do ícone (`.soft-skill-icon` de 50px para 64px) e `font-size`.

## 2025-10-03 13:41 (-03)
- Atualizado e-mail de contato para `alessandro@rangtecnologia.com.br` em:
  - `index.html` (hero social links e seção Contato)
  - `projeto.md` (Informações Pessoais)

## 2025-10-03 13:35 (-03)
- Adicionada foto de perfil (`profile.png`) na seção Hero (`.profile-img`).
- Ajustado contador de "Cofundação de Produto" para `10+` na seção `#about`.
- Corrigido CTA do Rang Saúde: removido de `#about` e inserido no bloco do projeto Rang Saúde em `#projects`.

## 2025-10-03 13:21 (-03)
- Criada seção `#services` no `index.html` após a seção de projetos:
  - Cartões: CTO-as-a-Service, Montagem de Equipe, Arquitetura & Integrações, DevOps & Observabilidade, Entrega de Software, Integrações SUS.
  - Reutilizado grid/cards de integrações para consistência visual.
  - CTA de cada card aponta para `#contact`.

## 2025-10-03 13:08 (-03)
- Adicionados projetos ao `index.html` na seção `#projects`:
  - Saúde no País (`https://saudenopais.com.br`).
  - Plantões Médicos Brasil (`http://plantoesmedicosbrasil.com.br/`).
- Mantido padrão visual (título `.project-title`, descrição, CTA com `target="_blank"` e `rel="noopener"`, separadores `<hr>`).

## 2025-09-24 09:52 (-03)
- Adicionadas seções ao `index.html`:
  - Projetos (inclui Rang Saúde, BetScope.app, Clube do Micro SaaS).
  - Integrações, Soft Skills, Contato, Footer.
- Adicionado JavaScript para:
  - Toggle do menu mobile.
  - Animações de entrada (`fade-in` com `IntersectionObserver`).
  - Botão "Voltar ao topo" com rolagem suave.
- Corrigido problema de duplicação de conteúdo após `</html>`.
- Criada pasta `docs/` com:
  - `instrucoes-ia.md`
  - `arquitetura.md`
  - `progresso.md`

## Pendências sugeridas
- Publicar em GitHub Pages ou Netlify.
- Otimizar performance (minificação, lazy-loading de ícones/imagens se adicionadas).
- Separar CSS e JS em arquivos próprios em uma futura refatoração.
