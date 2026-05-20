# ADR-0011 — Direção visual Lacuna v3 aprovada: γ.5 (Sálvia) + mark Fenda 02.A

- **Status:** aceita
- **Data:** 2026-05-12
- **Autor:** Gabriel + Claude
- **Escopo:** matriz
- **Relaciona:** [ADR-0007](adr-0007-pivo-identidade-visual-v2-para-v3.md) (pivô v2→v3, visual) · [ADR-0008](adr-0008-discovery-textual-v3-aprovado.md) (discovery textual v3) · [matriz/identidade/visual-discovery/README.md](../../matriz/identidade/visual-discovery/README.md) (re-discovery r2)
- **Substitui:** direção visual "Cinematic Authorial" (ADR-0008) e versão v2 modo claro + verde-musgo (ADR-0004) — ambas passam a ser histórico

## Contexto

A Lacuna acumulou **6 rejeições visuais consecutivas** entre site v2 (2026-05-08) e SVGs codados (2026-05-11), documentadas em [visual-discovery/README.md](../../matriz/identidade/visual-discovery/README.md). Cada rejeição tinha o mesmo padrão de erro do agente: minimalismo Bauhaus flat quando a direção declarada pelo fundador era execução premium com motion + depth + microinterações (estilo Framer Templates premium / heymessage / fabrica).

Em 2026-05-11, fundador descontinuou o wordmark `lac___na` (com underscores) preservando "Lacuna" como nome puro. Abriu re-discovery visual round 2 (princípio 21 inegociável: refs reais antes de proposta).

Em 2026-05-12 esta sessão produziu:
1. **12 refs reais** colocadas pelo fundador (todos templates Framer premium) — base pra decomposição estrutural
2. **5 inspeções ao vivo via chrome-devtools** (heymessage / fabrica / perform / essentia / agevia) extraindo tipografia, paleta, motion lib, padrões transversais
3. **Análise estrutural cruzada** com atmosfera Lacuna textual (ADR-0008): "deliberada · contemplativa · autoral · atmosférica · precisa"
4. **3 propostas de paleta** do fundador (Martinique+Zombie / Red+Wine / Flame+Finn) com hex WCAG verificados
5. **Iterações:** α (Cinematic Atmospheric) → β (Editorial Saturated) → γ (Atmospheric Light) → δ (mix α+γ) → γ.1..γ.4 (variantes) → γ.5 (final: γ.4+γ.1)
6. **Mark exploration:** 5 conceitos (Intervalo / Fenda / Inicial / Colchete / Respiração) → 3 refinamentos da Fenda → **02.A escolhido** com entusiasmo

## Decisão

Aprovada a direção visual Lacuna v3 final, composta por:

### 1. Modo light dominante — "Sálvia"

