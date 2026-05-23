# Felipe Neves · Portfólio

Portfólio pessoal desenvolvido em HTML e CSS puro, com JavaScript vanilla. Design dark premium com acento verde-lima, tipografia editorial e animações de entrada escalonadas.

🔗 **[Ver ao vivo →](https://devnvs.github.io/Portfolio/)**

---

## Visão geral

Site de uma página com cinco seções navegáveis, pensado para apresentar perfil, projetos e habilidades de forma direta e visualmente forte — sem frameworks, sem dependências de build.

```
Portfolio/
└── index.html   # Todo o HTML, CSS e JS em um único arquivo autocontido
```

---

## Seções

| # | Seção | O que tem |
|---|-------|-----------|
| — | Hero | Nome em tipografia gigante, badge de disponibilidade com pulse animado, grid de fundo com glow e indicador de scroll |
| 01 | Sobre | Texto de apresentação + grid 2×2 de métricas em destaque |
| 02 | Projetos | Lista clicável com três projetos reais linkados para GitHub Pages e GitHub |
| 03 | Habilidades | Grid com quatro categorias: Front-End, Produto & Negócio, IA & Automação e Ferramentas |
| 04 | Por que eu | Quatro cards de diferenciais com ícone, título e descrição |
| — | Contato | Tipografia display + botões diretos para WhatsApp, LinkedIn, GitHub e e-mail |

---

## Decisões técnicas

**Arquivo único** — Todo o CSS e o JS estão embutidos no `index.html`. Facilita o deploy via GitHub Pages sem etapa de build e mantém o repositório simples.

**Tipografia via Google Fonts** — Syne (display e headings), DM Sans (corpo) e DM Mono (labels, tags e código). Carregadas com `preconnect` para minimizar latência.

**Scroll reveal com IntersectionObserver** — Cada bloco com a classe `.reveal` entra em cena conforme o usuário desce. Usa `requestAnimationFrame` para sincronizar com o ciclo de pintura e inclui fallback para browsers sem suporte ao observer.

**Grain overlay via SVG inline** — Textura de ruído aplicada como pseudo-elemento `::before` em posição fixa, sem arquivo externo.

**Grid CSS para layout responsivo** — `repeat(auto-fit, minmax(...))` nas seções de skills e diferenciais. Breakpoint em `768px` para mobile: navegação oculta, padding reduzido, grid de projetos recolhido.

---

## Paleta e tokens

```css
--bg:           #0b0b0b   /* fundo principal */
--bg2:          #111111   /* superfícies */
--bg3:          #181818   /* hover de cards */
--accent:       #c8f04a   /* verde-lima — cor de destaque */
--text:         #f0ede8   /* texto primário */
--text-secondary: #a09d99 /* texto de apoio */
--text-muted:   #6b6866   /* labels e elementos discretos */
--border:       rgba(255,255,255,0.07)
```

---

## Como usar localmente

Não há dependências de Node, npm ou bundler. Basta abrir o arquivo:

```bash
# Clone o repositório
git clone https://github.com/devnvs/Portfolio.git

# Abra no navegador
open Portfolio/index.html
```

Para emular o ambiente de produção com live reload:

```bash
# Com VS Code
# Instale a extensão Live Server e clique em "Go Live"

# Ou com Python (se instalado)
cd Portfolio
python3 -m http.server 8000
# Acesse http://localhost:8000
```

---

## Deploy

O site está publicado via **GitHub Pages** diretamente da branch `main`. Qualquer push para `main` atualiza o site ao vivo automaticamente.

Para ativar em um fork:
1. Vá em **Settings → Pages**
2. Source: `Deploy from a branch`
3. Branch: `main` / `/ (root)`
4. Salve — o site estará disponível em `https://<seu-usuario>.github.io/Portfolio/`

---

## Projetos linkados

| Projeto | Repositório | Demo |
|---------|-------------|------|
| Nevra Systems | [devnvs/nevra-systems](https://github.com/devnvs/nevra-systems) | [ver ao vivo](https://devnvs.github.io/nevra-systems/) |
| Nevra Randomizer | [devnvs/nevra-randomizer](https://github.com/devnvs/nevra-randomizer) | [ver ao vivo](https://devnvs.github.io/nevra-randomizer/) |
| Nevra Converter | [devnvs/nevra-converter](https://github.com/devnvs/nevra-converter) | — |

---

## Contato

**Felipe Neves Ferreira** · Dev Front-End · Fundador da [Nevra Systems](https://nevrasystems.com)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-devfelipeneves-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/devfelipeneves/)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-falar%20agora-25D366?style=flat&logo=whatsapp&logoColor=white)](https://wa.me/+5548988017617)
[![GitHub](https://img.shields.io/badge/GitHub-devnvs-181717?style=flat&logo=github&logoColor=white)](https://github.com/devnvs)

---

© 2026 Felipe Neves Ferreira · Nevra Systems
