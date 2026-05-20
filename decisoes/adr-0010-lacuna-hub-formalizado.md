# ADR-0010 — Lacuna Hub formalizado como central viva de criação + arquitetura de continuidade cross-IA + metodologia de fases F0-F4

- **Status:** aceita
- **Data:** 2026-05-12
- **Autor:** Gabriel + Claude
- **Escopo:** matriz
- **Relaciona:** [ADR-0009](adr-0009-lacuna-hibrida-hub-builder-operacional.md) (Hub como builder operacional — base), [CLAUDE.md](../../CLAUDE.md) (princípios 25-28 adicionados), [matriz/principios-empresa.md](../../matriz/principios-empresa.md), [PROJECT.md](../../PROJECT.md), [CONTEXT.md](../../CONTEXT.md), [STATE.md](../../STATE.md), [docs/inputs/2026-05-12-ideias-framework.md](../../docs/inputs/2026-05-12-ideias-framework.md) (raciocínio que gerou esta ADR)

## Contexto

Após validar o primeiro builder do Bloco II ([`/criar-marca-filha`](../../.claude/skills/criar-marca-filha/SKILL.md), 2026-05-11), fundador pausou os builders restantes e abriu sessão dedicada à evolução do framework. Conduzida em 3 passos:

1. **Despejo livre** — fundador descreveu o que está sendo construído como **maior do que "framework"**: uma **central viva de criação** onde negócios sustentáveis nascem com investimento mínimo, escalam com padrões pré-estabelecidos por tipo, e alimentam a central de volta com lições + ferramentas + automações
2. **Imagem rabiscada** — desenho manual com 4 fases de criação de projeto + esquema de distribuição financeira + nota sobre empresa-online-multi-tipo
3. **Despejo guiado** — perguntas-pivôs sobre identidade, continuidade cross-IA, tipologia de projetos e inteligência de saúde

A sessão gerou material denso registrado em [docs/inputs/2026-05-12-ideias-framework.md](../../docs/inputs/2026-05-12-ideias-framework.md). Esta ADR consolida as decisões formais que viraram artefatos no Hub.

## Decisão

### 1. Nome formal do "sistema" — **Lacuna Hub**

A central de criação tem nome formal: **Lacuna Hub**. Empresa-mãe é Lacuna Studio (fundador solo por ora). Visibilidade interna por padrão — pode tornar-se pública algum dia através da Lacuna Studio (não inicial).

**Caráter:** infinitamente evoluível, bidirecional com projetos.

**Métrica macro:** **menor tempo do fundador × maior automação × maior rentabilidade** (triângulo, não eixo único).

### 2. Princípios fundadores novos (25-28) adicionados ao CLAUDE.md

- **25. Co-evolução fundador↔IA bidirecional** — Claude não é só executor. Também busca fontes, propõe melhorias, registra evolução. Fundador valida/redireciona.
- **26. HUB-ENTRY como entrada única cross-IA** — Toda IA/conta nova lê `HUB-ENTRY.md` (raiz) primeiro — resumo + apontamentos para continuar. Princípio 18 cobre micro (auto-suficiência por pasta); este cobre macro (auto-suficiência cross-instância).
- **27. Continuidade cross-conta (Claude-first)** — Memória persistente do Claude (`~/.claude/projects/.../memory/`) pode ser perdida na troca de conta. **Fonte da verdade migra para `.claude/onboarding/` versionado no repo**. Claude-first; outras IAs aceitam modo degradado.
- **28. Projetos podem modificar a central com rito** — Bidirecionalidade controlada. Projeto que descobrir padrão melhor pode propor mudança no Hub, **mas precisa notificar fundador + trazer fontes/dados reais que justifiquem antes**.

### 3. Metodologia de fases F0-F4 (aplicada individualmente por projeto)

Cada empresa/marca/produto que o fundador construir passa por 5 fases. Aplicada também a casos futuros com investimentos externos / participações menores.

| Fase | Faturamento-alvo | Dedicação fundador | Critério de transição |
|---|---|---|---|
| **F0 — Validação** | R$ 25k/mês com **30% margem líquida pro fundador** (R$ 7.500) | flex (sem padrão fixo) | Validar tese + atingir 25k com margem |
| **F1 — Construção** | R$ 150k/mês | seg-sex 7h ideal / **6h mín** · sáb-dom 3h ideal / 1h30 mín | Operar manualmente só dentro do tempo de F1 → libera escolha entre F2 ou manter |
| **F2 — Escala 1** | R$ 1MM (1kk)/mês | seg-sex 5h ideal / 4h mín · fds 2h ideal / 1h mín | Operar só dentro do tempo de F2 → libera escolha |
| **F3 — Escala 2** | R$ 10MM+ (10kk+)/mês | seg-sex 3h · fds 1h | Operar só dentro do tempo de F3 → libera escolha |
| **F4 — Manutenção** | R$ 10MM+ (sustentar) | seg-sex 1h · fds 30min — **fundador monitora pessoalmente, obrigatório** | Terminal ou redistribui foco pra outro projeto |

