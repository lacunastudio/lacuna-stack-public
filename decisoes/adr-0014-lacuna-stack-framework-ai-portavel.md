# ADR-0014 — Lacuna Stack como framework AI-portável otimizado pra Claude

- **Status:** aceita
- **Data:** 2026-05-19
- **Autor:** Gabriel + Claude
- **Escopo:** matriz + Marca #02 (Lacuna Studio como produto público)
- **Relaciona:**
  - [ADR-0009](adr-0009-lacuna-hibrida-hub-builder-operacional.md) — modelo híbrido
  - [ADR-0010](adr-0010-lacuna-hub-formalizado.md) — Hub formalizado (princípio 27 sobre continuidade cross-IA já preparou essa direção)
  - [ADR-0013](adr-0013-lacuna-studio-absorve-tese-loom-revertida.md) — Lacuna Studio absorve tese de framework + comunidade

## Contexto

Sessão de envelope de serviços (2026-05-19) trouxe observação crítica do fundador: "quem adquirir vai poder usar esse framework em qualquer IA de sua preferência (pelo menos as principais do mercado) — o importante é ter a capacidade de seguir documentações e .mds (claro, tudo otimizado e criado para claude-made)".

Essa observação não é detalhe — é decisão estratégica que muda posicionamento, TAM, diferenciação competitiva e implementação técnica do Lacuna Stack (info-produto principal).

**Antes desta ADR (assumido implícito):**
- Lacuna Stack = framework Claude Code-native
- TAM: usuários Claude Code
- Diferenciação: "estrutura completa pra Claude Code"
- Risco: dependente da Anthropic (mudanças de política, preço, modelo)

**Após esta ADR (decisão consciente):**
- Lacuna Stack = **framework AI-portável** otimizado pra Claude
- TAM: qualquer dev/founder usando IA principal capaz de ler documentação estruturada
- Diferenciação: **"use com a IA que você prefere"** — vantagem competitiva real vs concorrentes que prendem a uma ferramenta
- Risco: reduzido — framework sobrevive mudanças de IA

## Decisão

**Lacuna Stack é framework AI-PORTÁVEL.** Funciona com qualquer IA principal capaz de ler documentação estruturada (.md). **Otimizado pra Claude** — implementação de referência mais completa — mas usável em ChatGPT, Cursor, Windsurf, Gemini Code Assist e qualquer outra IA principal.

### O que isso significa concretamente

**Core do Lacuna Stack = markdown puro:**

| Componente | Formato | Portabilidade |
|---|---|---|
| 28 princípios fundadores | Markdown puro | ✅ Universal |
| 8 regras escopadas | Markdown puro com "carregar quando" instruções | ✅ Universal |
| Templates (ADR, STATE, PROJECT, CONTEXT) | Markdown puro | ✅ Universal |
| Estrutura de pastas | Convenção universal | ✅ Universal |
| Metodologia fases F0-F4 | Markdown puro | ✅ Universal |
| Distribuição financeira 35/50/15 | Markdown puro | ✅ Universal |

**Implementação otimizada Claude Code (inclusa como referência):**

| Componente | Formato | Portabilidade |
|---|---|---|
| 14 skills (slash-commands) | `.claude/skills/` | 🟡 Implementação de referência; portável via prompts equivalentes em outras IAs |
| 9+ agents | `.claude/agents/` | 🟡 Mesmo — portável via system prompts adaptados |
| 3 hooks (Stop, SessionStart, PostToolUse) | `.claude/hooks/` PowerShell | 🔴 Claude Code-only — opcional/extra |

**Implicação técnica:**
- Quem usa **Claude Code** recebe o pacote completo (markdown + skills + agents + hooks)
- Quem usa **ChatGPT/Cursor/Windsurf/Gemini** recebe markdown puro + templates de prompts equivalentes às skills/agents
- Mesma base, "execução otimizada" varia por IA

## Razões

