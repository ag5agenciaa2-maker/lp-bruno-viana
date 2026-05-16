# SITE DNA — VIANA ASSOCIADOS

**Nicho:** Advocacia Trabalhista Especializada — Defesa de Motoristas e Rodoviários (caminhoneiros, motoristas de ônibus) no Rio de Janeiro
**Posicionamento:** Escritório de nicho hiper-especializado que transmite autoridade técnica e proximidade com o trabalhador; o visual equilibra seriedade institucional (vermelho profundo + ouro) com linguagem acessível ao público rodoviário. A sensação de impacto é de "esse advogado é para mim", sem afastar com jargão elitista.
**Data de criação:** 2025

---

## IDENTIDADE VISUAL

### Paleta de Cores

| Variável CSS / Token Tailwind | Hex | Função Específica no Layout |
|---|---|---|
| `primary` / `--color-primary` | `#8B1E22` | Cor estrutural principal: botões primários, border-top dos cards de especialidades, header CTA, fundo da seção "Como Funciona", painel lateral do formulário de contato, cor do thumb da scrollbar |
| `secondary` / `--color-gold` | `#D4AF37` | Acento dourado: border-bottom dos headings do footer, border-top alternado nos cards, ícones de materialização dentro dos cards (estado hover), badges hero, numeração dos steps, sublinhado decorativo `.footer-heading::after` |
| `background-light` | `#F9F7F2` | Fundo alternado das seções Áreas, FAQ — tom bege-papel que quebra o branco puro e adiciona sofisticação editorial |
| `background-dark` | `#1A1A1A` | Fundo global dark mode + footer premium; valor base da sobreposição hero |
| `surface-light` | `#FFFFFF` | Fundo dos cards em modo claro, área do formulário, seção Sobre |
| `surface-dark` | `#262626` | Fundo dos cards em modo escuro |
| `text-light` | `#2D2D2D` | Texto principal modo claro |
| `text-dark` | `#E5E5E5` | Texto principal modo escuro |
| `rgba(212, 175, 55, 0.3)` | Gold 30% | Border dos ícones sociais no footer (estado normal) |
| `rgba(212, 175, 55, 0.15)` | Gold 15% | Background dos ícones sociais no hover |
| `rgba(212, 175, 55, 0.2)` | Gold 20% | Border-bottom dos headings no footer |
| `rgba(212, 175, 55, 0.15)` | Gold 15% | Border-top do footer-bottom |
| `rgba(26, 26, 26, 0.85)` | Dark 85% | Primeira camada do gradiente hero (background-image do `bg-hero-pattern`) |
| `rgba(139, 30, 34, 0.9)` | Primary 90% | Segunda camada do gradiente hero (coloração avermelhada inferior) |
| `#25D366` | WhatsApp Green | Botão flutuante WhatsApp |
| `#128C7E` | WhatsApp Dark | Hover do botão flutuante WhatsApp |
| `#661518` | Red Escuro | Hover da scrollbar thumb |
| `rgba(255,255,255,0.05)` | White 5% | Decorações circulares absolutas no painel de contato |
| `rgba(255,255,255,0.20)` | White 20% | Border dos cards de steps |

### Tipografia

