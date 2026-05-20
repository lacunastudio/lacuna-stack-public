# Como funciona o Lacuna Stack

> Visão geral do método. Sem detalhe operacional (esse vive no produto pago).

---

## A estrutura conceitual

O Lacuna Stack organiza um projeto/empresa em três camadas:

### Matriz

A identidade e operação da empresa-portfólio como um todo. Princípios, manifesto, identidade visual, posicionamento, presença pública. Quando você é founder solo com um projeto, a Matriz pode ficar enxuta (ou inexistente). Quando o projeto cresce pra empresa portfólio, a Matriz se expande.

### Sistema

O método reutilizável. Metodologias, regras, processos, conhecimento acumulado. Esta camada é compartilhada entre todos os projetos da empresa. Inclui ferramentas como:

- Lentes de novo projeto
- Fases F0-F4 (validação → tração)
- Distribuição financeira 35/50/15
- Métodos de documentação
- Versionamento
- Pesquisa e fontes vivas

### Marcas (ou projetos)

Os projetos concretos. Cada um com sua identidade, produto, audiência, financeiro. Empresa portfólio tem várias; founder solo tem um. Cada marca segue o método (Sistema) e respeita os princípios (Matriz), mas opera com autonomia.

---

## O ciclo de trabalho com IA

O Stack pressupõe que você usa uma IA principal (Claude, ChatGPT, Cursor, Windsurf, Gemini). O método estrutura como você trabalha com essa IA:

1. **A IA lê o hub.** Arquivos meta (CLAUDE.md, CONTEXT.md, PROJECT.md, STATE.md) são lidos automaticamente no início da sessão. A IA chega contextualizada.

2. **A IA aplica princípios.** Os 29 princípios orientam decisão. Regras escopadas (anti-alucinação, design execution, etc.) entram em situações específicas.

3. **A IA invoca agentes.** Pra trabalho especializado, a IA usa agentes (design-ux, brand-identity, copy-writer, etc.) com instruções específicas.

4. **A IA executa skills.** Slash commands (`/decidir`, `/discovery`, `/sync`, `/git-save`, etc.) automatizam fluxos repetíveis.

5. **A IA documenta tudo.** Cada decisão grande vira ADR. Cada sessão fecha com `/sync` (atualiza STATE.md + SESSION-LOG). Trabalho não-documentado é trabalho perdido.

6. **A IA aprende com você.** Co-evolução bidirecional: a IA propõe melhorias ao Hub quando descobre padrão melhor; você valida ou redireciona.

Esse ciclo se repete em todas as escalas: decisão pequena (1 sessão), decisão grande (ADR), refator (várias sessões com handoff estruturado entre elas).

---

## Portabilidade entre IAs

O Stack é otimizado pra Claude Code (foi onde nasceu e foi testado), mas o núcleo é markdown puro. Portável pra:

- **ChatGPT** — via Projects + Instructions
- **Cursor** — via `.cursorrules` + `.cursor/rules/`
- **Windsurf** — via `.windsurfrules`
- **Gemini Code Assist** — via documentação do projeto
- **Outras IAs** — qualquer uma que leia markdown estruturado

O produto pago tem capítulo dedicado a cada uma das 5 IAs principais com instruções específicas de adaptação.

---

## Fases F0-F4

Toda marca/projeto passa por fases. O Stack define cinco:

- **F0 — Validação.** Discovery, hipóteses, primeiros sinais. Sem receita ainda.
- **F1 — Primeiros sinais.** Primeiras conversões, validação de hipóteses chave.
- **F2 — Tração inicial.** Receita recorrente começando. CAC < LTV em sinal.
- **F3 — Crescimento.** Modelos de aquisição validados. Equipe começando a expandir.
- **F4 — Escala.** Operação madura, otimizações em CAC/LTV/NRR.

Cada fase tem critérios de saída claros (não prazo). Você não avança por tempo; avança por marco.

Detalhes operacionais no Manual em PDF (Parte 2 — Método Operacional).

---

## Distribuição financeira 35/50/15

A Lacuna aplica preset financeiro nas marcas-filhas:

- **35% — Fundador (pró-labore)**
- **50% — Reinvestimento no projeto**
- **15% — Reserva (fiscal + emergência)**

Não é regra dogmática; é ponto de partida que se ajusta conforme contexto. Detalhe operacional no Manual.

---

## O que esse método resolve

- **Trabalho que vira chat volátil.** Decisões importantes ficam registradas em ADR, não perdidas em conversa.
- **IA solta sem método.** A IA sabe o que você decidiu antes, segue princípios, aplica regras escopadas.
- **Reinventar processo a cada projeto.** O Sistema é reutilizável entre marcas-filhas.
- **Falta de scaffold operacional.** Em vez de começar com pasta vazia, você começa com estrutura adaptável.

---

## O que esse método NÃO resolve

- **Falta de ideia.** O Stack ajuda você a executar; não inventa o que executar.
- **Falta de disciplina.** Princípios são propostas; aplicação depende de você.
- **Falta de mercado.** Método não substitui validação real com clientes pagantes.

---

## Próximos passos

- **Quer ver os princípios completos:** [CLAUDE.md](../CLAUDE.md)
- **Quer ver decisões reais aplicando o método:** [decisoes/](../decisoes/)
- **Quer comprar o produto completo:** [comprar.md](comprar.md)

---

> Página pública. Detalhes operacionais no Manual em PDF (produto pago).
