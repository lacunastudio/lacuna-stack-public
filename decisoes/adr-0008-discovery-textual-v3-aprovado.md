# ADR-0008 — Discovery textual Lacuna v3 aprovado (manifesto, princípios, posicionamento, tagline, bio)

- **Status:** aceita
- **Data:** 2026-05-08
- **Autor:** Gabriel + Claude (via agente `brand-identity`)
- **Escopo:** matriz
- **Substitui:** [manifesto v2.2](../../matriz/identidade/manifesto.md) · [posicionamento v2.1](../../matriz/identidade/posicionamento.md) · [bio Instagram v2.1](../../matriz/identidade/bio-instagram.md)
- **Relaciona:** [ADR-0007](adr-0007-pivo-identidade-visual-v2-para-v3.md) (pivô v2→v3) · [refs-lacuna-v3.md](../../sistema/inteligencia/pesquisas/refs-lacuna-v3.md) (pesquisa de referências)

## Contexto

Após [ADR-0007](adr-0007-pivo-identidade-visual-v2-para-v3.md) registrar o pivô da identidade Lacuna v2→v3 (escopo: tudo — manifesto, identidade, paleta, voz), foi conduzido **discovery textual** com voz cinematográfica/atmosférica/autoral, baseado nas referências reais alinhadas com o fundador (Anthropic, A24, Lanthimos, Ghibli, Daniels EEAAO, Linear, Notion, Figma, Letterboxd, BAW).

**Direção visual escolhida:** "Cinematic Authorial" — paleta dupla narrativa, tipografia editorial, identidade adaptativa por marca-filha, motion cinematográfico.

**Processo:** agente `brand-identity` foi invocado com brief detalhado contendo (a) ADR-0007, (b) refs do fundador, (c) pesquisa consolidada em `refs-lacuna-v3.md`, (d) material textual atual a ser substituído, (e) restrições explícitas de tom (rejeitar buzzword tech, evitar pretensão vazia, ancorar em refs concretas). Saída foi salva em `matriz/identidade/discovery-v3-rascunho.md` para reação do fundador.

## Decisão

Aprovado o discovery textual v3 conforme rascunho, com os seguintes pontos de implementação:

### 1. Atmosfera em palavras-chave (5)
**deliberada · contemplativa · autoral · atmosférica · precisa**

### 2. Manifesto v3 — 3 variantes mapeadas por canal

- **Variante A (Poética)** → uso: hero do site, vídeo institucional, peças contemplativas
- **Variante B (Contemplativa)** → uso: página /sobre ou /manifesto, decks longos, perfil LinkedIn
- **Variante C (Surreal-direta)** → uso: posts soltos, vídeo curto, abertura de slide, conversa nova

Todas compartilham léxico, ritmo curto-longo, e a tese de fundo (vazio nomeável + tempo + recusa do desperdício + ofício).

### 3. Tagline v3
**"Cada projeto é um plano."** — duplo sentido funcional (trabalho + cinematográfico).

### 4. Princípios públicos v3 (6)
1. O vazio antes do plano
2. Tempo como matéria-prima
3. Cor narrativa, não decoração
4. Plano composto, não página preenchida
5. Discrição como direção
6. Cada obra é um filme

São **diferentes** dos princípios fundadores (10+) em [matriz/principios-empresa.md](../../matriz/principios-empresa.md). Princípios fundadores = internos/operacionais; princípios públicos = voz da marca em comunicação. Coexistem.

### 5. Posicionamento v3
- **Curto** (~25 palavras) para topo de site, slides, e-mail
- **Médio** (~62 palavras) para /sobre, decks, contexto

### 6. Bio Instagram v3
**Versão sintética** (~95 caracteres) com a tagline:
```
A Lacuna constrói marcas, produtos e serviços.
Cada projeto é um plano.

→ Conversar
```
Versão alternativa com filtro anafórico ("sem pressa, sem fórmula, sem ruído.") preservada para uso pragmático se a versão sintética soar distante demais nas primeiras semanas.

