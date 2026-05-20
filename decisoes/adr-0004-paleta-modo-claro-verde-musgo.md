# ADR-0004 — Paleta modo claro, acento verde-musgo `#3D5240`

- **Status:** aceita
- **Data:** 2026-05-08
- **Autor:** Gabriel + Claude
- **Escopo:** matriz

## Contexto

Identidade visual da Lacuna v1 era modo escuro (`#0a0a0a` base + branco texto + roxo `#7B68EE` acento). Decisão de fundador para o site v2: **modo claro**, com **cor de acento repensada do zero** (não ficar preso ao roxo).

Princípio 21 aplicado: 6 referências de paletas modo-claro institucionais foram pesquisadas antes da decisão (Basecamp, Stripe, Vercel, Linear, ohnotype, Once.com). Síntese identificou que azul-roxo é hegemônico em tech (`#0070F3` Vercel, `#475BA1` Linear, `#635BFF` Stripe) — exatamente o que o fundador quer evitar.

Cores de acento alternativas pesquisadas como saída do template:
- Dourado/amarelo-mel (Basecamp `#FFD60A`)
- Vermelho-tijolo (Once Campfire)
- **Verde-musgo (Once Writebook, Patagonia)**
- Âmbar/ocre (tendência 2026)
- Azul-tinta dessaturado (`#2C3E50`)

## Alternativas consideradas

### A — Âmbar/mostarda escura `#B8860B`
- Calor terroso, evita roxo. Risco WCAG em texto pequeno.

### B — Vermelho-ocaso fechado `#A33523`
- Ofício manuscrito, anti-digital-frio. Carrega carga emocional alta — exige economia rigorosa.

### C — Verde-musgo profundo `#3D5240` ← **escolhida**
- Longevidade, paciência. WCAG AAA. Raríssima em portfolios digitais. Referências: Patagonia, Once Writebook.

### D — Azul-tinta dessaturado `#2C3E50`
- Linear-style mas mais escuro. Risco: vizinho do território Stripe/Linear, diferenciação depende de tipografia.

### E — Acento-zero (preto sobre branco)
- Vercel-style. Trivial WCAG. Risco: pode parecer "sem identidade" sem outro gesto autoral.

## Decisão

**Paleta modo claro:**
- Fundo principal: `#FFFFFF`
- Fundo secundário: `#FAFAFA`
- Texto principal: `#0A0A0A` (não preto puro)
- Texto secundário: `#5B6770`
- **Acento principal: `#3D5240` (verde-musgo profundo)**
- Acento hover: `#2F4A3A`
- Borda: `#E5E5E5`

## Consequências

### O que fica mais fácil
- Coerência semântica com manifesto: verde-musgo carrega "tempo, paciência, ofício" — atributos centrais da tese Lacuna
- Diferenciação visual no espaço tech (95% dos competidores usam azul/roxo)
- Acessibilidade WCAG AAA garantida (~9:1 sobre branco)
- Tipografia (IBM Plex Mono + Inter) ainda protagonista — verde economiza, não domina

### O que fica mais difícil
- Quebra com identidade visual da Lacuna v1 (modo escuro + roxo) — pessoas que conheciam a versão antiga vão notar mudança
- Verde pode lê-se "outdoor/sustentabilidade/ESG" se não houver gesto técnico contrário (mitigado pela tipografia mono + estrutura site)
- Aplicação requer disciplina (1-2% da página) — fácil de exagerar e quebrar a tese "sem ruído"

### O que precisa ser revisado se isso mudar
- Se uso real revelar que o verde está sendo lido errado (pesquisa em wellness/lifestyle), criar nova ADR
- Se necessário expandir paleta com cor secundária (atualmente sem segundo acento), criar ADR

## Referências

- [matriz/identidade/design-system.md](../../matriz/identidade/design-system.md) — paleta aplicada
- [matriz/identidade/site-v2-esqueleto.md](../../matriz/identidade/site-v2-esqueleto.md) — onde paleta vai ser aplicada
- [sistema/inteligencia/learning-log.md](../../sistema/inteligencia/learning-log.md) — entrada "Pesquisa paletas modo claro 2026-05-08"