**Critério operacional de "automatizado":** fundador opera **apenas dentro do tempo estipulado da fase**. Atalhos válidos: automação (software/IA) **ou** delegação (freelas/funcionários).

**Alocação multi-projeto:** **apenas 1 projeto em F1 por vez**. Projetos paralelos só em F2-F4. Flexível conforme portfólio cresce.

Detalhe completo em [sistema/metodologia/fases-projeto.md](../../sistema/metodologia/fases-projeto.md).

### 4. Distribuição financeira (preset)

| Fatia | % | Detalhe |
|---|---|---|
| Pessoal | **35%** | Forma flexível — pro-labore, participação de lucros, distribuição — qualquer veículo que minimize impostos no contexto fiscal específico |
| Empresa | **50%** | Custos operacionais + caixa |
| Guardar | **15%** | **7,5% reserva pessoal + 7,5% futuras empresas/produtos/features** |

**Validade:** preset 35/50/15 só vale em **F1+** quando custos são previsíveis. Em **F0**, a regra é apenas "30% margem líquida pro fundador" (R$ 7.500 sobre R$ 25k).

**Camada acima:** módulo de saúde financeira adaptativa (Onda 3 — agente `saude-financeira` + skill `/avaliar-saude` + cron mensal) sugere ajustes em tempo real conforme estado do projeto.

Detalhe completo em [sistema/metodologia/distribuicao-financeira.md](../../sistema/metodologia/distribuicao-financeira.md).

### 5. Continuidade cross-IA (arquitetura)

**HUB-ENTRY.md** (raiz) é a entrada única para toda IA/conta nova. Resume o Hub Lacuna em 1 página + aponta a sequência de leitura:

```
HUB-ENTRY.md → .claude/onboarding/ → CLAUDE.md → STATE.md → SESSION-LOG.md → arquivos sob demanda
```

**`.claude/onboarding/`** (pasta nova) espelha no repo o conteúdo essencial da memória persistente local do Claude:

```
.claude/onboarding/
├── 01-founder.md        ← perfil do fundador (espelho de user_profile.md)
├── 02-working-style.md  ← feedbacks acumulados (consolida 7 feedback_*.md)
├── 03-project-vision.md ← visão macro (espelho de project_vision.md)
└── 04-structure.md      ← estrutura do hub (espelho de project_structure.md)
```

**Regras:** fonte da verdade = repo. Memória local Claude vira cache acelerador. Skill `/migrar-memoria` (Onda 2) reconcilia local↔repo periodicamente.

### 6. Tipologia de projetos — 2 grandes tipos com variantes

| Tipo grande | Pasta | Variantes (por escopo) |
|---|---|---|
| **Próprios** | `marcas/` | Marca completa · Produto isolado · SaaS · Serviço próprio · outras formas online |
| **Cliente (terceiros)** | `clientes/` | A definir conforme primeiro caso real (modelo de fases pode ser diferente) |

**Quem opera o projeto em F4:** fundador continua em **monitoramento pessoal obrigatório** (1h seg-sex + 30min fds). Não pode ser delegado. Resto = combinação variável de automação + IA + freelas + funcionários por projeto.

### 7. Ritos de evolução do Hub

- **`docs/HUB-CHANGELOG.md`** (novo, Onda 2) — cronologia da evolução do Hub em si (princípios, regras, skills, agentes, estrutura). Cada entrada aponta para ADR/commit/SESSION-LOG. Updates via `/sync` quando há mudança na central.
- **`docs/arquivados/`** (nova, Onda 2) — pasta com 5 subpastas (`principios/`, `skills/`, `agentes/`, `regras/`, `metodologias/`). Item aposentado preserva conteúdo + header com razão + link pro ADR de aposentadoria. Pode ser removido definitivamente depois.
- **Skill `/aposentar [tipo] [nome]`** (nova, Onda 2) — formaliza o rito (move arquivo + adiciona header + registra no CHANGELOG).
- **Skill `/migrar-memoria`** (nova, Onda 2) — reconcilia memória local Claude com `.claude/onboarding/` versionado.

### 8. Implementação em 4 ondas

- **Onda 1 (núcleo):** princípios 25-28 + HUB-ENTRY.md + `.claude/onboarding/` + STATE.md + fases-projeto.md + distribuicao-financeira.md
- **Onda 2 (infraestrutura):** `docs/HUB-CHANGELOG.md` + `docs/arquivados/` + skill `/aposentar` + skill `/migrar-memoria`
- **Onda 3 (saúde):** agente `saude-financeira` + skill `/avaliar-saude` + cron mensal
- **Onda 4 (limpeza):** rebrandig "framework"→"Lacuna Hub" onde fizer sentido

## Consequências

### Positivas