### 7. Vocabulário e anti-vocabulário
- **Substantivos de assinatura:** vazio, plano, frame, cena, atmosfera, tempo, silêncio, método, ofício, obra, estúdio
- **Verbos do fazer:** construir, encontrar, nomear, escolher, parar, escutar, olhar, deixar, recusar, apagar, compor
- **Imagens recorrentes:** espaço/lugar não habitado, trabalho parado no meio, geometria do vazio, estúdio↔filme, plano composto vs. página preenchida
- **Vocabulário rejeitado:** tech-genérico (máquina, exponencial, transformamos, delivery, performance, escalar, disruptivo, ecossistema), apelativo de venda (última oportunidade, milagre, secret sauce, transforme seu negócio), AI buzzword (AI-powered, AI-driven), filosofia abstrata vazia (acreditamos em…, nosso DNA é…, nossa missão é mudar o mundo), storytelling heroico (começou na garagem), pedido de empatia (entendemos que…), tropos cinematográficos clichês

## Implementação

Arquivos atualizados/criados nesta sessão:

- [matriz/identidade/manifesto.md](../../matriz/identidade/manifesto.md) — substituído (v2.2 → v3)
- [matriz/identidade/posicionamento.md](../../matriz/identidade/posicionamento.md) — substituído (v2.1 → v3)
- [matriz/identidade/bio-instagram.md](../../matriz/identidade/bio-instagram.md) — substituído (v2.1 → v3)
- [matriz/identidade/principios-publicos.md](../../matriz/identidade/principios-publicos.md) — **criado** (não existia antes)
- [matriz/identidade/discovery-v3-rascunho.md](../../matriz/identidade/discovery-v3-rascunho.md) — preservado como referência histórica do raciocínio

Princípio fundador 19 ("documentação como parte do trabalho, não anexo") cumprido.

## Consequências

**Imediatas:**
- Bio do Instagram `@lacunastd` precisa ser atualizada manualmente pelo fundador (ação fora do hub).
- Site v2 (em [matriz/engenharia/lacuna-site/](../../matriz/engenharia/lacuna-site/)) já estava arquivado pelo ADR-0007. Implementação visual v3 começa do zero quando paleta+tipografia forem definidas.
- LinkedIn perfil pode ser atualizado quando fundador quiser (manual).

**Em paralelo (próxima sessão):**
- Mockup visual com 3 paletas saturadas (vermelho-vinho / verde-abeto / âmbar-cobre) usando texto v3 já como base — fundador escolhe paleta.
- Após paleta escolhida: refinar par tipográfico (free com upgrade path para premium), motion patterns, sistema de identidade adaptativa por marca-filha.

**Pendentes a decidir após mockup visual:**
- Identidade adaptativa: cada marca-filha herda estrutura mas varia tom? Ou marcas-filhas são totalmente livres? (Decisão adiada — princípio público 6 sustenta o caminho adaptativo, mas execução precisa de mockup primeiro.)
- Tradução EN das peças textuais — só após v3 estabilizar em PT-BR com público.

**Não tocados nesta aprovação:**
- [matriz/principios-empresa.md](../../matriz/principios-empresa.md) — 10+ princípios fundadores intactos (são internos/operacionais).
- Estrutura do hub, sistema de lentes, skills, agentes, hooks, Marca #1 — todos intactos.
- ADRs históricos — todos intactos.

## Aprendizado registrado

- Princípio 21 (referências reais antes de propor) aplicado **com sucesso** desta vez. Refs alinhadas com fundador antes de qualquer proposta textual; agente `brand-identity` ancorou cada escolha em ref concreta.
- Memória [feedback_visual_reference_alignment](~/.claude/projects/.../memory/feedback_visual_reference_alignment.md) sustentou a decisão de não pular passos.
- **Próxima validação:** teste de aderência após mockup visual ("se cobrirmos nome Lacuna e nome A24/Lanthimos → mesma família visual?"). Se sim, segue. Se não, ajusta antes de implementar.