Verde-acinzentado off-white como fundo dominante, inspirado em [essentia.framer.media](https://essentia.framer.media/) (template Framer premium decomposto via chrome-devtools nesta sessão).

| Token | HEX | HSL | Função |
|---|---|---|---|
| `--color-bg` | `#D4DCCF` | hsl(95, 14%, 84%) | Sálvia clara — fundo dominante |
| `--color-bg-deep` | `#C8D0C2` | hsl(93, 12%, 79%) | Sálvia clara escurecida — gradient/layer |
| `--color-fg` | `#3A3D38` | hsl(96, 4%, 23%) | Sálvia profunda — texto principal |
| `--color-accent` | `#3A2E5A` | hsl(258, 32%, 27%) | Martinique — acento (palavra-chave, link, ícone) |

WCAG AAA: contraste `--color-fg` sobre `--color-bg` = 8.5:1 (passa AAA para texto pequeno).

Detalhe em [matriz/identidade/paleta.md](../../matriz/identidade/paleta.md).

### 2. Sistema tipográfico — Host Grotesk + Inter + JetBrains Mono

| Família | Função | Peso |
|---|---|---|
| **Host Grotesk** (Google Fonts, free) | Display + UI (wordmark, h1-h4, CTAs) | 300-500 |
| **Inter** (Google Fonts, free) | Body | 300-500 |
| **JetBrains Mono** (Google Fonts, free) | Labels técnicas, metadata, eyebrow caps | 400 |

Tracking display: -3 a -5.6px (variável conforme escala). Host Grotesk weight 400-500 (não bold heavy) — humanista, atmosférica, ressoa com heymessage e atmosfera contemplativa.

Detalhe em [matriz/identidade/tipografia.md](../../matriz/identidade/tipografia.md).

### 3. Wordmark + Mark

- **Wordmark:** "Lacuna" em **Host Grotesk weight 500** (header) ou **weight 400** (display massive), tracking -0.6 a -5.4px conforme escala.
- **Mark:** **Fenda 02.A** — círculo sólido com fenda diagonal sutil (ângulo 12°, largura 12% da viewport, centralizada).
  - Carrega vocabulário-âncora da Lacuna ("fenda", "vazio", "abertura", "corte")
  - Gesto cinematográfico (alusão a corte de filme / abertura de luz)
  - Funciona em escalas 16px (favicon) a 1080px (foto de perfil) — validado nesta sessão
  - Funciona em contextos light/dark/accent/neutro — validado

**Wordmark textural** (assinatura visual em peças grandes): "Lacuna" em Host Grotesk weight 500, ~460px, opacity 6%, posicionado no canto inferior direito do canvas saindo pra fora (eco editorial fabrica + essentia).

Detalhe em [matriz/identidade/mark.md](../../matriz/identidade/mark.md).

### 4. Diagramação base

- **Hero:** eyebrow mono caps + h1 massive (~128px) + sub Inter + CTA pill primário + CTA link secundário + footer mono
- **Wordmark textural** posicionado ao fundo, canto inferior direito
- **Composição assimétrica** esquerda-pesada (texto à esquerda, wordmark à direita)
- **Whitespace generoso** — atmosfera respiratória

Preview de referência: [matriz/identidade/visual-discovery/previews/preview-gamma-5-mix-host-grotesk-wordmark-direita.html](../../matriz/identidade/visual-discovery/previews/preview-gamma-5-mix-host-grotesk-wordmark-direita.html).

### 5. Motion (a desenhar em sessão dedicada — Onda II)

**Lib confirmada:** Framer Motion (validada como universal nas 5 refs top-tier inspecionadas).

**Princípios:**
- Scroll-driven reveal das linhas tipográficas
- Hover states sutis nos CTAs (translateX em seta, fade no background)
- Wordmark textural pode ter parallax leve
- Gradient atmosférico pode pulsar lentamente

Specs concretas (easing curves, durations, scroll-triggers) ficam para sessão dedicada — Onda II do roadmap visual.

### 6. Sem fotografia inicial

Direção começa **sem fotografia atmosférica própria** (decisão consciente do fundador, 2026-05-12). Atmosfera vem de:
- Tipografia massive Host Grotesk
- Gradient atmosférico de fundo (radial light)
- Wordmark textural como elemento de composição

Fotografia atmosférica fica como **evolução possível** (Onda III) quando justificar custo de produção/curadoria.

## Consequências

### Positivas

- **Coerência interna alta:** atmosfera textual ADR-0008 (deliberada/contemplativa/autoral/atmosférica/precisa) + atmosfera visual γ.5 (sálvia + Host Grotesk + Fenda) bate 1:1
- **Custo zero:** Host Grotesk + Inter + JetBrains Mono são free no Google Fonts. Sem custo de tipografia. Sem fotografia obrigatória.
- **Escalabilidade:** mark Fenda funciona em 16px (favicon) a 1080px (profile pic). Identidade pronta pra múltiplos canais.
- **Vocabulário visual alinhado com Framer Templates premium** — bate com o "nível de execução" que o fundador admira (heymessage / fabrica / essentia validados via chrome-devtools nesta sessão)
- **Differenciação:** modo light verde-acinzentado é raro no espaço de studios criativos digitais (mais comuns: dark, off-white neutro). Diferenciador autoral.

### Negativas / tradeoffs aceitos

- **Modo light contradiz preferência inicial declarada** (fundador disse "dark dominante" antes; após ver γ light, escolheu light com clareza). Tradeoff: light fica menos "cinematic noturno" mas mais "studio editorial contemplativo" — alinhamento com refs essentia mais próximo.
- **Sem fotografia inicial:** identidade depende muito de tipografia + composição. Risco de parecer "tipográfica demais" pode aparecer; mitigação via wordmark textural + gradient + microelementos editoriais.
- **Direção "Cinematic Authorial" do ADR-0008 é parcialmente preservada (atmosfera, voz) mas parcialmente substituída (paleta dupla narrativa → sálvia única, serif editorial → grotesque humanista).** Textos do ADR-0008 permanecem válidos com pequeno reset de metadata (remover `lac___na`, atualizar referência à direção visual).
- **Host Grotesk é fonte relativamente nova** (Source Foundry, ~2023). Risco de "fontes em alta hoje, esquecidas amanhã". Mitigação: variable font open source — não trava upgrade futuro.

### Operacionais (executadas nesta sessão)

- Criar [matriz/identidade/paleta.md](../../matriz/identidade/paleta.md)
- Criar [matriz/identidade/tipografia.md](../../matriz/identidade/tipografia.md)
- Criar [matriz/identidade/mark.md](../../matriz/identidade/mark.md)
- Reescrever [matriz/identidade/design-system.md](../../matriz/identidade/design-system.md) (v2 modo claro + verde-musgo → v3 γ.5 Sálvia)
- Arquivar em [matriz/identidade/arquivo/](../../matriz/identidade/arquivo/): discovery-v3-rascunho, discovery-logo-v3 (5 conceitos pré-Fenda), site-v2-*, mockups v3 paleta a/b/c (rejeitados), 11 SVGs code-generated (rejeitados)
- Reset de metadata em [manifesto.md](../../matriz/identidade/manifesto.md) / [posicionamento.md](../../matriz/identidade/posicionamento.md) / [bio-instagram.md](../../matriz/identidade/bio-instagram.md): remover `lac___na`, atualizar referência à direção visual
- [DECISIONS-LOG.md](../../DECISIONS-LOG.md) + [STATE.md](../../STATE.md) + [BACKLOG.md](../../BACKLOG.md) + [docs/HUB-CHANGELOG.md](../../docs/HUB-CHANGELOG.md) + [docs/SESSION-LOG.md](../../docs/SESSION-LOG.md) atualizados

## O que NÃO muda

- **Toda a copy aprovada em ADR-0008 permanece válida.** Manifesto (3 variantes A/B/C), tagline ("Cada projeto é um plano."), posicionamento (curto + médio), bio Instagram, 6 princípios públicos, vocabulário+anti-vocabulário, frases-DNA invioláveis. Apenas pequeno reset de metadata (remover `lac___na` e atualizar referência visual).
- **Atmosfera 5 palavras-chave** (deliberada · contemplativa · autoral · atmosférica · precisa) permanece como ancoragem.
- **Princípio fundador 10** (discrição sobre stack/IA em comunicação pública) permanece — releitura quando Lacuna Hub virar público algum dia.
- **Estrutura macro do Hub** (matriz / sistema / marcas / clientes / decisoes / docs / .claude) — intacta.
- **Marca #1, ADRs históricos, agentes, skills, regras** — todos preservados.

## Pontos em aberto pra futuras sessões

- **Onda II — Sistema completo:** motion patterns (easing, duration, scroll triggers), estados (hover/focus/active), componentes base (button, link, eyebrow, footer, card), variantes (citações, listas, cards de portfólio)
- **Onda III — Aplicação:** 2ª seção do site (manifesto/portfólio/contato), versão mobile (375px — princípio 16), aplicação em peças (card cliente, post IG, slide deck, e-mail template)
- **Identidade adaptativa por marca-filha:** princípio público 6 ("cada obra é um filme") sugere variação de atmosfera por marca. Mark Lacuna fica como assinatura constante; cada marca-filha pode ter paleta/tipografia tonal própria dentro do sistema base. A definir quando 2ª marca surgir.
- **Fotografia atmosférica:** quando justificar custo, explorar fotografia autoral (não stock) que adicione camada cinematográfica.
- **Tradução EN dos copys:** quando Lacuna for atuar em mercado EN.

## Referências

- [matriz/identidade/visual-discovery/](../../matriz/identidade/visual-discovery/) — pasta completa de re-discovery r2 (refs, previews, marks-exploration, refinement)
- [matriz/identidade/visual-discovery/refs-links.md](../../matriz/identidade/visual-discovery/refs-links.md) — 12 sites Framer + 2 galerias Behance + 1 anti-ref
- [matriz/identidade/visual-discovery/previews/preview-gamma-5-mix-host-grotesk-wordmark-direita.html](../../matriz/identidade/visual-discovery/previews/preview-gamma-5-mix-host-grotesk-wordmark-direita.html) — preview de referência da diagramação aprovada
- [matriz/identidade/visual-discovery/previews/preview-mark-fenda-refinement.html](../../matriz/identidade/visual-discovery/previews/preview-mark-fenda-refinement.html) — refinamento + validação do mark Fenda 02.A
- [ADR-0008](adr-0008-discovery-textual-v3-aprovado.md) — discovery textual v3 (atmosfera + voz)
- [ADR-0007](adr-0007-pivo-identidade-visual-v2-para-v3.md) — pivô v2→v3
- [ADR-0004](adr-0004-paleta-modo-claro-verde-musgo.md) — paleta modo claro v2 (substituída)
- Princípio 21 CLAUDE.md — refs reais antes de proposta visual (aplicado de verdade nesta rodada)
- Princípio 15 CLAUDE.md — design execution baseline (8pt grid, design tokens, 1 detalhe autoral)
- 5 inspeções chrome-devtools desta sessão: heymessage, fabrica, perform, essentia, agevia