- **Continuidade real cross-IA/cross-conta** — troca de conta Claude Max não perde mais contexto. Outras IAs entram em modo degradado funcional.
- **Mecânica de progressão clara por projeto** — F0-F4 com critérios mensuráveis (faturamento + tempo do fundador) substitui ambiguidade de "quando escalar?".
- **Distribuição financeira normalizada** — preset 35/50/15 evita decisão ad-hoc mês a mês; inteligência de saúde adaptativa cuida das exceções.
- **Bidirecionalidade controlada** — projetos podem evoluir a central sem caos (rito obrigatório de notificar + fontes).
- **Vocabulário consolidado** — "Lacuna Hub" como nome formal reduz ambiguidade de "framework"/"sistema"/"central".
- **Rito de evolução estruturado** — HUB-CHANGELOG dá visão temporal da central; arquivados preserva histórico do que saiu.

### Negativas / tradeoffs aceitos

- **Mais artefatos para manter** — HUB-ENTRY, onboarding/, HUB-CHANGELOG, arquivados/ aumentam a superfície. Mitigação: skills (`/aposentar`, `/migrar-memoria`) e `/sync` estendido automatizam updates.
- **Princípio 10 (discrição sobre stack/IA) vs Lacuna Hub público** — se Hub virar público algum dia, releitura desse princípio será necessária. Por ora não-acionável.
- **Memória local Claude vira cache, não fonte** — mudança de modelo mental; pode gerar atrito até `/migrar-memoria` estar pronta. Mitigação: durante Onda 2, escrever-em-ambos manualmente.
- **F0-F4 é hipótese ainda não validada em prática** — números são metas direcionais. Aprendizado real ajustará valores em ADRs futuras.

### Operacionais (executados nesta sessão)

- Adicionar princípios 25-28 ao [CLAUDE.md](../../CLAUDE.md)
- Criar [HUB-ENTRY.md](../../HUB-ENTRY.md) na raiz
- Criar [.claude/onboarding/](../../.claude/onboarding/) com 4 arquivos
- Atualizar [STATE.md](../../STATE.md) — Lacuna Hub formal + F0 25k + foco evolução framework
- Criar [sistema/metodologia/fases-projeto.md](../../sistema/metodologia/fases-projeto.md)
- Criar [sistema/metodologia/distribuicao-financeira.md](../../sistema/metodologia/distribuicao-financeira.md)
- Atualizar [PROJECT.md](../../PROJECT.md) + [matriz/principios-empresa.md](../../matriz/principios-empresa.md) refletindo Lacuna Hub formal
- Atualizar [BACKLOG.md](../../BACKLOG.md) marcando concluídos + adicionando ondas 2/3 como roadmap
- Atualizar [DECISIONS-LOG.md](../../DECISIONS-LOG.md) adicionando ADR-0010

## O que NÃO muda

- Princípios fundadores 1-11 da [matriz/principios-empresa.md](../../matriz/principios-empresa.md) — todos permanecem
- Princípios 1-24 do CLAUDE.md — todos permanecem (princípios 25-28 adicionam, não substituem)
- Estrutura macro `matriz/` + `sistema/` + `marcas/` + `clientes/` + `decisoes/` + `docs/` + `.claude/`
- Skill `/criar-marca-filha` (recém-validada) — preservada
- Metas concretas das marcas em construção (Marca #1 / RH humano) — paralelas e intocadas
- Plano de assinatura escalonado ([STATE.md](../../STATE.md)) — preservado, vira insumo da metodologia financeira

## Pontos em aberto pra futuras ADRs

- **Variantes de projeto próprio** (marca / produto / SaaS / serviço próprio / outras formas online) — definir templates próprios por variante ou tratar como sub-tipos dentro de `marcas/`?
- **Modelo de fases pra projetos cliente** — diferente das F0-F4. Decidir quando 1º caso real surgir.
- **Fase 4 final** — terminal puro ou ponto de redistribuição? Decidir quando 1º projeto chegar lá.
- **Princípio 10 vs Lacuna Hub público** — releitura quando decisão de tornar Hub público for tomada.

## Referências

- [docs/inputs/2026-05-12-ideias-framework.md](../../docs/inputs/2026-05-12-ideias-framework.md) — raciocínio bruto e tabelas que geraram esta ADR
- [ADR-0009](adr-0009-lacuna-hibrida-hub-builder-operacional.md) — Hub como builder operacional (base estrutural)
- [Princípio 18 CLAUDE.md](../../CLAUDE.md) — auto-suficiência por pasta (este princípio 26 estende para escala macro/cross-instância)
- [Princípio 19 CLAUDE.md](../../CLAUDE.md) — documentação como parte do trabalho (esta ADR materializa em práticas concretas)
- [Princípio 24 CLAUDE.md](../../CLAUDE.md) — triggers de skills (skills novas de Onda 2/3 seguem o padrão)
