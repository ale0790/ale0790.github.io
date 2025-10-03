# Progresso

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
