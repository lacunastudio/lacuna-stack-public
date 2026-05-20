# ADR-0009 — Lacuna como empresa híbrida (portfólio + serviços) e Hub como builder operacional

- **Status:** aceita
- **Data:** 2026-05-09
- **Autor:** Gabriel + Claude
- **Escopo:** matriz
- **Substitui:** [Princípio fundador #8 anterior](../../matriz/principios-empresa.md) (versão "empresa portfólio com possibilidade futura de servir terceiros")
- **Relaciona:** [CLAUDE.md](../../CLAUDE.md) · [PROJECT.md](../../PROJECT.md) · [CONTEXT.md](../../CONTEXT.md) · [.claude/rules/investigar-solucoes.md](../../.claude/rules/investigar-solucoes.md) (criada nesta ADR)

## Contexto

Conversa de reformatação aberta em 2026-05-09 (ver [SESSION-LOG.md](../../docs/SESSION-LOG.md)). Após pausa formal de todas as tasks visuais Lacuna v3 e renomeação do hub para `lacuna-hub`, fundador formalizou três viradas fundadoras simultâneas que justificam decisão registrada antes de qualquer implementação:

1. **Lacuna deixa de ser portfólio puro.** Passa a ser **empresa híbrida ativa**: marcas/produtos próprios **+** serviços a terceiros (criação de marcas, branding, identidade visual, sites, SaaS, sistemas internos, automações) quando a oportunidade aparecer. **Foco de prioridade segue sendo o portfólio próprio**; serviços a terceiros entram quando o caso real surgir, não como porta de captação ativa preventiva.

2. **Hub deixa de ser só "central de inteligência viva".** Passa a ser **framework + central operacional + builder real**. Inteligência continua, mas ganha camada de **execução** — builders rodáveis, MCPs ativados, skills com side-effect que produzem artefato pronto.

3. **Critério de qualidade vira "alto em todas as áreas trabalhadas".** Não simultaneamente — step-by-step, no que estiver sendo trabalhado em cada momento. Áreas declaradas: design, desenvolvimento, automações, copy, SEO, financeiro, jurídico/burocracia, código, segurança, tráfego pago.

A virada surge do reconhecimento de que (a) o hub tem maturidade alta enquanto a Marca #1 não tem cliente, (b) a identidade Lacuna emperrou em 4 rounds de tentativa visual sem nível desejado, (c) abrir para serviços a terceiros pode trazer aprendizado e fluxo de caixa antes da Marca #1 estar madura, sem desviar foco principal.

## Decisão

### 1. Reescrita do princípio fundador #8

De:
> "Empresa portfólio, com possibilidade futura de servir terceiros."

Para:
> "Empresa híbrida: portfólio próprio prioritário + serviços a terceiros quando a oportunidade aparecer. A Lacuna abriga marcas/produtos próprios como foco de longo prazo (ativo de marca + audiência + autoridade) e presta serviços externos pontualmente — não como pipeline ativo de captação, mas como porta aberta para casos relevantes que aparecerem. Decisões respeitam a prioridade do portfólio mas não fecham a porta de serviços."

### 2. Hub vira builder operacional

Camadas confirmadas do Hub a partir desta ADR:

- **Camada de inteligência** (existia): princípios, metodologia, learning-log, pesquisas, ADRs, documentação viva
- **Camada de método** (existia parcialmente): agentes especializados, regras escopadas, skills de processo
- **Camada de execução** (NOVA): MCPs ativados (Higgsfield, Meta Ads, Google Ads, GA4, Figma, Vercel, Notion, Stripe, etc. conforme demanda), skills com side-effect (`/criar-marca`, `/criar-projeto-cliente`, `/criar-landing`, etc.), templates rodáveis

### 3. Pasta `clientes/` criada

Estrutura paralela a `marcas/` para abrigar projetos de serviço a terceiros. Não confunde com Marca-filha — Marca-filha é da Lacuna, Cliente-projeto é de terceiro com escopo + entregável + valor. Ver [clientes/CONTEXT.md](../../clientes/CONTEXT.md) e [clientes/TEMPLATE-projeto.md](../../clientes/TEMPLATE-projeto.md).

### 4. Nova regra `.claude/rules/investigar-solucoes.md`

Regra carregada **sempre que o fundador relatar dificuldade técnica, gap de capacidade, ou ineficiência de processo**. Obriga: pesquisar HOJE (com data) por MCPs/skills/agents/APIs/ferramentas existentes antes de construir solução do zero. Materializa princípio 17 do CLAUDE.md aplicado ao próprio Hub.

### 5. Roadmap de afiação por blocos

Aceito o roadmap proposto na sessão anterior (Blocos I-V), com priorização:

- **Bloco I — Fundação** (esta ADR + princípios + pasta `clientes/` + regra investigar-solucoes) → executado nesta sessão
- **Bloco II — Builders reais** (skills `/criar-marca-filha`, `/criar-projeto-cliente`, `/criar-landing`, `/criar-campanha-paga`, `/gerar-imagem-prompt`) → próxima sessão dedicada
- **Bloco III — Cobertura nova** (agentes `financeiro-tributario`, `video-creator`; skills `/setup-tracking`, `/setup-seo`) → conforme demanda
- **Bloco IV — Conexões externas** (MCPs Higgsfield/Figma/Notion/Meta Ads/Google Ads/GA4 conforme caso) → conforme orçamento e necessidade
- **Bloco V — Qualidade contínua** (atualizar `/auditar` e `/saude-hub`, catálogo de referências visuais) → contínuo

### 6. Política de gasto

Confirmada na sessão: budget até **~$100 USD/mês** para assinaturas, **com cautela e validação primeiro**. Princípio: tentar gratuito antes; assinar quando há caso real que justifica; pesquisar profundamente antes de pagar; cancelar se não resolver. Cenários $0 → $29 → $56 → $85 documentados na sessão.

## Consequências

### Positivas
- **Caminho de receita acelerado:** serviços a terceiros podem gerar caixa antes da Marca #1 estar madura
- **Aprendizado por exposição real ao mercado:** servir cliente externo expõe gaps que projeto próprio esconde
- **Hub vira ferramenta real, não só meta-trabalho:** builders rodáveis transformam o hub em capacidade aplicável, reduzindo risco de virar refúgio
- **Regra investigar-solucoes:** força que toda dificuldade vire pesquisa primeiro, não construção do zero — economiza tempo e ancora em soluções consolidadas

### Negativas / tradeoffs aceitos
- **Foco mais difícil de manter:** com 2 frentes (portfólio + serviços), risco de dispersão é real. Mitigação: prioridade do portfólio mantida no princípio.
- **Comunicação pública mais complexa:** "empresa portfólio + serviços" é mais difícil de pitchar que "studio que faz X". Aceito — categoria continua deliberadamente em aberto (princípio #9).
- **Princípio 10 (discrição sobre stack/IA) pode entrar em tensão** quando vendendo serviço AI-native. Tratado caso a caso — princípio mantido como padrão; menção pública vira decisão consciente quando agrega valor.
- **Hub fica mais complexo:** mais MCPs, mais skills, mais regras. Mitigação: leitura sob demanda (princípio de otimização de tokens), MCPs só ativados quando necessário.

### Operacionais
- Atualizar [matriz/principios-empresa.md](../../matriz/principios-empresa.md) — princípio #8 reescrito
- Atualizar [PROJECT.md](../../PROJECT.md) da Matriz — framing híbrido + camadas do Hub
- Atualizar [CONTEXT.md](../../CONTEXT.md) raiz — acrescentar pontos do framing híbrido
- Criar [clientes/](../../clientes/) com CONTEXT, README, TEMPLATE
- Criar [.claude/rules/investigar-solucoes.md](../../.claude/rules/investigar-solucoes.md)
- [DECISIONS-LOG.md](../../DECISIONS-LOG.md) atualizado com esta ADR
- [STATE.md](../../STATE.md) e [docs/SESSION-LOG.md](../../docs/SESSION-LOG.md) atualizados

## O que NÃO muda

- Princípios fundadores 1-7 e 9-11 permanecem (marca > produto, crescimento orgânico, audiência, etapas, evolução, embasamento real, honestidade radical, categoria em aberto, discrição sobre stack, comunicação institucional)
- 24 princípios CLAUDE.md permanecem, com 1 ajuste em #8 referência cruzada
- Estrutura `matriz/` + `sistema/` + `marcas/` permanece — pasta `clientes/` adiciona, não substitui
- Marca #1 (RH humano) intocada, segue paralela
- Identidade Lacuna v3 textual aprovada (ADR-0008) preservada — visual continua pausado até nova abordagem (provavelmente via Higgsfield + Recraft conforme plano de assinatura)

## Referências

- Pesquisa MCP consolidada na sessão de 2026-05-09 (Meta Ads MCP oficial 29/04/2026, Higgsfield MCP 30/04/2026, Figma Dev Mode MCP, Canva MCP 09/02/2026, Recraft V4 SVG, Google Ads MCP, GA4 MCP, Vercel/Notion/Stripe MCPs oficiais)
- Princípio 17 CLAUDE.md (investigar antes de construir)
- Princípio 22 CLAUDE.md (isolamento por conversa) — esta sessão é continuação direta da reformatação aberta, sem mudança de escopo
