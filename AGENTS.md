# Instruções pra agentes

Este repositório é dado, não código de aplicação. Não há build, teste nem
dependência pra instalar.

1. Leia `components.json` (tudo) ou `componentes/<id>.json` (um).
2. Copie `html`, `css` e `js` pro projeto de destino. O CSS depende dos tokens
   em `tokens` (campo do JSON) — leve junto ou mapeie as custom properties pras
   do projeto.
3. `demo` é só a demonstração: não copie junto sem querer.
4. Precisa adaptar pra React/Vue/Svelte? Use o `prompt` do componente como
   especificação — ele carrega as decisões e as armadilhas que o código sozinho
   não conta.

Os componentes são HTML/CSS/JS puros e assumem fundo escuro. Fontes: Sora,
Manrope e JetBrains Mono, carregadas do Google Fonts pela URL em `fontes`.
