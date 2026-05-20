# ADR-0013 — Lacuna Studio absorve tese de ecossistema; Lacuna Loom revertida

- **Status:** aceita
- **Data:** 2026-05-19
- **Autor:** Gabriel + Claude
- **Escopo:** matriz
- **Substitui:** [ADR-0012](adr-0012-lacuna-loom-marca-02-metodo-comunidade.md) (criada na MESMA sessão, ~6h antes; revertida por priorização de velocidade vs receita)
- **Relaciona:**
  - [ADR-0009](adr-0009-lacuna-hibrida-hub-builder-operacional.md) — modelo híbrido (portfólio próprio prioritário + serviços pontuais) permanece válido
  - [ADR-0010](adr-0010-lacuna-hub-formalizado.md) — formalização do Hub permanece válida; este ADR amplia o veículo público da Lacuna Studio
  - [ADR-0011](adr-0011-direcao-visual-v3-aprovada-gamma5-fenda.md) — identidade γ.5 Sálvia + mark Fenda continua sendo veículo visual

## Contexto

Mesma sessão de 2026-05-19 que criou Lacuna Loom como Marca #02 via [ADR-0012](adr-0012-lacuna-loom-marca-02-metodo-comunidade.md), depois de 5 turnos socráticos. Trabalho subsequente (constraint faceless + tentativas de copy/manifesto + funil + reframe "ecossistema interno") expôs três tensões críticas que justificam reversão consciente:

### 1. Pressão financeira real do fundador

Declarado explicitamente em mensagem: *"preciso de receita o quanto antes pra reinvestir em ferramentas e branding, tráfego"*, e mais adiante: *"o importante é colocarmos no ar e fazermos acontecer, sem ficar travado em decisões que não nos levam a faturar absolutamente nada enquanto eu só tenho contas pra pagar: assinaturas, contas de casa, custos de vida"*.

Caminho com marca-filha nova exige cravar copy nova, criar landing nova, definir identidade adaptativa, decidir repo público, comunidade tier, etc. = estimativa de 8-12 semanas até primeira receita.

### 2. Lacuna Studio já tem 80% do que precisa pronto

- Identidade visual fechada: γ.5 Sálvia + mark Fenda 02.A ([ADR-0011](adr-0011-direcao-visual-v3-aprovada-gamma5-fenda.md))
- Domínio `lacunastudio.com.br` registrado
- Handles `@lacunastd` ativos
- Manifesto v3 aprovado ([ADR-0008](adr-0008-discovery-textual-v3-aprovado.md))
- Princípios públicos v3 (6 princípios) escritos
- Site Lacuna v3 **implementado** em `gabszeera/lacuna-site`, esperando deploy Netlify

Usar Lacuna Studio como veículo público encurta drasticamente o caminho até primeira receita (~3-5 semanas estimadas).

### 3. Reframe de tese durante a sessão

Fundador corrigiu mid-sessão: *"não sei se a ideia é literalmente o build in public... é mais a ideia de nos ajudarmos, quem está ali dentro, do ecossistema, do framework"*.

Esse reframe tornou Lacuna Loom como entidade separada **menos justificável** — a tese de ecossistema interno de ajuda mútua pode viver dentro de Lacuna Studio sem complicação adicional.

## Decisão

**Reverter ADR-0012.** Lacuna Studio passa a ter dupla função: **holdco institucional + primeiro produto público (ecossistema + método + comunidade)**. Tese, posicionamento, constraint faceless, funil de vendas, estratégia 360 inbound e pricing hipóteses da ADR-0012 são **absorvidos por Lacuna Studio**.

### O que muda

| Antes | Depois |
|---|---|
| Lacuna Studio = holdco institucional discreta | Lacuna Studio = holdco + primeiro produto público (ecossistema + método + comunidade) |
| Lacuna Loom = Marca #02 com identidade própria tonalizada | Revertida; estrutura `marcas/02-lacuna-loom/` arquivada em `docs/arquivados/marcas/02-lacuna-loom/` |
| Tese central: "build in public com método" | Tese central: "ecossistema interno onde quem está dentro se ajuda, com método aplicável" |
| Manifesto Lacuna apenas contemplativo (3 variantes A/B/C) | Manifesto Lacuna ganha Variante D (aplicada/ecossistema) sem invalidar A/B/C |
| Princípios públicos: 6 princípios contemplativos | Princípios públicos ganham princípio novo sobre ajuda mútua/critério de entrada |
| Princípio 10 com exceção pra Lacuna Loom | Princípio 10 mantém flexibilidade por escopo — Lacuna Studio opera com transparência ao ser primeiro produto público |

### O que se preserva (migra direto pra Lacuna Studio)

Praticamente tudo que importa da ADR-0012:

