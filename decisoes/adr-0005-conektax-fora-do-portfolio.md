# ADR-0005 — Conekta X fica fora do portfolio público da Lacuna

- **Status:** aceita
- **Data:** 2026-05-08
- **Autor:** Gabriel + Claude
- **Escopo:** matriz

## Contexto

O fundador (Gabriel) tem **outro projeto/empresa em operação ativa**: a **Conekta X** (`conektax.com.br`, `@conektax`, CNPJ 65.962.612/0001-00). Está vendendo produto: plataforma de geração de currículo otimizado para passar em sistemas ATS (R$ 29,90+).

Tagline da Conekta X: *"Currículo profissional em 5 minutos aprovado por ATS"*.
Manifesto: *"Não é o seu currículo que tá ruim. É o filtro de RH que tá barrando ele."*

**Detecção de tensão filosófica grave:**

| Conekta X | Marca #1 da Lacuna (em discovery) |
|---|---|
| Trabalha **COM** o sistema ATS | Quer **SUBSTITUIR** o sistema ATS |
| Otimiza currículo | Substitui currículo |
| Score ATS 0-100 | Recusa o filtro como prêmio |
| Currículo profissional em 5 min | Apresentação honesta sem pressa |

São **teses incompatíveis**. Apresentar Conekta X como marca-filha da Lacuna ou no portfolio público violaria:
- Manifesto da Lacuna v2.1: "Cada projeto resolve um vazio. Nada é genérico." (Conekta X otimiza padrão existente)
- Princípio 1 (Honestidade radical): expor um produto que vai contra a tese pública seria contradição insustentável
- Manifesto Versão B: "O jeito antigo desperdiça muita coisa. A gente faz diferente." (Conekta X é otimização do "jeito antigo")

Cronologia provável: Conekta X é o projeto que originou o nome da pasta `curriculo-automatico-inteligente`. A Lacuna como Matriz nasceu de reflexão posterior do fundador, com pivot conceitual para tese oposta (anti-ATS).

## Alternativas consideradas

### A — Conekta X fica FORA do portfolio público da Lacuna ← **escolhida**
- Projeto paralelo do fundador, legado, independente da Lacuna
- Continua operando, vendendo, sem interferência
- Marca #1 da Lacuna mantém tese anti-ATS sem contradição pública
- Maior coerência filosófica e operacional

### B — Conekta X vira cliente/parceiro real, não marca-filha
- Apareceria no portfolio com aviso "tese é do cliente, não da Lacuna"
- Tensão filosófica permanece, contornada por contexto
- Risco: leitor não nota o aviso; leitura pública vira "Lacuna construiu Conekta X" → contradição

### C — Conekta X migra para alinhar com tese Lacuna
- Repensar produto público para não ser "otimização ATS"
- Risco grave: destrói operação atual que está vendendo
- Rejeitado.

### D — Marca #1 (RH humano) é que repensa
- Pausar/repensar Marca #1 porque o fundador já tem Conekta X ativa
- Rejeitado: a Marca #1 é projeto novo da Lacuna; não há razão para canibalizá-la pela Conekta X que tem outra natureza

## Decisão

**Conekta X é projeto paralelo do fundador**, externo ao framework da Lacuna Studio:

1. **NÃO criar** `marcas/02-conektax/` no hub da Lacuna
2. **NÃO listar** Conekta X no "Trabalho em construção" do site v2 da Lacuna
3. **NÃO mencionar** Conekta X na presença pública da Lacuna (site, redes, manifesto, copy)
4. **Conekta X continua operando independentemente** — site, IG, vendas, CNPJ próprios, sem interferência
5. **A Marca #1 da Lacuna (RH humano) segue com sua tese anti-ATS** — sem precisar negar publicamente a Conekta X

## Consequências

### O que fica mais fácil
- Manifesto Lacuna mantém integridade total
- Marca #1 desenvolve sua tese sem precisar negociar com produto contrário
- Conekta X continua operação atual sem reposicionamento forçado
- Princípio 1 (Honestidade radical) preservado

### O que fica mais difícil
- Fundador tem dois "chapéus" ativos simultaneamente (operador Conekta X + construtor Lacuna+Marca #1)
- Se Conekta X aparecer publicamente associado ao fundador (ex: bio do LinkedIn pessoal), pode haver confusão de quem pergunta "mas você não tem outra coisa anti-ATS?"
- Marca #1 vai ser construída tecnicamente em paralelo a Conekta X — possível conflito de tempo/energia do fundador

### O que precisa ser revisado se isso mudar
- Se Conekta X for descontinuada → pode ser absorvida no histórico da Lacuna como "experimento anterior" (com transparência)
- Se Marca #1 pivotar para algo que se complementa com Conekta X (improvável dado pivot já feito) → reabrir
- Se fundador quiser fazer "ponte narrativa" pública entre os dois (ex: post no LinkedIn explicando trajetória) → planejar copy específico, fora do framework da Lacuna

## Notas operacionais

- **Conekta X não entra no learning-log da Lacuna** como projeto ativo (apenas como contexto desta ADR)
- **Memória do Claude** registra a separação para futuras IAs entenderem o contexto sem confundir
- **Bio pessoal do fundador** (LinkedIn, etc.) pode mencionar ambos como projetos, sem precisar reconciliar publicamente

## Referências

- [matriz/identidade/manifesto.md](../../matriz/identidade/manifesto.md) — manifesto da Lacuna que a Conekta X violaria se incluída
- [marcas/01-rh-humano/PROJECT.md](../../marcas/01-rh-humano/PROJECT.md) — Marca #1 com tese oposta à Conekta X
- [matriz/identidade/site-v2-esqueleto.md](../../matriz/identidade/site-v2-esqueleto.md) — seção "Trabalho em construção" que NÃO incluirá Conekta X