1. **TAM aumenta drasticamente** — todo dev AI-builder vs só usuários Claude Code. Mercado BR cresce de ~10-20k pra ~100-300k.
2. **Diferenciação competitiva real** — vs Notion templates (prendem a Notion), Cursor templates (prendem a Cursor), Custom GPTs (prendem a OpenAI), workflows Claude-only.
3. **Princípio fundador #10 vivo** — "ferramenta serve ao trabalho, não amarra". Esse princípio já existia interno; agora vira posicionamento de marca.
4. **Risco reduzido** — se Anthropic mudar política, preço, modelo ou política de uso, framework Lacuna sobrevive.
5. **Marca Lacuna não depende de Anthropic** — independência estratégica.
6. **Coerência com princípio 27** — continuidade cross-IA (HUB-ENTRY + .claude/onboarding/) já estava preparada pra essa direção desde ADR-0010.

## Consequências

### Imediatas (executadas nesta sessão)

- Cardápio de serviços ([cardapio.md](../../matriz/operacao/servicos/cardapio.md)) reflete portabilidade nos Serviços C e D
- About page Lacuna Studio ([about-publico.md](../../matriz/identidade/about-publico.md)) ganha menção à portabilidade
- Variante D do manifesto ([manifesto.md](../../matriz/identidade/manifesto.md)) ganha linha sobre portabilidade
- **Princípio público novo #8** ([principios-publicos.md](../../matriz/identidade/principios-publicos.md)): "Ferramenta serve ao trabalho, não amarra"
- One-pager de serviços ([one-pager.md](../../matriz/operacao/servicos/one-pager.md)) menciona "qualquer IA principal"
- Bios cross-redes ([bio-instagram.md](../../matriz/identidade/bio-instagram.md)) preservam tom sem mencionar IA específica (já compatível)
- Regra de tendências ([conteudo-publico-tendencia.md](../../.claude/rules/conteudo-publico-tendencia.md)) amplia scan pra comunidades multi-IA

### Médio prazo (próxima sessão)

- Mockup do Lacuna Stack (info-produto) refletindo portabilidade desde o desenho
- Documentação do Stack em markdown puro como core
- Templates Claude Code como "extras opcionais"
- Versão pra Cursor, Windsurf, ChatGPT — adaptações de prompt equivalentes às skills

### Risco principal a vigiar

**O framework precisa SER LITERALMENTE portável.** Se na prática só funciona bem com Claude Code, esse posicionamento vira marketing falso e quebra confiança. Validação obrigatória antes de lançar: testar Stack em ChatGPT Projects + Cursor + Windsurf + Gemini Code Assist. Se quebrar significativamente em alguma, ajustar core OU recalibrar promessa pra "otimizado pra Claude e Cursor" (subset).

### Validação técnica obrigatória antes do lançamento

Checklist:
- [ ] Princípios funcionam como system prompt em ChatGPT Projects
- [ ] Regras escopadas adaptáveis pra Cursor `.cursorrules`
- [ ] Templates ADR/STATE/PROJECT lidos por qualquer IA
- [ ] Estrutura de pastas reconhecida por qualquer IA
- [ ] Pelo menos 3 IAs principais testadas com framework completo
- [ ] Documentação com "como usar com [IA X]" pra 3-5 IAs principais

Se algum item quebrar significativamente: revisar core OU ajustar promessa pública.

## Aprendizado meta

Essa ADR nasceu de **observação durante envelope de serviços**, não de discussão dedicada de produto. Sinal de que decisões estratégicas grandes podem emergir em momentos laterais — vale escutar cada observação do fundador com peso, mesmo quando aparece em contexto adjacente.

**A registrar no learning-log:** posicionamento competitivo (lock-in vs portabilidade) é decisão arquitetural fundadora — afeta TAM, diferenciação, risco. Vale revisitar quando produtos similares aparecerem no mercado.

---

**Ato fundador desta decisão:** observação direta do fundador 2026-05-19, sem hesitação, com clareza sobre vantagem competitiva e proteção contra dependência de uma única IA. Sem teimosia em formato Claude-only por inércia.
