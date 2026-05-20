# ADR-0002 (Matriz) — Long-form como formato primário do canal YouTube; Shorts apenas como recorte derivado

- **Status:** aceita
- **Data:** 2026-05-08
- **Autor:** Gabriel + Claude (com pesquisa de mercado fundamentada)
- **Escopo:** matriz

## Contexto

YouTube tem hoje (fim de 2025 em diante) **dois formatos com algoritmos completamente decoupados**: long-form e Shorts. São feeds separados, rankers separados, e a audiência tem **~10% de overlap** (Subscribr 2026; Outlierkit 2026; AIR Media-Tech 2025).

Risco documentado conhecido como **"Shorts trap"**:
- Canal acumula views em Shorts mas conversão para long-form fica em **1-3%**
- Audiência de Shorts não migra para 15min de papo
- Tom/ritmo dos Shorts (cortes rápidos, gancho de 3s) cria dissonância cognitiva com long-form mais reflexivo
- Subs ganhos por Shorts inflam contagem mas **não impactam watch time do canal todo**

Contra-argumento: canais que combinam long-form e Shorts crescem **34-41% mais rápido** que mono-formato — mas a chave é **coerência tonal entre os dois**, não só volume.

Como ADR-0001 estabeleceu YouTube como autoridade vertical (não aquisição rápida), a escolha de formato precisa servir esse propósito.

## Alternativas consideradas

1. **Shorts e long-form em paralelo, com cadências independentes**
   - Prós: máxima exploração das duas engines; mais oportunidades de descoberta
   - Contras: dispersão de energia do founder solo; risco real de Shorts trap; gerenciar 2 fluxos de produção paralelos é inviável solo nos primeiros 6 meses
2. **Apenas long-form, sem Shorts**
   - Prós: foco total; sem risco de fragmentar audiência
   - Contras: deixa de capturar a engine de descoberta de Shorts (que tem alcance gigante)
3. **Long-form primário, Shorts apenas como recorte derivado do long-form** ← **escolhida**
   - Prós: respeita o foco do founder solo; Shorts servem como prévia que puxa para o long-form (com pinned comment); coerência tonal natural; aproveita re-uso de conteúdo já produzido
   - Contras: Shorts derivados podem ter performance inferior aos Shorts pensados nativamente; requer disciplina para não cair na tentação de fazer Shorts originais "fáceis"
4. **Apenas Shorts**
   - Prós: produção rápida; descoberta forte
   - Contras: contradiz ADR-0001 (autoridade vertical); ad revenue muito menor; sem ativo composto de SEO

## Decisão

**Formato primário do canal YouTube = long-form.** Shorts são **secundários e exclusivamente derivados** de long-forms publicados.

**Regras concretas:**

1. **Primeiros 6 meses do canal:** exclusivamente long-form, sem Shorts. Concentrar energia em estabelecer cadência consistente (1/semana) e aprender o que funciona em retenção/CTR.
2. **A partir do 7º mês (ou marco "10 long-forms publicados, o que vier antes"):** Shorts entram como recortes. Cada Short publicado deve:
   - Ser **extraído de um long-form já publicado** (não conteúdo original autônomo)
   - Ter **pinned comment linkando o long-form de origem**
   - Manter coerência tonal com o long-form (mesma voz, mesmo ritmo escalado)
3. **Cadência Shorts:** 2-3/semana máximo. Não exceder o ratio Shorts:long-form. Volume Shorts > Long-form aumenta risco de Shorts trap documentado.
4. **Proibido:** Shorts originais autônomos (sem long-form de origem) nos primeiros 12 meses. Após esse marco, reabrir discussão.

**Duração de long-form:**
- **Sweet spot geral:** 8-15min (equilíbrio retenção/monetização — mid-roll ads disponíveis a partir de 8min)
- **Deep-dives quando justificado:** 15-30min (engagement total alto na plataforma; 50% do engagement vem dessa faixa)
- **Não fazer:** vídeos <8min sem razão estrutural (perde mid-roll); >30min sem retenção comprovada

## Consequências

**O que vira mais fácil:**
- Foco mental do founder solo
- Decisão de produção rápida ("é Short? então é recorte de qual vídeo?")
- Coerência tonal natural entre formatos
- Reutilização de trabalho já feito (vídeo de 15min vira 3-5 Shorts derivados sem retrabalho)

**O que vira mais difícil:**
- Resistir à tentação de fazer Short "rápido" para postar quando a semana sumir
- Tolerar a sensação de "estar perdendo a engine de Shorts" nos primeiros 6 meses
- Disciplina de pinned comment em todo Short (se esquecer, vira ruído)

**O que precisa ser revisado se isso mudar:**
- Se um Short específico viralizar (>1M views) e gerar leads/conversões mensuráveis para Marca #1 → reabrir discussão sobre Shorts originais
- Se algoritmos voltarem a integrar (algo improvável dado o decoupling de 2025) → revisar
- Se aparecer founder BR no nosso nicho com tração comprovada via Shorts puros → reavaliar premissas

## Quando revisitar

- **Marco sugerido:** 12 meses após lançamento do canal, ou ao chegar em 10.000 subs (o que vier antes)
- **Trigger de dado:** se algum Short publicado gerar >100 leads/conversões mensuráveis para Marca #1
- **Princípio:** decisão atual = heurística informada pelo Shorts trap documentado. Manter flexibilidade conforme aprendizado real do canal mostrar o que funciona para nós especificamente.