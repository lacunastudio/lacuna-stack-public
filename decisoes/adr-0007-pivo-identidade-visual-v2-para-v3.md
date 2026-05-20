# ADR-0007 — Pivô da identidade visual Lacuna v2 → v3 (premium-tech motion-saturado)

- **Status:** aceita (decisão de virada; novo discovery de identidade abre)
- **Data:** 2026-05-08
- **Autor:** Gabriel + Claude
- **Escopo:** matriz
- **Substitui:** ADR-0004 (paleta verde-musgo) — em revisão
- **Relaciona:** princípio 21 (referências reais antes de propor) + memória `feedback_visual_reference_alignment`

## Contexto

Após implementação técnica do site v2 em Next.js 16 ([matriz/engenharia/lacuna-site/](../../matriz/engenharia/lacuna-site/)) — código que portou o HTML preview v1.0 "validado" para componentes React com paleta v2.3, IBM Plex Mono + Inter, IntersectionObserver fade-in e wordmark loading — o fundador acessou localhost:3000 e reportou desalinhamento profundo com o que imaginava:

> "tá completamente distante de qualquer coisa que eu estava imaginando. completamente simples e cru. Os exemplos [Naval, levels.io, Patagonia, Once Writebook] que você me deu são muito legais, mas o que vc fez não tem absolutamente nada a ver com nenhum deles. Eles tem cores, imagens, efeitos, uma infinidade de coisas. O nosso só tem preto e branco e nada, zero efeitos desktop, zero tudo."

Análise honesta confirmou a divergência:

| Referência citada no spec | O que ela tem | O que entregamos tem |
|---|---|---|
| nav.al (Naval) | Podcast embedado, links coloridos, feed denso, lista de essays clicáveis | Texto institucional estático |
| levels.io | Laranja vibrante, foto, números públicos ($ARR), screenshots, mapa | Off-white + verde-musgo pontual + zero foto |
| Patagonia institucional | Fotografia majestosa outdoor, vídeo, ativismo visual rico | Zero imagem |
| Once Writebook | Verde + branco vibrante, screenshots, gradientes, microanimações | Fade-in 250ms + IBM Plex Mono |

O resultado se aproxima muito mais de **Robin Sloan / Maciej Cegłowski / Mark Hurst** (portfólios super-minimalistas radicais) do que das referências citadas. As referências viraram **decoração argumentativa** — justificaram a decisão sem guiá-la.

## Direção declarada pelo fundador

**"Tipo Linear/The Browser Company — motion + paleta saturada"** + escopo da virada: **"tudo — manifesto, identidade, paleta, voz"**.

Não é refino do v2 — é **discovery novo de identidade Lacuna v3**.

## Decisão

1. **Lacuna v2 (atual) é arquivada como referência histórica.** Não vai a produção. Código em [matriz/engenharia/lacuna-site/](../../matriz/engenharia/lacuna-site/) preservado como "versão A — spec validado em mockup que não bateu na implementação real". Útil como aprendizado, não como base.

2. **Lacuna v3 é discovery de identidade do zero**, com:
   - Referências reais alinhadas ANTES de qualquer mockup (princípio 21 aplicado de verdade desta vez)
   - Direção: motion sofisticado + paleta saturada + "premium-tech com personalidade" (Linear / The Browser Company / Vercel / Stripe / Cosmos como universo de inspiração inicial — a confirmar com fundador)
   - Manifesto + voz + tom textual revistos junto (não preservados separadamente — visual e voz andam juntos)
   - Paleta inicial verde-musgo `#3D5240` (ADR-0004) **em revisão** — pode ser preservada como acento secundário, substituída, ou complementada com cor saturada vibrante
   - Tipografia em revisão — IBM Plex Mono pode permanecer para títulos como gesto técnico, mas tipografia de display talvez precise de algo com mais expressão

3. **Próxima sessão de identidade abre limpa** com:
   - `/sync` antes (princípio 22 — isolamento por conversa)
   - `/voltei` após `/pausa` (princípio 23 — fundador captura referências reais offline antes)
   - Discovery de identidade conduzido pelo agente `brand-identity` com agente `design-ux` em paralelo
   - **Sem** propor visual sem 5+ referências concretas alinhadas com fundador

4. **Não tocar o ativo já consolidado:**
   - Estrutura do hub (matriz/sistema/marcas)
   - Princípios da Matriz textuais (24 princípios em CLAUDE.md)
   - Sistema de lentes para iniciar projetos
   - Skills, agentes, hooks, workflows
   - Marca #1 (rh-humano) discovery
   - **Sistema de versionamento + ADRs**

   O pivô é **só de identidade da Lacuna** (visual + voz + manifesto).

## Aprendizado registrado

Memória `feedback_visual_reference_alignment.md` persistida. **Teste de aderência** virou regra: antes de avançar de mockup para implementação, perguntar — "se cobrirmos o nome 'Lacuna' e o logo da [referência citada], um observador externo identifica que pertencem à mesma família visual?" Se não, ou as refs estão erradas, ou a execução desviou.

## Consequências

- **Trabalho preservado:** copy v1.4 PT/EN, design-system v2.3, manifesto v2.2, princípios 01-06, mockups, HTML preview, código Next.js — tudo arquivado, recuperável.
- **Trabalho descartado como "produto":** nada vai pra produção como está. Tudo é insumo de aprendizado para o v3.
- **Impacto em outras frentes:** zero. Marca #1 segue independente. Hub segue. Skills/agentes seguem.
- **Próximo passo:** discovery de identidade Lacuna v3 (sessão dedicada, abrir após `/pausa` + `/voltei`).
