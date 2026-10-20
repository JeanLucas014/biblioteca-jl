# Biblioteca de componentes — JL

55 componentes em HTML, CSS e JavaScript puros, tema escuro, sem framework
e sem build. Cada um traz o código como está em produção mais um prompt pronto
pra recriar o componente em outro projeto, com as decisões e as armadilhas.

Vêm de dois lugares: o site [jeanlucasdev.com.br](https://jeanlucasdev.com.br)
e o BASE, o painel interno que uso pra tocar o trabalho.

## Para um agente

Comece por `components.json` — ele traz tudo: tokens, reset, categorias e os
55 componentes completos.

```
https://raw.githubusercontent.com/JeanLucas014/biblioteca-jl/main/components.json
```

Um componente por vez, quando você já sabe o id:

```
componentes/<id>.json    campos separados (prompt, html, css, js)
componentes/<id>.html    página pronta, com tokens e fontes — abre no navegador
```

Campos de um componente:

| campo | o que é |
|---|---|
| `id`, `nome`, `categoria`, `descricao` | identificação |
| `prompt` | o texto pra colar numa IA e reconstruir o componente do zero |
| `html`, `css`, `js` | o código; `js` é um módulo ES e nem todo componente tem |
| `demo` | linhas que só montam a demonstração — não fazem parte do componente |
| `altura`, `layout` | dicas de preview: altura em px, e `cheio` pra quem ocupa a largura toda |

Pra montar a página de um componente na mão: injete `tokens`, `reset`, a folha
de `fontes` (Google Fonts) e o `css`, depois o `html` e o `js` num
`<script type="module">`. É o que o `.html` pronto já faz.

## Categorias

| categoria | itens | ids |
|---|---|---|
| Botões | 2 | `botao-anti-metal`, `filtros-pill` |
| Navegação | 4 | `header-sticky`, `indicador-scroll`, `rodape`, `abas-sem-js` |
| Hero | 4 | `hero-sticky`, `hero-badge-scramble`, `hero-reveal`, `hero-crossfade` |
| Cards | 5 | `card-servico`, `card-diferencial`, `card-projeto`, `card-retrato`, `card-vitrine` |
| Seções | 10 | `secao-eyebrow`, `grade-blueprint`, `linha-do-tempo`, `faq-acordeao`, `cta-bloco`, `carrossel-coverflow`, `trilho-snap`, `faixas-sangradas`, `grade-hairline`, `secao-por-tom` |
| Formulários | 5 | `campos-formulario`, `progresso-wizard`, `seletor-segmentado`, `cards-escolha`, `form-whatsapp` |
| Efeitos | 5 | `spotlight-cursor`, `borda-card-brilho`, `reveal-scroll`, `hero-parallax`, `veu-duplo` |
| Loaders | 1 | `tela-carregamento` |
| Dashboard (BASE) | 19 | `base-tokens`, `base-stat-card`, `base-status-badge`, `base-source-pill`, `base-transaction-row`, `base-cadence-card`, `base-empty-state`, `base-goal-card`, `base-month-selector`, `base-sidebar`, `base-tabbar`, `base-dashboard`, `base-sheet`, `base-confirm-dialog`, `base-secret-field`, `base-amount-input`, `base-responsive-list`, `base-revenue-breakdown`, `base-annual-chart` |

## Licença

Domínio público (Unlicense) — use à vontade, sem precisar creditar.

Duas exceções que não são minhas: os caminhos dos ícones vêm do
[lucide](https://lucide.dev) (ISC) e o gráfico anual carrega
[Chart.js](https://www.chartjs.org) (MIT) pela CDN.

## Como este repo é atualizado

Gerado por script a partir do repositório do BASE, que é privado. Não edite os
arquivos aqui — a próxima geração passa por cima. Achou um problema, abra uma
issue.
