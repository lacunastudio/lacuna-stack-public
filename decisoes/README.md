# Decisões registradas — ADRs da Matriz Lacuna

> Esta pasta contém ADRs reais da Lacuna Studio. Decisões estratégicas e operacionais registradas no momento em que foram tomadas, com contexto e razão.

---

## O que é uma ADR

**ADR** = Architecture Decision Record (Registro de Decisão de Arquitetura).

É um documento curto que registra uma decisão importante no momento em que foi tomada. Inclui:

- **Contexto** — qual problema/pergunta estava em jogo
- **Decisão** — o que foi escolhido
- **Razão** — por que essa opção em vez das outras
- **Consequências** — o que muda como resultado
- **Status** — proposta, aceita, depreciada, ou substituída

ADRs preservam a memória das decisões. Quando alguém pergunta "por que vocês escolheram isso?" meses depois, a resposta está documentada em vez de perdida em conversa de chat.

O conceito de ADR vem da engenharia de software, mas a Lacuna aplica em todas as áreas (visual, estratégia, posicionamento, técnico).

---

## ADRs neste repositório

São treze ADRs da Matriz (a entidade Lacuna como um todo), por ordem cronológica. Note que **ADR-0006 foi pulada** (foi proposta mas descartada antes de virar registro).

| # | ADR | Tema |
|---|---|---|
| 1 | [adr-0001-youtube-autoridade-vertical.md](adr-0001-youtube-autoridade-vertical.md) | YouTube como canal de autoridade |
| 2 | [adr-0002-youtube-long-form-primario-shorts-recorte.md](adr-0002-youtube-long-form-primario-shorts-recorte.md) | Long-form como formato primário, Shorts como recorte |
| 3 | [adr-0003-youtube-thumbs-sistema-visual-coerente.md](adr-0003-youtube-thumbs-sistema-visual-coerente.md) | Sistema visual coerente pra thumbnails |
| 4 | [adr-0004-paleta-modo-claro-verde-musgo.md](adr-0004-paleta-modo-claro-verde-musgo.md) | Paleta inicial em modo claro verde-musgo |
| 5 | [adr-0005-conektax-fora-do-portfolio.md](adr-0005-conektax-fora-do-portfolio.md) | Marca anterior do fundador (Conektax) fora do portfólio |
| 6 | _0006 pulada_ | (descartada antes de virar registro) |
| 7 | [adr-0007-pivo-identidade-visual-v2-para-v3.md](adr-0007-pivo-identidade-visual-v2-para-v3.md) | Pivô de identidade visual v2 → v3 |
| 8 | [adr-0008-discovery-textual-v3-aprovado.md](adr-0008-discovery-textual-v3-aprovado.md) | Discovery textual v3 aprovado |
| 9 | [adr-0009-lacuna-hibrida-hub-builder-operacional.md](adr-0009-lacuna-hibrida-hub-builder-operacional.md) | Lacuna como híbrida hub + builder operacional |
| 10 | [adr-0010-lacuna-hub-formalizado.md](adr-0010-lacuna-hub-formalizado.md) | Lacuna Hub formalizado como camada |
| 11 | [adr-0011-direcao-visual-v3-aprovada-gamma5-fenda.md](adr-0011-direcao-visual-v3-aprovada-gamma5-fenda.md) | Direção visual v3 aprovada (γ.5 Sálvia + mark Fenda) |
| 12 | [adr-0012-lacuna-loom-marca-02-metodo-comunidade.md](adr-0012-lacuna-loom-marca-02-metodo-comunidade.md) | Lacuna Loom como marca #02 (método + comunidade) |
| 13 | [adr-0013-lacuna-studio-absorve-tese-loom-revertida.md](adr-0013-lacuna-studio-absorve-tese-loom-revertida.md) | Lacuna Loom revertida; Studio absorve a tese |
| 14 | [adr-0014-lacuna-stack-framework-ai-portavel.md](adr-0014-lacuna-stack-framework-ai-portavel.md) | Lacuna Stack como framework AI-portável |

---

## Como ler

**Por contexto:** se você quer entender uma decisão específica, leia a ADR direto.

**Por ordem cronológica:** se quer ver a evolução da Lacuna, lê 0001 → 0014 em ordem. Mostra o que foi decidido, o que foi revertido, e como o método se construiu junto com a empresa.

**Atenção especial:** ADR-0012 e ADR-0013 mostram uma decisão tomada e revertida na mesma sessão. ADR-0014 estabelece a tese de portabilidade entre IAs. Esses três contêm os movimentos estratégicos mais recentes da Lacuna Studio.

---

## Por que ADRs públicas?

A maioria das empresas mantém decisões internas confidenciais. A Lacuna escolheu publicar as ADRs da Matriz como prova de trabalho. Você vê:

- Como decidimos (estrutura repetível)
- O que decidimos (conteúdo específico)
- Por que decidimos (razões registradas, não retroativamente racionalizadas)
- Quando mudamos de ideia (decisões revertidas ficam registradas, não apagadas)

Isso é diferente de blog post de "lições aprendidas" — ADRs são contemporâneas à decisão, não posthoc.

---

## ADRs das Marcas

Marcas-filhas da Lacuna (atualmente Marca #1 RH humano) têm ADRs próprias em `decisoes/marca-[nome]/` no hub interno. Algumas vão sendo publicadas aqui conforme deixarem de ser sensíveis.

---

> Pasta atualizada conforme novas ADRs entram. Cada commit que adiciona ADR aparece no [HUB-CHANGELOG](../docs/HUB-CHANGELOG.md).
