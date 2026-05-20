# ADR-0003 (Matriz) — Thumbnails do YouTube em sistema visual coerente com identidade Lacuna, não convenção de mercado

- **Status:** aceita
- **Data:** 2026-05-08
- **Autor:** Gabriel + Claude (com pesquisa de mercado fundamentada)
- **Escopo:** matriz

## Contexto

A convenção dominante de thumbnails do YouTube em 2026 é **face expressiva + seta vermelha + círculo + texto grande em amarelo/vermelho**. Pesquisas (bfind 2026; Outlierkit 2026) mostram que essa convenção **vence em testes médios** — CTR 4-6% é "bom"; <2% sinaliza problema.

Porém:
- Nichos B2B/business toleram (e às vezes preferem) thumbs **mais minimalistas e tipográficas**
- **Coerência visual entre thumbs do canal** (mesma família tipográfica, mesma paleta) cria **reconhecimento de canal** — sinal forte de Browse personalizado por cluster de watch history (Outlierkit 2026)
- A Lacuna tem **identidade visual já definida** (preto/branco/roxo `#7B68EE`, IBM Plex Mono + Inter, lac___na com underscores)
- Princípio 11 da Matriz: **evitar cara de AI-made/page builder** — convenção face+seta+círculo é o padrão "AI-made" perfeito para o algoritmo recém-purgado em jan/2026

Pesquisa fundamentada em [learning-log entrada 2026-05-08 YouTube](../../sistema/inteligencia/learning-log.md).

A pergunta era: **otimizar thumb por CTR individual de cada vídeo (convenção de mercado) ou por coerência de canal (sistema visual Lacuna)?**

## Alternativas consideradas

1. **Convenção de mercado (face+seta+círculo+vermelho/amarelo)**
   - Prós: CTR potencialmente 0,5-1% maior em testes médios; "fórmula testada"
   - Contras: contradiz princípio 11; faz canal parecer genérico; Browse personalizado em 2026 favorece reconhecimento de marca; cada thumb seria isolada, sem ativo de canal
2. **Thumbs em sistema visual coerente com identidade Lacuna** ← **escolhida**
   - Prós: alinha com princípio 11; Browse personalizado favorece reconhecimento de canal; ativo de marca de longo prazo; coerência com IG/site/identidade institucional; cada thumb fortalece a Lacuna como marca, não só o vídeo individual
   - Contras: pode custar 0,5-1% de CTR vs convenção; exige disciplina de design system; mais trabalho inicial para definir templates
3. **Sem sistema, cada thumb decidida no momento**
   - Prós: máxima flexibilidade
   - Contras: caos visual; canal parece amador; Browse personalizado pune

## Decisão

**Thumbnails do YouTube seguem sistema visual coerente com identidade Lacuna**, mesmo que isso custe 0,5-1% de CTR vs convenção de mercado.

**Sistema visual mínimo (a refinar com `brand-identity` agente quando produzir as primeiras 3 thumbs):**

- **Paleta:** preto, branco, roxo `#7B68EE` — mesmas cores da identidade institucional
- **Tipografia:** **IBM Plex Mono** para texto principal (mantém DNA tipográfico Lacuna); **Inter** para apoio se necessário
- **Texto na thumb:** 3-5 palavras MAX, legível em mobile
- **Composição:** preferir tipografia + 1 elemento gráfico autoral (símbolo, geometria, foto tratada). **Não** padrão face+seta+círculo
- **Coerência:** todas as thumbs do canal devem ser reconhecíveis como mesmo canal **mesmo sem o nome aparecer**
- **Detalhe autoral:** 1 elemento intencional por thumb (alinhamento atípico, espaço negativo, microtipografia) — princípio 15 (design execution baseline) e 18 (auto-suficiência por pasta)

**A/B testing nativo (Test & Compare):** quando elegível (Advanced Features ativadas), usar **dentro do sistema visual** para refinar variações — testar diferentes ângulos de tipografia/composição, **não** sair do sistema para testar convenção de mercado.

## Consequências

**O que vira mais fácil:**
- Decisão de design rápida (sistema definido, não reinventar a cada thumb)
- Reconhecimento de canal pelo Browse personalizado
- Coerência institucional Lacuna (canal = extensão da marca, não silo)
- Defender contra "fazer feio para ganhar CTR" — temos princípio escrito

**O que vira mais difícil:**
- Resistir à pressão psicológica quando algum vídeo do nicho viralizar com convenção de mercado
- Manter qualidade tipográfica em todas as thumbs (não cair em texto preguiçoso)
- Aceitar que CTR pode ser 0,5-1% menor em testes individuais

**O que precisa ser revisado se isso mudar:**
- Se CTR sustentado for <2% por mais de 10 vídeos (claro problema de descoberta) → reavaliar sistema, mas testar variações **dentro** dele primeiro antes de sair
- Se identidade Lacuna v2 mudar (manifesto, paleta, tipografia) → atualizar sistema de thumbs em conjunto
- Se algum estudo grande mostrar que thumb sistêmica perde tração no nicho específico de carreira/recrutamento → revisitar

## Quando revisitar

- **Marco sugerido:** após 10 long-forms publicados com sistema visual atual, avaliar CTR médio
- **Trigger de dado:** CTR <2% sustentado por 10+ vídeos consecutivos
- **Trigger institucional:** mudança da identidade visual da Lacuna v2 (manifesto, paleta, tipografia) → adaptar sistema de thumbs
- **Princípio:** decisão atual = heurística baseada em coerência de marca + risco operacional do princípio 11. Manter flexibilidade para ajustar **dentro do sistema** conforme dado real chegar.