| Elemento | Família | Peso | Tamanho Exato | Observações |
|---|---|---|---|---|
| H1 Hero | Playfair Display (serif) | 700 | `text-4xl` → `md:text-5xl` → `lg:text-6xl` (2.25rem / 3rem / 3.75rem) | `leading-tight`; texto branco sobre overlay escuro |
| Subtitle Hero | Playfair Display (serif) | 400 (italic) | `text-2xl` → `md:text-3xl` (1.5rem / 1.875rem) | Classe `italic`; cor `text-secondary` (#D4AF37) |
| Descrição Hero | Roboto (sans-serif) | 300 | `text-lg` → `md:text-xl` (1.125rem / 1.25rem) | `font-light`; `max-w-2xl`; cor `text-gray-200` |
| H2 Seções | Playfair Display (serif) | 700 | `text-3xl` → `md:text-4xl` (1.875rem / 2.25rem) | Usado em Áreas, Sobre, FAQ; cor `text-primary` |
| H3 Cards | Playfair Display (serif) | 700 | `text-xl` (1.25rem) | `font-display text-xl font-bold mb-3` |
| Body/Parágrafos | Roboto (sans-serif) | 400 | `text-base` / `text-lg` (1rem / 1.125rem) | `leading-relaxed`; cor `text-gray-600` / `dark:text-gray-400` |
| Body Sobre (destaque) | Roboto (sans-serif) | 500 | `text-lg` (1.125rem) | `font-medium`; cor `text-gray-700` |
| Nav Links Header | Roboto (sans-serif) | 400–500 | `text-sm` (0.875rem) | `hover:text-primary`; espaçamento `space-x-8` |
| Steps Heading | Playfair Display (serif) | 600 | `text-xl` (1.25rem) | Cor branca sobre fundo primary |
| Steps Descrição | Roboto (sans-serif) | 400 | `text-sm` (0.875rem) | Cor `white/80` |
| Footer Heading | Playfair Display (serif) | 700 | `1rem` | `border-bottom: 1px solid gold/20` + pseudo-elemento `::after` dourado |
| Footer Links | Roboto (sans-serif) | 400 | `0.9rem` | Cor `white/65`; hover `gold`; prefixo `›` dourado |
| Footer Contato | Roboto (sans-serif) | 400 | `0.88rem` | `line-height: 1.5`; ícone SVG dourado inline |
| Footer Bottom | Roboto (sans-serif) | 400 | `0.82rem` | Cor `white/50` |
| Labels Form | Roboto (sans-serif) | 500 | `text-sm` (0.875rem) | `block text-sm font-medium text-gray-700` |
| Badge Hero | Roboto (sans-serif) | 400 | `text-sm` (0.875rem) | `border border-secondary/50 rounded-full bg-black/30 backdrop-blur-sm` |
| Ícones | Material Icons (icon font) | — | `material-icons` (24px padrão) | Usados em cards, lista hero, formulário de contato |

### Estilo Geral

Design editorial jurídico de nicho, construído sobre uma grade dual-tone (vermelho institucional + ouro editorial) que evoca autoridade sem afastar o trabalhador. A arquitetura segue progressão temática: Hero imersivo com parallax fotográfico (fundo rodoviário real) → seções alternadas bege-papel/branco para respiração visual → seção de processo em bloco monocromático primary para contraste máximo → fechamento com footer premium full-dark. Playfair Display ancora a seriedade serif em headings; Roboto garante legibilidade moderna no corpo. O sistema dark-mode é implementado via classes Tailwind (`dark:`) em todos os componentes, mas sem alterar a identidade visual — as cores de acento (primary e gold) permanecem constantes em ambos os modos.

---

## LAYOUT — SEÇÃO POR SEÇÃO

### SEÇÃO 1 — Header (Navegação Fixa)

**Estrutura:** `fixed` no topo, `z-50`, full-width. Internamente `flex justify-between items-center h-24` dentro de `max-w-7xl mx-auto px-4 sm:px-6 lg:px-8`. Três blocos: logo (esquerda), nav (centro, `hidden md:flex space-x-8`), ações (direita: toggle dark + CTA WhatsApp).

**Fundo:** `bg-surface-light/95 dark:bg-surface-dark/95 backdrop-blur-sm shadow-md border-b border-primary/20` — vidro fosco com leve borda inferior vermelha.

**Elementos Restritos:**
- Logo: `h-14 md:h-16 w-auto object-contain rounded-full shadow-md`
- Links: cor `text-gray-700 dark:text-gray-300`, hover `text-primary`
- Botão CTA: `bg-primary text-white px-5 py-2.5 rounded shadow-sm hover:shadow-md hover:bg-red-900 flex items-center gap-2 font-medium`
- Mobile: hamburguer `md:hidden`, menu drawer sobreposto

**Animação:** Sem entrance animation. O `shadow-md` persiste durante o scroll (position fixed). Transições `transition` padrão nos links.

**Micro-interações:**
- Logo: `hover:opacity-90` (fade leve)
- Nav links: `hover:text-primary` (color transition)
- Botão CTA: `hover:bg-red-900` (escurece vermelho), `hover:shadow-md` (eleva sombra)
- Dark toggle: não especificado visualmente

**Diferenciador Visual:** O header combina logo com `rounded-full` (logo circular, incomum em sites jurídicos) com a borda inferior `border-primary/20` — sutil marcação de identidade sem peso visual.

---

### SEÇÃO 2 — Hero (#home)

**Estrutura:** `relative pt-24 pb-16 lg:pt-40 lg:pb-32`. Layout interno `flex flex-col items-center text-center` com `max-w-2xl mx-auto` para a coluna de conteúdo. Imagem de fundo com sobreposição dupla de gradiente (dark → primary).

**Fundo:**
```css
background-image: linear-gradient(
  rgba(26, 26, 26, 0.85),
  rgba(139, 30, 34, 0.9)
), url('img/hero-bg-rodoviario.png');
background-size: cover;
background-position: center;
background-attachment: fixed; /* parallax — desabilitado em mobile via @media */
```

**Elementos Restritos:**
- Badge topo: `inline-block px-3 py-1 mb-4 border border-secondary/50 rounded-full bg-black/30 backdrop-blur-sm` com texto `text-secondary text-sm`
- H1: `font-display text-4xl md:text-5xl lg:text-6xl font-bold leading-tight text-white mb-4`
- Subtitle itálico: `text-secondary italic text-2xl md:text-3xl font-display mb-6`
- Parágrafo descrição: `text-lg md:text-xl text-gray-200 mb-8 max-w-2xl mx-auto font-light`
- Lista de benefícios: `space-y-3` com ícones `material-icons text-secondary` inline + texto `text-gray-200`
- Botões: `flex flex-col sm:flex-row gap-4 mt-10 justify-center`
  - Gold CTA: `bg-secondary text-primary-900 font-bold px-8 py-3.5 rounded hover:bg-yellow-500 transition shadow-lg`
  - Outline: `bg-transparent border-2 border-white text-white font-medium px-8 py-3.5 rounded hover:bg-white hover:text-primary transition`

**Animação:** Classe `.fade-in-up` nos elementos principais — `opacity: 0; transform: translateY(20px)` → `opacity: 1; transform: translateY(0)` em `0.8s ease-out`. Parallax `bg-fixed` no desktop, desabilitado em mobile (`background-attachment: scroll`).

**Micro-interações:**
- Botão Gold: `hover:bg-yellow-500` (shift de saturação)
- Botão Outline: `hover:bg-white hover:text-primary` (inversão completa de cor)

**Diferenciador Visual:** Gradiente duplo que inicia em escuro neutro e termina em vermelho-primary — transição que ambienta o fundo fotográfico dentro da identidade cromática sem filtro monocromático genérico. Badge com `backdrop-blur-sm` no Hero é detalhe editorial raramente visto em LPs jurídicas.

---

### SEÇÃO 3 — Áreas de Atuação (#areas)

**Estrutura:** `py-20 bg-background-light dark:bg-background-dark`. Grid interno: `grid md:grid-cols-2 gap-8 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8`. 4 cards em 2×2 no desktop, 1 coluna no mobile.

**Fundo:** `bg-background-light` (`#F9F7F2`) — bege-papel, sem imagem, sem gradiente.

**Elementos Restritos:**
- Header da seção: `text-center mb-16` com H2 `font-display text-3xl md:text-4xl font-bold text-primary mb-4` + parágrafo subtitle `text-gray-600 max-w-2xl mx-auto`
- Cada card: `bg-surface-light dark:bg-surface-dark p-8 rounded shadow-lg border-t-4 hover:-translate-y-2 transition duration-300 group`
- Border-top alternado: `border-secondary` (cards 1 e 4) | `border-primary` (cards 2 e 3)
- Icon wrapper: `w-14 h-14 bg-secondary/10 rounded-full flex items-center justify-center mb-6 group-hover:bg-secondary transition`
- Ícone material: `material-icons text-secondary text-3xl group-hover:text-white transition`
- H3: `font-display text-xl font-bold mb-3 text-text-light dark:text-text-dark`
- Parágrafo: `text-gray-600 dark:text-gray-400 leading-relaxed`

**Animação:** `hover:-translate-y-2 transition duration-300` (lift 2px para cima em 300ms).

**Micro-interações:**
- Card: `-translate-y-2` no hover (levita)
- Icon wrapper: `group-hover:bg-secondary` (fundo fica ouro sólido)
- Ícone material: `group-hover:text-white` (ícone branqueia dentro do fundo ouro)
- Transição do ícone: `transition` (300ms padrão)

**Diferenciador Visual:** Uso de `group` do Tailwind para orquestrar múltiplas transições simultâneas (fundo do wrapper + cor do ícone) sem JavaScript. Border-top alternada entre secondary e primary cria ritmo visual sem uniformidade mecânica.

---

### SEÇÃO 4 — Sobre o Escritório (#about)

**Estrutura:** `py-20 bg-white dark:bg-surface-dark relative overflow-hidden`. Grid interno: `grid lg:grid-cols-2 gap-12 items-center max-w-7xl mx-auto`.

**Fundo:** `bg-white dark:bg-surface-dark` + decoração skew lateral: `absolute right-0 top-0 w-1/3 h-full bg-gray-50 dark:bg-black/20 skew-x-12` — bloco inclinado que quebra a retangularidade da seção.

**Elementos Restritos:**
- Coluna texto (esquerda):
  - H2: `font-display text-3xl md:text-4xl font-bold text-primary mb-6`
  - Parágrafo destaque: `text-lg text-gray-700 dark:text-gray-300 mb-6 font-medium`
  - Parágrafos secundários: `text-gray-600 dark:text-gray-400 mb-6 leading-relaxed`
  - Grid stats 2 colunas: `grid grid-cols-2 gap-6 mt-8`
  - Cada stat: `border-l-2 border-secondary pl-4` com número `font-display text-3xl font-bold text-primary` e label `text-sm text-gray-600`
- Coluna imagem (direita):
  - Wrapper: `relative`
  - Imagem: `rounded shadow-2xl w-full object-cover h-[500px]` com `loading="lazy"`
  - Badge absoluto: `absolute -bottom-6 -left-6 bg-primary p-6 rounded shadow-xl hidden md:block` com texto branco e ícone material

**Animação:** `fade-in-up` aplicado na entrada dos elementos ao scroll.

**Micro-interações:** Sem hover interativo nos elementos principais. Badge e decoração são estáticos.

**Diferenciador Visual:** O bloco `skew-x-12` absoluto na direita cria uma divisão diagonal sutil que diferencia essa seção de um simples two-column-grid. O badge `-bottom-6 -left-6` com posição negativa sobrepõe o limite da imagem — técnica editorial que rompe o grid de forma controlada.

---

### SEÇÃO 5 — Como Funciona (Steps)

**Estrutura:** `py-20 bg-primary text-white relative`. Grid interno: `grid grid-cols-1 md:grid-cols-4 gap-8 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative`. Linha horizontal conectora: `hidden md:block absolute top-1/2 left-0 w-full h-0.5 bg-white/20 -z-10`.

**Fundo:** `bg-primary` (#8B1E22) — bloco monocromático de alto contraste. Sem imagem, sem gradiente.

**Elementos Restritos:**
- Header: `text-center mb-16` com H2 `font-display text-3xl md:text-4xl font-bold text-white mb-4`
- Cada card step: `bg-primary border border-white/20 p-6 rounded-lg text-center hover:bg-white/10 transition duration-300 relative`
- Número círculo: `w-12 h-12 bg-secondary text-primary font-bold text-xl rounded-full flex items-center justify-center mx-auto mb-4 shadow-lg` (48×48px, ouro com número vermelho)
- Heading step: `text-xl font-display font-semibold mb-2 text-white`
- Descrição step: `text-sm text-white/80`
- Linha conectora: `position: absolute; top: 50%; left: 0; width: 100%; height: 0.5px; background: rgba(255,255,255,0.20)`

**Animação:** `transition duration-300` nos cards (300ms). Linha conectora é estática.

**Micro-interações:**
- Card hover: `hover:bg-white/10` (fundo levemente branco sobre primary — sutil)

**Diferenciador Visual:** Seção inteiramente em `bg-primary` com a numeração em círculos `bg-secondary` — inversão da paleta: onde o restante do site usa primary sobre backgrounds claros, aqui o background É o primary. A linha conectora `white/20` atrás dos cards simula um processo visual sem depender de SVG ou animação.

---

### SEÇÃO 6 — Dúvidas Frequentes (#faq)

**Estrutura:** `py-20 bg-background-light dark:bg-background-dark`. Container: `max-w-4xl mx-auto px-4 sm:px-6 lg:px-8`. Lista: `space-y-4`. Usa elemento HTML nativo `<details>/<summary>` para accordion sem JavaScript.

**Fundo:** `bg-background-light` (`#F9F7F2`) — retorna ao bege da seção de áreas (ritmo visual alternado).

**Elementos Restritos:**
- Header: `text-center mb-16` com H2 primary + subtitle gray
- `<details>`: `group bg-surface-light dark:bg-surface-dark rounded-lg shadow-sm`
- `<summary>`: `flex justify-between items-center font-medium cursor-pointer list-none p-6 text-lg`
- Chevron SVG: `transform group-open:rotate-180 transition-transform duration-200`
- Conteúdo: `text-gray-600 dark:text-gray-400 mt-0 px-6 pb-6 leading-relaxed border-t border-gray-100 dark:border-gray-700 pt-4`

**Animação:** `group-open:rotate-180 transition-transform duration-200` no ícone chevron (200ms). Expansão do conteúdo é nativa do `<details>` sem animação CSS adicional.

**Micro-interações:**
- Summary hover: cursor pointer
- Chevron: rotação 180° ao abrir (`group-open:` do Tailwind via JS polyfill ou CSS selector `details[open]`)

**Diferenciador Visual:** Accordion via HTML semântico nativo (`<details>/<summary>`) em vez de JavaScript — detalhe técnico que melhora acessibilidade e performance sem sacrifício visual. `list-none` no summary remove o marcador padrão do browser.

---

### SEÇÃO 7 — Contato (#contact)

**Estrutura:** `py-12 bg-gray-100 dark:bg-[#1f1f1f]`. Card central: `bg-surface-light dark:bg-surface-dark rounded-xl shadow-2xl overflow-hidden flex flex-col md:flex-row max-w-5xl mx-auto`. Split: formulário (esquerda, `w-full md:w-3/5 p-8 md:p-12`) + painel info (direita, `bg-primary w-full md:w-2/5 p-8 md:p-12 text-white`).

**Fundo:** Wrapper `bg-gray-100 dark:bg-[#1f1f1f]`. Card com `rounded-xl shadow-2xl overflow-hidden`. Painel direito: `bg-primary` com 2 círculos decorativos absolutos (`rounded-full bg-white/5`): `absolute top-0 right-0 -mr-16 -mt-16 w-64 h-64` e `absolute bottom-0 left-0 -ml-16 -mb-16 w-40 h-40`.

**Elementos Restritos:**
- H2 form: `font-display text-2xl font-bold text-primary mb-6`
- Labels: `block text-sm font-medium text-gray-700 dark:text-gray-300`
- Inputs/Select/Textarea: `mt-1 block w-full rounded-md border-gray-300 dark:border-gray-600 dark:bg-background-dark shadow-sm focus:border-primary focus:ring focus:ring-primary/20 transition`
- Espaçamento entre fields: `space-y-6`
- Submit: `w-full bg-primary text-white font-bold py-3.5 px-4 rounded hover:bg-red-900 transition focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary`
- Help text: `text-xs text-gray-500 text-center mt-4`
- Painel info: H3 `font-display text-2xl font-bold text-white mb-8` + items `flex items-start gap-4` com ícone material e texto `text-white/90`
- Botão WhatsApp no painel: `bg-[#25D366] hover:bg-[#128C7E] text-white font-medium py-3 px-6 rounded flex items-center justify-center gap-2 transition w-full mt-4`

**Animação:** `transition` nos inputs (focus). Sem entrada animada.

**Micro-interações:**
- Inputs: `focus:border-primary focus:ring focus:ring-primary/20` (ring glow vermelho ao focar)
- Submit: `hover:bg-red-900` + `focus:ring-2 focus:ring-offset-2 focus:ring-primary`
- WhatsApp painel: `hover:bg-[#128C7E]`

**Diferenciador Visual:** O split do card com `overflow-hidden` e `rounded-xl` cria um container unificado onde o painel direito em primary com os círculos decorativos em `white/5` funciona como painel de informações que parece "fazer parte" do formulário — em vez de dois blocos separados.

---

### SEÇÃO 8 — Footer Premium

**Estrutura:** CSS Grid nativo (não Tailwind): `grid-template-columns: 1.5fr 1fr 1fr 1.2fr; gap: 3rem; max-width: 1280px; margin: 0 auto`. Breakpoints: `≤1024px → 1fr 1fr`; `≤640px → 1fr` (stack).

**Fundo:** `background: var(--color-bg-dark)` (`#1A1A1A`). Sem imagem, sem gradiente. Presença via contraste com o ouro.

**Elementos Restritos:**
- Col 1 (Brand): Logo `h-24 w-auto object-contain` + parágrafo descritivo `font-size: 0.9rem; line-height: 1.7; color: rgba(255,255,255,0.65)` + social links
- Col 2 (Links Rápidos): `.footer-heading` + `.footer-links`
- Col 3 (Contato): `.footer-heading` + `.footer-contact` com SVG icons dourados + links clicáveis
- Col 4 (Atendimento + Mapa): `.footer-heading` + horários + iframe Google Maps `100% × 120px; border-radius: 8px; opacity: 0.85`
- Footer bottom: `flex justify-between align-center flex-wrap` com copyright + créditos `font-size: 0.82rem; color: rgba(255,255,255,0.5)`

**Animação:** `transition: opacity 0.3s ease` no iframe do mapa.

**Micro-interações:**
- Social icons: `hover: background rgba(212,175,55,0.15); border-color: #D4AF37; color: #D4AF37; transform: translateY(-2px)` — 3 propriedades simultâneas em `0.3s ease`
- Links rápidos: `hover: color: #D4AF37; padding-left: 4px` em `0.2s ease` (deslizamento leve)
- Links de contato: `hover: color: #D4AF37` em `0.2s ease`
- Mapa iframe: `hover: opacity: 1` (sai de 0.85 para 1.0 em `0.3s ease`)
- `.footer-heading::after`: `content: ''` com `background: linear-gradient(135deg, #D4AF37, #a68a4a); width: 40px; height: 2px; position: absolute; bottom: -1px; left: 0` — sublinhado dourado degradê em cada heading do footer

**Diferenciador Visual:** O `.footer-heading::after` com `linear-gradient(135deg, #D4AF37, #a68a4a)` em 40px cria um sublinhado dourado de comprimento fixo — diferente do `border-bottom` que se estende pela largura total. Cada heading do footer tem sua própria "assinatura" visual. O prefixo `›` dourado nos links (via `::before` no CSS) adiciona hierarquia sem usar ícones externos.

---

## COMPONENTES REUTILIZÁVEIS

### Botão Primário (CTA Principal)

```css
/* Base */
background-color: #8B1E22;
color: #FFFFFF;
font-family: 'Roboto', sans-serif;
font-weight: 700;
padding: 0.875rem 2rem; /* py-3.5 px-8 */
border-radius: 0.25rem; /* rounded */
box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1), 0 4px 6px -2px rgba(0,0,0,0.05); /* shadow-lg */
transition: background-color 150ms ease, box-shadow 150ms ease;
display: inline-flex;
align-items: center;
gap: 0.5rem;

/* Hover */
background-color: #7f1d1f; /* red-900 Tailwind */

/* Focus */
outline: none;
box-shadow: 0 0 0 2px #FFFFFF, 0 0 0 4px #8B1E22;
```

### Botão Outline (Secundário Hero)

```css
/* Base */
background-color: transparent;
border: 2px solid #FFFFFF;
color: #FFFFFF;
font-family: 'Roboto', sans-serif;
font-weight: 500;
padding: 0.875rem 2rem;
border-radius: 0.25rem;
transition: background-color 150ms ease, color 150ms ease;

/* Hover */
background-color: #FFFFFF;
color: #8B1E22;
```

### Botão Gold (Hero CTA Alternativo)

```css
/* Base */
background-color: #D4AF37;
color: #8B1E22; /* text-primary */
font-weight: 700;
padding: 0.875rem 2rem;
border-radius: 0.25rem;
box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1);
transition: background-color 150ms ease;

/* Hover */
background-color: #EAB308; /* yellow-500 Tailwind */
```

### Card de Especialidade

```css
/* Base */
background-color: #FFFFFF; /* surface-light */
padding: 2rem; /* p-8 */
border-radius: 0.25rem; /* rounded */
box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1), 0 4px 6px -2px rgba(0,0,0,0.05); /* shadow-lg */
border-top: 4px solid #D4AF37; /* ou #8B1E22 em cards alternados */
transition: transform 300ms ease;

/* Hover */
transform: translateY(-8px); /* -translate-y-2 = 0.5rem = 8px */

/* Icon Wrapper — Base */
width: 56px; /* w-14 */
height: 56px; /* h-14 */
background-color: rgba(212, 175, 55, 0.1); /* bg-secondary/10 */
border-radius: 50%;
transition: background-color 300ms ease;

/* Icon Wrapper — Hover (via .group:hover) */
background-color: #D4AF37;

/* Ícone — Hover */
color: #FFFFFF;
```

### Card de Step

```css
/* Base */
background-color: #8B1E22;
border: 1px solid rgba(255, 255, 255, 0.2);
padding: 1.5rem; /* p-6 */
border-radius: 0.5rem; /* rounded-lg */
transition: background-color 300ms ease;

/* Hover */
background-color: rgba(255, 255, 255, 0.1);

/* Número Círculo */
width: 48px;
height: 48px;
background-color: #D4AF37;
color: #8B1E22;
border-radius: 50%;
font-weight: 700;
box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1);
```

### Inputs do Formulário

```css
/* Base */
display: block;
width: 100%;
margin-top: 0.25rem;
border-radius: 0.375rem; /* rounded-md */
border: 1px solid #D1D5DB; /* border-gray-300 */
box-shadow: 0 1px 2px 0 rgba(0,0,0,0.05); /* shadow-sm */
transition: border-color 150ms ease, box-shadow 150ms ease;
padding: 0.5rem 0.75rem;

/* Focus */
border-color: #8B1E22;
box-shadow: 0 0 0 3px rgba(139, 30, 34, 0.2); /* focus:ring focus:ring-primary/20 */
outline: none;

/* Dark Mode */
border-color: #4B5563; /* gray-600 */
background-color: #1A1A1A;
color: #FFFFFF;
```

### Ícones Sociais do Footer

```css
/* Base */
display: flex;
align-items: center;
justify-content: center;
width: 38px;
height: 38px;
border-radius: 50%;
border: 1px solid rgba(212, 175, 55, 0.3);
color: rgba(255, 255, 255, 0.6);
transition: all 0.3s ease;

/* Hover */
background-color: rgba(212, 175, 55, 0.15);
border-color: #D4AF37;
color: #D4AF37;
transform: translateY(-2px);
```

### Botão Flutuante WhatsApp

```css
/* Base */
position: fixed;
bottom: 1.5rem; /* bottom-6 */
right: 1.5rem; /* right-6 */
z-index: 50;
background-color: #25D366;
color: #FFFFFF;
padding: 0.875rem; /* p-3.5 */
border-radius: 50%; /* rounded-full */
box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1), 0 4px 6px -2px rgba(0,0,0,0.05); /* shadow-lg */
transition: transform 150ms ease, background-color 150ms ease;

/* Hover */
background-color: #128C7E;
transform: scale(1.10); /* hover:scale-110 */

/* Badge de Notificação */
position: absolute;
top: -0.25rem;
right: -0.25rem;
background-color: #DC2626; /* red-600 */
color: #FFFFFF;
font-size: 0.75rem;
font-weight: 700;
width: 20px;
height: 20px;
border-radius: 50%;
border: 2px solid #FFFFFF;
animation: bounce 1s infinite; /* animate-bounce */
```

---

## ANTI-PADRÕES REGISTRADOS

❌ **1. Hero com vídeo de fundo ou ilustração vetorial genérica de tribunal/martelo:** A LP usa fotografia real de contexto rodoviário (`hero-bg-rodoviario.png`) + sobreposição de gradiente duplo que incorpora a cor-marca — resultado: imersão temática com identidade, não stock photo jurídico genérico.

❌ **2. Paleta azul-marinho + amarelo canário (combo advocacia clichê):** A identidade usa vermelho profundo (`#8B1E22`) + ouro editorial (`#D4AF37`) — combinação que remete à tradição jurídica clássica sem recorrer ao azul-corporate que 90% dos escritórios copiam.

❌ **3. Seção "Por que nos escolher?" com lista de checkmarks genéricos:** Substituída pela seção "Como Funciona" com 4 steps numerados em bloco monocromático primary — mostra processo, não promessas.

❌ **4. Cards de serviços com ícones de Font Awesome genéricos e descrição de 3 linhas:** Os cards de especialidades usam Material Icons contextuais (transporte, lei, saúde) com animação de grupo (wrapper muda de ouro-transparente para ouro sólido + ícone branqueia) — micro-interação que demonstra qualidade técnica.

❌ **5. Botão "Fale Conosco" fixo em posição central com cor padrão verde WhatsApp visível no primeiro scroll:** O floating button WhatsApp tem badge de notificação `animate-bounce` em vermelho (`bg-red-600`) com borda branca — detalhe que cria urgência visual sem ser apenas um círculo verde comum.

❌ **6. Footer minimalista com copyright e 3 links:** Footer em 4 colunas com CSS Grid nativo, ícones sociais com hover triplo (fundo + borda + cor em `0.3s ease`), mapa Google Maps embutido com `opacity: 0.85` que sobe para `1.0` no hover, headings com sublinhado dourado via `::after` de 40px de largura fixa — nível editorial premium incomum em LPs de escritórios de médio porte.

❌ **7. Accordion FAQ implementado com JavaScript/jQuery:** Uso do elemento HTML semântico nativo `<details>/<summary>` com Tailwind `group-open:rotate-180` para rotação do chevron — zero JS, acessível por padrão, semântico para SEO.

❌ **8. Seção "Sobre" com foto de fachada do escritório e texto corporativo de 2 parágrafos:** A seção incorpora estatísticas em grid 2×2 com `border-l-2 border-secondary pl-4` (numeração com borda dourada), decoração `skew-x-12` absoluta e badge sobrepostos na imagem com coordenadas negativas (`-bottom-6 -left-6`) — design editorial que quebra o grid e cria profundidade.