- **Tese central:** método aplicável + comunidade de pares pra fundadores AI-native ano 1 que estão construindo
- **Constraint faceless:** sem rosto/identidade pessoal do fundador; voz coletiva primeira pessoa do plural (memória `feedback_marca_faceless.md` permanece válida, agora aplicada a Lacuna Studio)
- **Reframe ecossistema interno:** não é build in public, é ajuda mútua entre quem está dentro
- **Funil de vendas projetado:** 5 etapas (descoberta → interesse → nutrição → compra → expansão)
- **Estratégia 360 inbound:** orgânica (X/Threads/LinkedIn/IG/TikTok/Newsletter) + paga (Meta Ads R$ 300-500 + Google Ads R$ 200-300 + newsletter cross-promo)
- **Modelo de receita refinado pelo fundador:** material principal PAGO (info-produto), repo público separado GRÁTIS como teaser/SEO/credibilidade, comunidade a decidir (grátis vs paga)
- **Pricing hipóteses:** info-produto R$ 47-97, membership R$ 39-79/mês
- **Critério de saída:** 6 semanas de publicação consistente sem sinais reais = pivotar
- **Custos operacionais endossados:** R$ 500-1.000/mês total
- **Direção tonal aprovada:** mix Are.na (declarativa funcional) + Stripe Press (intelectual low-key) + mínimo radical estilo A24

### O que se perde (custo aceito conscientemente)

- ~3-4h documentado em ADR-0012 + estrutura `marcas/02-lacuna-loom/` — preservadas como histórico/aprendizado
- Domínios `lacunaloom.com`/`.com.br`/`.io` reservados pelo fundador (~R$ 110/ano se mantidos; pode liberar quando renovar)
- Handles `@lacunaloom` em X/Instagram/TikTok/Threads/LinkedIn/GitHub reservados — ficam dormentes
- Pureza arquitetural "holdco multi-marca pública" — Lacuna Studio acumula funções. Reversível no futuro.

## Razões

1. **Velocidade > arquitetura** dado o contexto financeiro real. Tempo até primeira receita é constraint dura.
2. **Princípio 1 (honestidade radical):** pivotar consciente quando se enxerga melhor não é desperdício; insistir por sunk cost é o erro real.
3. **Princípio 5 (cortar escopo agressivamente):** manter Loom como marca-filha só fazia sentido se ALGO ganhava; ganhava rigor arquitetural mas perdia velocidade — tradeoff ruim pro momento atual.
4. **Princípio 14 (parar quando algo não convence antes de comprometer mais):** copy/manifesto Loom desafinaram em múltiplas tentativas; reframe "não é build in public" + pressão financeira tornaram o momento ideal pra revisitar arquitetura inteira antes de comprometer mais.
5. **Lacuna Studio já tem identidade fechada e site pronto:** trabalho dobrado pra criar identidade Loom separada quando Lacuna Studio absorve com pequenas adições.

## Consequências

### Imediatas (executadas nesta sessão)

- `marcas/02-lacuna-loom/` movido pra `docs/arquivados/marcas/02-lacuna-loom/` com header REVERTIDA
- ADR-0012 status muda pra SUBSTITUÍDA, com pointer pro ADR-0013
- PROJECT.md raiz atualizado removendo Marca #02 Loom do mapa ativo
- Lacuna Studio (Matriz) declarada como holdco + primeiro produto público
- DECISIONS-LOG.md atualizado refletindo reversão + ADR-0013 adicionado
- STATE.md, BACKLOG.md, HUB-CHANGELOG.md, SESSION-LOG.md atualizados

### Próximos passos (Onda 4 — agora aplicada a Lacuna Studio)

- Manifesto Lacuna ganha **Variante D** (aplicada/ecossistema) — sessão atual ou próxima
- Princípios públicos ganham **princípio novo** sobre ajuda mútua/critério de entrada
- Copy nova pra landing v0 / about page no tom Are.na + Stripe Press já cravado
- Mockup textual do info-produto (TOC do método embalado, formato, preço)
- Setup ferramentas mínimas (newsletter, venda, comunidade, analytics)
- Repo público separado pro método (decisão técnica: nome, escopo, formato)
- Deploy site Lacuna v3 (já implementado) atualizado pra refletir novo posicionamento
- Publicação consistente por 6 semanas (critério de saída de hipótese forte)

### Médio prazo
- Quando Marca #1 RH humano descongelar (futuro): provável vira marca-filha separada (escopo distinto justifica)
- Se receita escalar, possível reorganização: Lacuna Studio volta a ser holdco institucional silenciosa; primeiro produto público (atual Lacuna Studio) vira marca-filha autônoma com nome próprio
- Domínios `lacunaloom.*` ficam dormentes — decisão futura: manter, liberar, ou usar pra subprojeto

### Risco principal a vigiar
- **Lacuna Studio pode acumular funções demais.** Tem que vigiar pra não virar "marca que faz tudo, mas nada bem". Quando segunda marca-filha pública nascer, possível reorganização (Lacuna Studio volta a ser holdco silenciosa; primeiro produto público vira marca-filha autônoma).

## Aprendizado meta absorvido

Esta ADR substitui outra criada na MESMA sessão (~6h antes). Sinal de:
- Iteração saudável (princípio 1 ativo, sem teimosia por sunk cost)
- Risco de over-engineering antecipado (criamos arquitetura antes de validar mercado)
- Pressão financeira como filtro essencial em fase F0 (sem receita validada, simplicidade vence)

**A registrar no learning-log:** em fase F0 (validação), constraint financeira do fundador deve ser filtro primário pra decisões arquiteturais; arquitetura "pura" pode esperar pós-primeira-receita.

---

**Ato fundador desta reversão:** decisão consciente do fundador 2026-05-19, motivada por clareza sobre pressão financeira e por reconhecimento de que tese central (ecossistema interno + método aplicável) pode viver dentro de Lacuna Studio sem complicação adicional. Sem teimosia. Sem sunk cost. Velocidade primeiro.
