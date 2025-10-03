# Arquitetura da Página e Diretrizes

## Visão Geral
- Projeto: site pessoal estático (`index.html`) com CSS inline e JS leve para interações.
- Paleta: Gradientes roxo/azul (`#667eea`/`#764ba2`) e destaques `#2563eb`.
- Tipografia: Segoe UI / sistema.

## Estrutura de Seções (index.html)
1. Header fixo com navegação e menu mobile.
2. Hero (perfil, título, CTA e links sociais).
3. Sobre (texto + estatísticas).
4. Formação (cards responsivos).
5. Habilidades (categorias com tags).
6. Experiência (card detalhado com conquistas).
7. Projetos (Rang Saúde, BetScope.app, Clube do Micro SaaS).
8. Integrações (grid de integrações relevantes).
9. Soft Skills (competências comportamentais).
10. Contato (informações + formulário sem backend).
11. Footer (direitos autorais).
12. Botão Voltar ao Topo e JS de interação.

## JavaScript
- Menu mobile: toggle `.nav-links.active` via `.menu-toggle`.
- Animações: `IntersectionObserver` adiciona `.visible` a `.fade-in`.
- Scroll-to-top: botão `.scroll-top` aparece após 600px.
- Acessibilidade: botões com `aria-label`, links externos com `rel="noopener"`.

## Responsividade
- Breakpoint principal: 768px (nav colapsa, grids em 1 coluna onde aplicável).

## Boas Práticas
- Manter HTML semântico e classes coesas.
- Evitar duplicações de seções/markup.
- Em futura evolução, considerar separar `style.css` e `main.js`.

## Próximos Passos Sugeridos
- Adicionar seção de depoimentos/casos de sucesso.
- Adicionar projetos adicionais (se houver) com imagens/logos otimizadas.
- Pipeline simples de publicação (GitHub Pages/Netlify).
