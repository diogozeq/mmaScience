# Relatório Final — Luana Santos vs Karol Rosa

> **Autor:** Diogo Zequini — Cientista de Dados
>
> Este relatório analisa todas as lutas da Luana Santos e Karol Rosa no UFC. Toda os dados são processados com Python e algoritmos de Machine Learning para ajuste por qualidade de oponente.

---

## Sumário

1. [Melhores Ações para a Luana](#capítulo-1-melhores-ações-para-a-luana)
2. [O Que a Equipe da Karol Provavelmente Vai Planejar](#capítulo-2-o-que-a-equipe-da-karol-provavelmente-vai-planejar)
3. [Insights Ocultos — Luana Santos](#capítulo-3-insights-ocultos--luana-santos)
   - [Onde Ela É Extrema na Categoria](#onde-ela-é-extrema-na-categoria-peso-galomosca-feminino)
   - [Insights Positivos](#insights-positivos)
   - [Insights Negativos](#insights-negativos)
4. [Insights Ocultos — Karol Rosa](#capítulo-4-insights-ocultos--karol-rosa)
   - [Onde Ela É Extrema na Categoria](#onde-ela-é-extrema-na-categoria-peso-galo-feminino)
   - [Insights Positivos](#insights-positivos-1)
   - [Insights Negativos](#insights-negativos-1)
5. [Análise Subjetiva Luta a Luta — Luana Santos](#capítulo-5-análise-subjetiva-luta-a-luta--luana-santos)
6. [Análise Round a Round — Luana Santos](#capítulo-6-análise-round-a-round--luana-santos)
   - [Dados Frios — Médias por Round](#dados-frios--médias-por-round)
   - [Dados Frios — Variações Médias Round a Round](#dados-frios--variações-médias-round-a-round)
   - [Dados Frios — Distribuição de Alvos e Posições por Round](#dados-frios--distribuição-de-alvos-e-posições-por-round)
   - [Dados Frios — Detalhamento Luta a Luta](#dados-frios--detalhamento-luta-a-luta)
   - [Análise Técnica](#análise-técnica)
   - [Brechas e Insights](#brechas-e-insights)
   - [Visão de Coach](#visão-de-coach)
7. [Análise Round a Round — Karol Rosa](#capítulo-7-análise-round-a-round--karol-rosa)
8. [Perfil vs Média — Luana Santos](#capítulo-8-perfil-vs-média--luana-santos)
9. [Cruzamento de Dados Frios](#capítulo-9-cruzamento-de-dados-frios)

---

## Capítulo 1: Melhores Ações para a Luana

> Os capítulos 1 a 4 formam uma leitura contínua. O Cap 1 define o que fazer. O Cap 2 antecipa o que o outro lado vai fazer. Os Caps 3 e 4 mostram de qual luta vem cada conclusão, com o que era esperado, o que aconteceu e por quê.

Em ordem de importância:

1. **Tratar os rounds 1 e 2 como janela principal de vitória.** No R1, Luana conecta 4.8 sig./min com 60% de precisão e mantém 100% de defesa de queda. Das 5 vitórias dela no UFC, 3 terminaram antes do R3 e 2 foram decisões sustentadas por controle. No R3, o striking cai para 1.2/min, a precisão para 26% e a defesa de queda para 0%. Karol chegou ao fim em todas as 12 lutas no UFC. A janela mais limpa da Luana está no início da luta; se a luta avançar, ela precisa ganhar o round por controle, não por troca aberta.

2. **Buscar controle acima de 60% como gatilho para a finalização.** As duas finalizações da Luana no UFC vieram nas lutas em que ela mais controlou: Lisboa 80% e Agapova 69%. Croden ficou em 62% e Egger em 52%, mas as duas foram para decisão. O padrão é claro: queda precisa virar posição estável antes da finalização aparecer.

3. **Não aceitar troca em pé a média-curta distância.** Karol conecta 5.37 sig./min contra 2.34/min de Luana. O saldo da Karol é +0.63/min, enquanto o da Luana é -1.21/min. A precisão da Karol é 57% e o volume dela é o maior entre as adversárias que Luana enfrentou. Troca longa em pé deixa Karol somar round.

4. **Usar o wrestling para cortar o volume da Karol.** Luana é a 2ª do grupo do Peso Galo em controle médio, com 49% de controle médio. As oponentes conectam só 36% dos golpes contra ela, contra 48% da média geral. O plano precisa passar por queda, estabilização e controle de ritmo antes que Karol construa vantagem no volume.

5. **Proteger a defesa de queda no R3 como prioridade específica de camp.** Nos três rounds 3 que disputou, a defesa de queda foi 0% nos três. A amostra é pequena, mas o sinal é forte porque se repetiu em todas as lutas que chegaram lá. Se a luta entrar no R3 e Karol conseguir inverter ou quedar, Luana perde a zona onde costuma controlar a luta.

6. **Não perseguir troca em pé quando o saldo de striking virar contra.** O R2 e o R3 mostram saldo de striking negativo, com domínio de controle ainda positivo: 93% no R2 e 60% no R3. Nos rounds tardios, Luana precisa voltar para queda, grade e controle. Urgência em pé aumenta o volume da Karol e reduz o tempo para achar o takedown limpo.

---

## Capítulo 2: O Que a Equipe da Karol Provavelmente Vai Planejar

1. **Levar a luta ao R3 como objetivo primário de camp.** Karol chegou ao fim em 100% das 12 lutas no UFC, somando 36 rounds disputados. O R3 da Luana tem striking em 1.2/min e defesa de queda em 0% no recorte analisado. Para Karol, sobreviver aos dois primeiros rounds já coloca a luta no terreno onde o histórico da Luana fica mais vulnerável.

2. **Construir placar com volume de striking antes de buscar vantagem no grappling.** Karol é a 2ª do grupo do Peso Galo em golpes significativos conectados por minuto, com 5.37 sig./min. O saldo dela é +0.63/min e a precisão é 57%. Em 8 vitórias no UFC, todas foram por decisão. Cada round sem finalização da Luana alimenta o modo de luta da Karol.

3. **Defender o takedown para negar o eixo central do jogo da Luana.** Luana tem saldo de -1.21/min no striking e depende da queda para cortar o volume da adversária. Karol tem 72% de defesa de queda. Quando a primeira entrada da Luana falha e a luta fica em pé por tempo longo, Karol ganha espaço para trabalhar o volume.

4. **Explorar a saída de baixo quando o takedown entrar.** A queda da Luana só vira vantagem se ela estabilizar. Se Karol levantar, inverter ou forçar scramble, ela tira Luana da zona de controle e devolve a luta para pontuação em volume. A disputa depois da queda é o ponto de maior incerteza do encaixe.

5. **Usar os chutes nas pernas como ferramenta de distância nos rounds iniciais.** Karol é a 2ª do top 15 do Peso Galo em golpes nas pernas por minuto, com 1.69/min. Luana fica em 0.37/min e o ataque dela às pernas cai de 13% no R1 para 8% nos rounds seguintes. Chutar a perna cedo ajuda Karol a manter distância, atrasar a entrada de queda e cobrar esse desgaste nos rounds tardios.

---

## Capítulo 3: Insights Ocultos — Luana Santos

> Os dois capítulos anteriores definem os planos. A partir daqui, mostramos de onde vem cada conclusão: qual luta, o que era esperado, o que aconteceu e por quê. Recorte: 6 lutas UFC (5V–1 resultado negativo).

### Onde Ela É Extrema na Categoria (Peso Galo Feminino)

| Métrica | Valor Luana | Posição no grupo |
|---------|-------------|:-----------------:|
| Controle médio de luta | 49% | 2ª |
| Quedas aplicadas/5min | 0.70 | 3ª |
| Defesa de striking | 64% | 4ª |
| Tentativas de queda/5min | 1.53 | 5ª |
| Finalizações tentadas/15min | 1.17 | 2ª |
| Volume de striking | 2.34 sig./min | 15ª |
| Golpes no clinch/min | 0.26 | 14ª |

- Luana tem um perfil muito claro dentro do grupo do Peso Galo: 2ª em controle médio, 3ª em quedas aplicadas e 5ª em tentativas de queda. O jogo dela ganha valor quando a queda vira posição estável.
- O outro lado do perfil também aparece: 15ª em volume de striking e 14ª em golpes no clinch. Se a luta ficar longa em pé, ela entra no território onde Karol tem mais ferramenta.

---

### Insights Positivos

1. **vs Agapova: maior aceleração de finalização do recorte.** Luana tentou submissões a 0.87/min contra Agapova. Esse volume não aparece em nenhuma outra luta dela no UFC. A finalização no R1 veio porque ela chegou cedo em posição dominante e atacou antes da adversária organizar defesa.

2. **vs Lisboa e vs Agapova: controle acima de 60% abriu a finalização.** Lisboa ficou em 80% de controle para Luana. Agapova ficou em 69%. As duas lutas com controle mais alto foram também as duas finalizações dela no UFC.

3. **vs O'Neill: absorveu 83 golpes significativos sem ser derrubada — o queixo passou no teste de volume mais duro do recorte.** Volume consistente pelos 3 rounds: R1 3.20/min, R2 2.40/min, R3 2.60/min. Zero knockdowns sofridos em 83 golpes conectados por O'Neill, uma striker de alto volume na divisão. O motor físico aguentou os 15 minutos sem colapso.

---

### Insights Negativos

1. **vs Egger: defesa de queda 0% e vitória mesmo assim.** Egger completou a única queda que tentou. Luana venceu porque conseguiu controlar outros trechos da luta, mas o alerta fica para o R3: quando a adversária consegue passar pela defesa de queda, a resposta posicional da Luana ainda não aparece como padrão confiável.

2. **vs O'Neill: wrestling travado e striking em desvantagem.** O'Neill conectou 5.53/min contra 2.73/min de Luana. O saldo de -2.80/min foi o pior do recorte. Luana acertou 1 queda em 5 tentativas, bem abaixo da média de carreira de 62%. Quando queda e striking travam ao mesmo tempo, o plano fica estreito.

3. **Segunda metade da carreira UFC: 2V–1 resultado negativo sem explicação causal clara no recorte.** Primeira metade: 3V–0D (100%). Segunda metade: 2V–1 resultado negativo (67%). As adversárias mais recentes (Lisboa, Croden) não são, em tese, as mais difíceis da carreira. A tendência ainda não tem explicação clara nos dados disponíveis — pode ser variação normal da amostra, pode ser acúmulo de informação sobre o perfil dela.

4. **R3 nas três lutas que chegaram até lá: defesa de queda 0% e striking em 1.2/min.** Luana ainda tenta buscar o wrestling nos rounds tardios, mas a defesa de queda cai no mesmo trecho. Contra Karol, esse desequilíbrio pesa porque qualquer perda de posição no R3 devolve a luta para volume e placar.

---

## Capítulo 4: Insights Ocultos — Karol Rosa

> Mesma lógica do capítulo anterior, agora pelo lado da Karol. Recorte de carreira no UFC: 12 lutas (8V–4D). Os dados abaixo mostram o que a equipe dela deve tentar usar contra a Luana.

### Onde Ela É Extrema na Categoria (Peso Galo Feminino)

| Métrica | Valor Karol | Posição |
|---------|-------------|---------|
| Golpes significativos/min | 5.37 | 2ª no grupo |
| Golpes nas pernas/min | 1.69 | 2ª no grupo |
| Golpes no chão/min | 0.56 | 5ª no grupo |
| Defesa de queda | 72% | 8ª no grupo |
| Vitórias por decisão no UFC | 8 de 8 vitórias | 100% |
| Finalizações aplicadas no UFC | 0 em 8 vitórias | sem finalização no UFC |

- Karol é a 2ª do grupo em volume de golpes significativos e a 2ª em golpes nas pernas. A equipe dela deve querer uma luta longa, com distância aberta e pontuação acumulada.
- A defesa de queda de 72% é boa o suficiente para obrigar Luana a preparar entrada. Queda forçada, sem estabilizar depois, dá tempo para Karol levantar e voltar para o volume.

---

### Insights Positivos

1. **UFC completo: 100% das lutas chegaram ao limite.** Em 12 lutas no UFC, nenhuma foi interrompida antes do tempo. São 8 vitórias e 4 derrotas, todas por decisão. Com 5.37 sig./min, Karol soma round com volume e mantém esse padrão mesmo contra níveis diferentes de oposição.

2. **Saída de baixo como ponto de atenção pós-queda.** Karol não precisa vencer o wrestling inteiro para atrapalhar Luana. Basta levantar, inverter ou travar a estabilização depois da queda. Contra uma Luana que depende de controle para finalizar, a primeira defesa depois do takedown vale tanto quanto a defesa da entrada.

---

### Insights Negativos

1. **Nenhuma finalização no UFC em 8 vitórias.** Karol tem 0.05 tentativa de finalização por 5min, contra 0.40 da Luana. Quando ela entra no grappling, o uso mais provável é posicionamento, grade, controle curto e pontuação.

2. **Defesa de queda de 72% contra a 5ª maior frequência de tentativas da categoria.** Luana tenta 1.53 quedas por 5min, quase o dobro da Karol, que fica em 0.81. Para Karol, defender uma entrada isolada não resolve a luta inteira. Ela vai precisar repetir defesa, giro e saída de grade durante vários minutos.

---

## Capítulo 5: Análise Subjetiva Luta a Luta — Luana Santos

> Recorte luta a luta. Os números que embasam os insights dos Capítulos 3 e 4.

### Médias de Carreira

| Métrica | Média dela |
|---------|:---------:|
| Golpes Sig. Conectados/min | 2.34 |
| Golpes Sig. Absorvidos/min | 3.55 |
| Precisão Striking | 56% |
| Defesa Striking | 64% |
| Quedas Aplicadas/15min | 2.57 |
| Precisão Quedas | 62% |
| Defesa de Quedas | 80% |
| Tentativas de Sub/15min | 1.17 |

> Esses são os números normais dela. Nos bullets de cada luta, mostramos onde ela saiu desse padrão.

---

### Resumo do Recorte

- Recorte geral do relatório: 6 lutas no UFC (5 vitórias + 1 derrota)
- Período: 09/12/2023 a 13/12/2025
- Neste capítulo subjetivo detalhado: 5 lutas com dados completos de lutadora + oponente
- A vitória sobre Juliana Miller entra nos consolidados e na análise round a round, mas fica fora deste capítulo por ter perfil estatístico muito fora do padrão
- Nota: 2 das 5 lutas foram disputadas em Peso Mosca (vs Agapova e vs Casey O'Neill) — Luana compete normalmente em Peso Galo

---

### Vitórias Recentes

#### 1. vs Melissa Croden — UFC Fight Night: Royval vs. Kape (13/12/2025)
**Decisão | R3 5:00 | Peso Galo**

##### Dados Objetivos

| Métrica | Luana Santos | Melissa Croden |
|---------|:-----------:|:--------------:|
| Sig Strikes Conectados | 12 | 22 |
| Sig Strikes Tentados | 24 | 74 |
| Precisão (%) | 50% | 30% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 3/7 | 0/1 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 9:21 | 0:44 |
| Controle (%) | 62% | 5% |

##### Pontos Positivos

- 9:21 de controle em 15 minutos de luta — 62% do tempo total. Três quedas distribuídas nos 3 rounds, defesa da Croden nula (0/1). O wrestling foi o motor da vitória, não o striking.
- Defesa de 70%, acima dos 64% de média: a Croden conectou 22 em 74 tentativas (30% de precisão) e, das poucas que passaram, a maioria veio no R2 quando Luana abriu mão do striking. Absorveu pouco em termos absolutos — 1.47/min, bem abaixo dos 3.55/min que costuma levar.

##### Pontos Negativos

- Striking colapsou progressivamente ao longo dos rounds: R1 10/13 (77%) → R2 2/8 (25%) → R3 0/3 (0%). No terceiro round, zero sig strikes conectados com 3 tentativas. O volume total de 0.80/min é 66% abaixo da média dela de 2.34/min — a maior diferença negativa das últimas 5 lutas.
- Saldo de striking negativo de -0.67/min. Croden conectou mais por minuto (1.47/min vs 0.80/min de Luana). Numa luta de decisão em que o wrestling segurou, funciona — mas o padrão de striking que some nos rounds finais é recorrente nos dados recentes.

---

#### 2. vs Tainara Lisboa — UFC Fight Night: Burns vs. Morales (17/05/2025)
**Finalização | R2 4:59 | Peso Galo**

##### Dados Objetivos

| Métrica | Luana Santos | Tainara Lisboa |
|---------|:-----------:|:--------------:|
| Sig Strikes Conectados | 15 | 6 |
| Sig Strikes Tentados | 19 | 34 |
| Precisão (%) | 79% | 18% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 2/2 | 0/1 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 7:57 | 0:00 |
| Controle (%) | 80% | 0% |

##### Pontos Positivos

- 79% de precisão com 19 tentativas — 23 pontos acima da média de 56%. Alta precisão e alto controle na mesma luta raramente aparecem juntos; aqui vieram combinados com finalização no R2. A Lisboa ficou com 0 controle e 18% de precisão no striking — domínio em todas as dimensões.
- 2/2 nas quedas (100% vs 62% de média), 80% de controle do tempo total: o grappling funcionou do início ao fim, sem espaço para a Lisboa se organizar no pé.

##### Pontos Negativos

- Volume de 1.50/min, 36% abaixo da média de 2.34/min. Nas últimas três lutas em que venceu por decisão ou grappling, o slpm ficou abaixo do normal (0.80 vs Croden, 1.50 vs Lisboa, 0.6 vs Agapova). É possível que o plano de luta priorize o wrestling — mas o padrão de striking baixo vale monitorar, especialmente contra lutadoras que defendem bem o takedown.

---

#### 3. vs Mariya Agapova — UFC Fight Night: Namajunas vs. Cortez (13/07/2024)
**Finalização | R1 3:27 | Peso Mosca**

##### Dados Objetivos

| Métrica | Luana Santos | Mariya Agapova |
|---------|:-----------:|:--------------:|
| Sig Strikes Conectados | 2 | 3 |
| Sig Strikes Tentados | 4 | 14 |
| Precisão (%) | 50% | 21% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/1 | 0/0 |
| Tentativas de Sub | 3 | 0 |
| Controle (tempo) | 2:23 | 0:00 |
| Controle (%) | 69% | 0% |

*(Luta curta: 3:27. Os números desta luta são sinais direcionais — amostra pequena demais pra consolidar padrão.)*

##### Pontos Positivos

- 3 tentativas de finalização em 3:27 de luta — equivale a 13.04/15min contra uma média de 1.17/15min dela. A pressão no chão foi imediata e constante; conseguiu a queda, manteve controle e foi atrás da finalização sem esperar estabilizar. É uma das maiores densidades de sub attempts que ela registrou.
- Defesa de 79% (Agapova conectou 3 em 14 tentativas): mesmo iniciando e gerenciando a fase de finalização, manteve o nível de defesa acima da média de 64%.

##### Pontos Negativos

- Luta finalizada em R1 com amostra limitada — não é possível extrair padrões de comportamento por rounds ou tendências de cardio. O que fica de Agapova é que a pressão de finalização funcionou; sobre Luana, esta luta confirma mais do que revela.

---

#### 4. vs Stephanie Egger — UFC Fight Night: Song vs. Gutierrez (09/12/2023)
**Decisão | R3 5:00 | Peso Galo**

##### Dados Objetivos

| Métrica | Luana Santos | Stephanie Egger |
|---------|:-----------:|:---------------:|
| Sig Strikes Conectados | 53 | 44 |
| Sig Strikes Tentados | 104 | 115 |
| Precisão (%) | 51% | 38% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 2/4 | 1/1 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 7:44 | 1:06 |
| Controle (%) | 52% | 7% |

##### Pontos Positivos

- 3.53/min de sig strikes conectados — 51% acima da média de 2.34/min, sem abrir mão da precisão (51% vs 56% de média). Essa é a luta em que chegou mais perto de combinar volume e acerto ao mesmo tempo. Melhor round no R2: 5.60/min, a maior taxa de striking de todo o recorte.
- Distribuição de golpes ao corpo foi de 42% nessa luta (22/53 sig conectados) contra 23% de média de carreira. Mudou o alvo de forma consistente ao longo dos 3 rounds — especialmente no R1 e R2 — o que provavelmente abriu a cabeça da Egger nos momentos críticos.

##### Pontos Negativos

- Queda brusca do R2 para o R3: 5.60/min → 1.00/min. Uma redução de 82% no volume de striking no último round. A Egger subiu para 2.20/min no R3 e conseguiu completar uma queda. Luana ganhou o R3 no controle (2:42), não no striking — o mesmo padrão da luta contra a Croden.
- Quedas: 2/4 (50%) vs 62% de média — abaixo, e a Egger completou a única tentativa que fez (1/1). Numa luta decidida no striking, o wrestling menos preciso não custou caro; contra uma grappler melhor, custaria.

---

### Derrotas Recentes

#### 1. vs Casey O'Neill — UFC 305: Du Plessis vs. Adesanya (17/08/2024)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Luana Santos | Casey O'Neill |
|---------|:-----------:|:-------------:|
| Sig Strikes Conectados | 41 | 83 |
| Sig Strikes Tentados | 97 | 193 |
| Precisão (%) | 42% | 43% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/5 | 0/2 |
| Tentativas de Sub | 0 | 1 |
| Controle (tempo) | 2:21 | 2:21 |
| Controle (%) | 16% | 16% |

##### Pontos Negativos

- O'Neill conectou 5.53/min contra 2.73/min de Luana — saldo de -2.80/min, o pior do recorte. A diferença não foi de precisão (43% vs 42%), foi volume puro: O'Neill tentou 193 golpes significativos, quase o dobro dos 97 de Luana. Tentar acompanhar na troca sem aumentar o volume era uma equação que não fechava.
- Takedowns: 1/5 (20%) vs 62% de média — a alternativa ao striking estava bloqueada. A saída mais óbvia para sair de uma desvantagem de volume era derrubar e controlar; nas 5 tentativas de queda, só 1 completou. Com o wrestling travado e o striking em desvantagem, não havia segunda opção.
- Precisão de 42% com 97 tentativas — 14 pontos abaixo da média de 56%. Com O'Neill atiçando 193 tentativas, Luana estava reagindo ao ritmo da adversária em vez de impor o dela. Essa combinação de volume alto com precisão abaixo do normal aparece tipicamente quando o atleta está sendo pressionado a responder, não a construir.

##### Pontos Positivos

- Volume consistente pelos 3 rounds sem colapsar: R1 3.20/min, R2 2.40/min, R3 2.60/min. Não abandonou o striking nem desmoronou fisicamente — o motor aguentou os 15 minutos contra a striker mais pesada que enfrentou até então.
- Zero knockdowns sofridos em 83 golpes conectados por O'Neill. O'Neill é uma striker de alto volume na divisão — Luana absorveu volume alto sem ceder a sequência que poderia encerrar a luta. O queixo passou no teste de volume mais duro do recorte.

---

## Capítulo 6: Análise Round a Round — Luana Santos

> Como Luana se comporta em cada round — volume, precisão, grappling e onde o equilíbrio da luta muda de dono.

### Perfil Geral

- Total de lutas analisadas: 6
- Categorias: Peso Galo (4 lutas), Peso Mosca (2 lutas)
- Resultado geral: 5V–1D–0Emp (nos dados disponíveis)
- Vitórias por método: 2 Decisão, 1 KO/TKO, 2 Finalização
- Derrotas por método: 1 Decisão
- Empates: 0
- Lutas com dados de rounds 3: 3 lutas (vs Melissa Croden, vs Casey O'Neill, vs Stephanie Egger)

---

### Dados Frios — Médias por Round

| Métrica | R1 (n=6) | R2 (n=4) | R3 (n=3) |
|---------|:--------:|:--------:|:--------:|
| **Striking** | | | |
| Golpes sig. conectados/min | 4.8 | 2.4 | 1.2 |
| Golpes sig. tentados/min | 8.4 | 4.7 | 3.2 |
| Precisão (%) | 60% | 50% | 26% |
| Knockdowns/5min | 0.0 | 0.0 | 0.0 |
| **Grappling** | | | |
| Quedas/5min | 0.6 | 1.0 | 0.7 |
| Tentativas de queda/5min | 1.1 | 2.3 | 1.3 |
| Precisão de queda (%) | 58% | 56% | 50% |
| Tentativas de finalização/5min | 0.7 | 0.5 | 0.0 |
| Defesa de queda (%) | 100% | 100% | 0% |
| **Controle** | | | |
| Controle (%) | 45% | 57% | 43% |
| **Oponente** | | | |
| Golpes sig. oponente/min | 2.9 | 2.8 | 3.3 |
| Precisão oponente (%) | 31% | 34% | 35% |
| **Saldos** | | | |
| Saldo de striking/min | +1.9 | –0.4 | –2.1 |
| Saldo de quedas/5min | +0.6 | +1.0 | +0.3 |
| Dominância de striking (%) | 56% | 48% | 20% |
| Dominância de controle (%) | 86% | 93% | 60% |

*Amostra pequena em R3 (n=3). O dado de defesa de queda 0% no R3 vem das lutas que chegaram ao terceiro round — qualquer conclusão aqui é direcional, não consolidada.*

---

### Dados Frios — Variações Médias Round a Round

| Métrica | R1→R2 (n=4) | R2→R3 (n=3) |
|---------|:-----------:|:-----------:|
| Golpes sig. conectados/min | –0.4 | –1.6 |
| Golpes sig. tentados/min | –0.5 | –2.5 |
| Precisão (%) | –13% | –16% |
| Quedas/5min | +0.5 | –0.3 |
| Tentativas de queda/5min | +1.0 | –1.3 |
| Precisão de queda (%) | +22% | +8% |
| Tentativas de finalização/5min | +0.5 | –0.3 |
| Controle (%) | +10% | –5% |
| Alvos: cabeça (%) | +12% | +16% |
| Alvos: corpo (%) | –2% | –7% |
| Alvos: pernas (%) | –10% | –9% |
| Posição: distância (%) | –2% | –6% |
| Posição: clinch (%) | –6% | +6% |
| Saldo de striking/min | –0.7 | –1.3 |
| Saldo de quedas/5min | +0.5 | –0.7 |
| Dominância de controle (%) | +11% | –20% |

---

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos (%)

| Alvo | R1 (n=6) | R2 (n=4) | R3 (n=3) |
|------|:--------:|:--------:|:--------:|
| Cabeça | 61% | 62% | 65% |
| Corpo | 25% | 30% | 28% |
| Pernas | 13% | 8% | 8% |
| **Oponente — Cabeça** | 45% | 58% | 60% |
| **Oponente — Corpo** | 31% | 10% | 24% |
| **Oponente — Pernas** | 23% | 32% | 16% |

#### Posição (%)

| Posição | R1 (n=6) | R2 (n=4) | R3 (n=3) |
|---------|:--------:|:--------:|:--------:|
| Distância | 92% | 90% | 90% |
| Clinch | 8% | 2% | 10% |
| Chão | 0% | 8% | 0% |

---

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Categoria | Resultado | Método | Rounds | Sig./min | Precisão | Saldo/min | Controle % |
|------|----------|-----------|-----------|--------|:------:|:--------:|:--------:|:---------:|:----------:|
| 12/08/2023 | Juliana Miller | Mosca | **V** | KO/TKO | R1 | 17.1 | 60% | +10.6 | 12% |
| 09/12/2023 | Stephanie Egger | Galo | **V** | Decisão | R3 | 3.5 | 51% | +0.6 | 52% |
| 13/07/2024 | Mariya Agapova | Mosca | **V** | Finalização | R1 | 0.6 | 50% | –0.3 | 69% |
| 17/08/2024 | Casey O'Neill | Mosca | **D** | Decisão | R3 | 2.7 | 42% | –2.8 | 16% |
| 17/05/2025 | Tainara Lisboa | Galo | **V** | Finalização | R2 | 1.5 | 79% | +0.9 | 80% |
| 13/12/2025 | Melissa Croden | Galo | **V** | Decisão | R3 | 0.8 | 50% | –0.7 | 62% |

*A luta contra Juliana Miller (17.1 sig./min, +10.6 saldo) fica fora do padrão. Todas as outras lutas ficaram entre 0.6 e 3.5 sig./min. O KO em menos de 4 minutos infla os números de striking daquele confronto.*

---

### Análise Técnica

- O volume de striking cai a cada round: 4.8 sig./min no R1, 2.4 no R2 e 1.2 no R3. As quedas por 5min aumentam do R1 para o R2. Luana migra o peso da luta para controle conforme os rounds avançam.

- A precisão de striking cai de 60% no R1 para 26% no R3, junto com a queda de tentativas. A leitura mais útil para o camp é simples: se o striking começa a perder volume e precisão, o round precisa voltar para queda, grade e controle.

- A distribuição de alvos se concentra na cabeça ao longo dos rounds: 61% no R1, 62% no R2, 65% no R3. O ataque às pernas começa em 13% no R1 e cai para 8% nos rounds seguintes. Esse alvo precisa aparecer mais se a ideia for tirar base da Karol antes da entrada.

- A defesa de queda é 100% nos R1 e R2 (n=6 e n=4 respectivamente), mas cai para 0% no R3 (n=3). Amostra pequena para o R3, mas o padrão é consistente com as lutas que chegaram lá: nas três lutas com R3, Luana não defendeu nenhuma queda no terceiro round.

- O saldo de striking vai de +1.9/min no R1 para –0.4 no R2 e –2.1 no R3. A dominância de controle se mantém positiva nos três rounds: 86%, 93% e 60%. Quando a trocação entra no negativo, o controle ainda sustenta o caminho de vitória.

---

### Brechas e Insights

**1.** Precisão de striking cai 13% do R1 para o R2, e o volume também cai 0.4/min. Menos tentativa com menos precisão indica perda de produção em pé, não seletividade.

**2.** Dominância de controle sobe para 93% no R2, o pico da luta em controle. O saldo de striking no mesmo round já é negativo, em –0.4/min. Luana ganha esse trecho no chão enquanto perde a troca em pé.

**3.** Defesa de queda 100% nos R1-R2 e 0% no R3 (n=3). Quando Luana chega ao terceiro round, a resistência ao takedown cai no recorte disponível. As lutas onde isso aconteceu foram sustentadas por controle e finalização anteriores.

---

### Visão do Analista

#### Se eu fosse da equipe adversária:

- Forçar a luta até o R3. Luana cai para 1.2 sig./min no terceiro round e aparece com 0% de defesa de queda no recorte. Karol deve tentar sobreviver aos dois primeiros rounds e cobrar esse trecho final.

- No R1, evitar gastar energia em queda forçada. A defesa de queda da Luana nos primeiros rounds é 100% nas 6 lutas. O R2 abre mais troca posicional porque Luana começa a tentar mais quedas.

- Atacar as pernas nos rounds iniciais. Karol é a 2ª do top 15 em golpes nas pernas por minuto, com 1.69/min. Luana cai para 8% de ataques às pernas a partir do R2, então a resposta dela nesse alvo tende a diminuir.

- Manter o striking no R2 mesmo depois de ser derrubada. O controle da Luana no R2 chega a 57% em média, mas o volume dela nesse round cai para 2.4 sig./min. Se Karol levantar rápido ou bater na saída, ela mantém o round vivo para os juízes.

- Priorizar o clinch no R3. A posição de clinch sobe para 10% no terceiro round, contra 2% no R2. Dominar a grade nesse trecho ataca justamente o round onde a defesa de queda da Luana caiu.

#### Se eu fosse da equipe da Luana:

- Resolver a luta no R1 ou R2, ou chegar ao R3 já com controle acumulado. No recorte completo de 6 lutas no UFC, Luana tem 5 vitórias, e 3 delas terminaram antes do terceiro round: KO contra Juliana Miller e finalizações contra Agapova e Lisboa. As decisões contra Egger e Croden só funcionaram porque o controle compensou a queda de striking nos rounds tardios. O R3 é o trecho de maior risco.

- Trabalhar defesa de queda nos rounds tardios como prioridade de camp. Nos R3 analisados, a defesa caiu para 0%. Pode ser cansaço, posicionamento ou ajuste adversário, mas o padrão está no vídeo e Karol pode mirar isso.

- Manter o ataque às pernas durante toda a luta. Luana mira pernas em 13% dos golpes no R1 e cai para 8% depois. Contra Karol, esse alvo ajuda a tirar base antes da entrada de queda e reduz a fluidez do volume em pé.

- Usar o clinch como transição para grappling desde o R1. O controle de 45% no R1 já é alto e chega a 57% no R2. Antecipar essa pressão evita que Karol tenha minutos limpos para acumular striking.

- Nos rounds onde o saldo de striking for negativo, cortar a troca em pé e voltar para o chão. O R2 e R3 mostram saldo de striking negativo, com dominância de controle positiva nos mesmos rounds. Luana precisa transformar esses minutos em queda, grade e estabilização.

---

## Capítulo 7: Análise Round a Round — Karol Rosa

> Como Karol cresce por round, onde ela soma placar e quais janelas a Luana precisa atacar antes da luta entrar no ritmo dela.

### Perfil Geral

- Total de lutas analisadas: 12
- Categoria: Peso Galo feminino
- Resultado geral: 8V–4D
- Vitórias por método: 8 decisões
- Derrotas por método: 4 decisões
- Todas as 12 lutas chegaram ao R3

---

### Dados Frios — Médias por Round

| Métrica | R1 (n=12) | R2 (n=12) | R3 (n=12) |
|---------|:---------:|:---------:|:---------:|
| **Striking** | | | |
| Golpes sig. conectados/min | 5.0 | 6.0 | 6.6 |
| Tentativas sig./min | 9.6 | 10.4 | 11.6 |
| Precisão (%) | 55% | 58% | 59% |
| **Grappling** | | | |
| Quedas/5min | 0.3 | 0.4 | 0.5 |
| Tentativas de queda/5min | 0.5 | 0.5 | 1.4 |
| Precisão de queda (%) | 50% | 80% | 37% |
| Tentativas de finalização/5min | 0.0 | 0.2 | 0.0 |
| Defesa de queda (%) | 44% | 83% | 76% |
| **Controle** | | | |
| Controle (%) | 18% | 34% | 36% |
| Dominância de controle (%) | 48% | 68% | 77% |
| **Saldos** | | | |
| Saldo de striking/min | +0.4 | +1.7 | +1.8 |
| Saldo de quedas/5min | 0.0 | +0.3 | +0.3 |
| Dominância de striking (%) | 51% | 61% | 60% |

---

### Dados Frios — Variações Round a Round

| Métrica | R1→R2 (n=12) | R2→R3 (n=12) |
|---------|:------------:|:------------:|
| Golpes sig. conectados/min | +1.0 | +0.6 |
| Tentativas sig./min | +0.8 | +1.2 |
| Precisão (%) | +3% | +1% |
| Tentativas de queda/5min | 0.0 | +0.9 |
| Precisão de queda (%) | +38% | -47% |
| Controle (%) | +17% | +2% |
| Saldo de striking/min | +1.3 | +0.1 |
| Saldo de controle (%) | +19% | +6% |

---

### Dados Frios — Alvos e Posições por Round

#### Alvos da Karol (%)

| Alvo | R1 (n=12) | R2 (n=12) | R3 (n=12) |
|------|:---------:|:---------:|:---------:|
| Cabeça | 48% | 64% | 65% |
| Corpo | 18% | 15% | 15% |
| Pernas | 34% | 21% | 20% |

#### Posições da Karol (%)

| Posição | R1 (n=12) | R2 (n=12) | R3 (n=12) |
|---------|:---------:|:---------:|:---------:|
| Distância | 82% | 61% | 64% |
| Clinch | 12% | 13% | 20% |
| Chão | 6% | 26% | 16% |

---

### Análise Técnica

- Karol cresce round a round no striking: 5.0 sig./min no R1, 6.0 no R2 e 6.6 no R3. A precisão também sobe, de 55% para 59%. Ela aumenta volume sem perder limpeza.

- O salto mais perigoso para Luana está do R1 para o R2. O saldo de striking da Karol sai de +0.4/min para +1.7/min, enquanto o controle sobe de 18% para 34%. Se Luana não travar o ritmo cedo, Karol começa a somar placar no segundo round.

- O R1 é a melhor janela para atacar a defesa de queda da Karol. A defesa dela fica em 44% no primeiro round e sobe para 83% no R2 e 76% no R3. A entrada da Luana precisa aparecer cedo, antes de Karol ajustar distância e timing.

- Karol usa a perna como preparação no R1: 34% dos golpes dela vão nesse alvo. Depois, ela migra para cabeça: 64% no R2 e 65% no R3. A Luana precisa responder aos chutes baixos sem abrir troca longa de mão.

- No R3, Karol tenta mais quedas: 1.4 tentativas/5min, contra 0.5 nos dois rounds anteriores. A precisão cai para 37%, mas o clinch sobe para 20% e a dominância de controle chega a 77%. Mesmo quando a queda não entra limpa, ela usa corpo a corpo para prender e pontuar.

---

### Brechas e Insights

**1.** O R1 é o round menos dominante da Karol. O saldo de striking fica em +0.4/min e a dominância de controle em 48%. É a janela mais limpa para Luana entrar na queda antes da luta virar volume acumulado.

**2.** A defesa de queda da Karol melhora muito depois do primeiro round. 44% no R1, 83% no R2 e 76% no R3. Se Luana esperar demais para testar a queda, enfrenta a versão mais ajustada da Karol.

**3.** O R2 é onde Karol mais conecta striking com controle. O saldo de striking sobe para +1.7/min e o chão aparece em 26% das posições. Se Luana perder o R2 em volume e posição, o R3 começa com Karol no tipo de luta que ela mais conhece.

**4.** O R3 da Karol é forte em controle, mas menos limpo nas quedas. Ela tenta quase 3x mais quedas que no R2, com precisão caindo de 80% para 37%. Luana pode punir essas entradas se mantiver base, underhook e saída de grade.

---

### Visão do Analista

#### Para a equipe da Luana:

- Atacar Karol no R1 com entrada de queda preparada. A defesa de queda dela é 44% nesse round, bem abaixo dos 83% do R2. É a melhor janela para Luana transformar o começo da luta em controle.

- Não deixar o R2 virar round de estabilização da Karol. Ela sobe para +1.7/min no saldo de striking e 34% de controle. Se esse round fica confortável para Karol, o placar começa a sair da mão.

- Responder aos chutes baixos sem aceitar troca longa. Karol usa 34% dos golpes nas pernas no R1 para preparar distância. A resposta precisa ser checagem, passo para fora, entrada na grade ou queda.

- No R3, defender a grade antes da queda. Karol aumenta tentativas de queda e clinch nesse round, mas a precisão cai. Se Luana vencer underhook e sair do corpo a corpo, ela corta a parte mais produtiva do R3 da Karol.

#### O que a equipe da Karol deve querer:

- Passar pelo R1 sem ceder controle longo. A defesa de queda da Karol é pior no primeiro round, então sobreviver sem ficar presa por minutos já muda a luta para o trecho onde ela melhora.

- Acelerar no R2. Karol cresce para 6.0 sig./min, +1.7/min de saldo e 34% de controle nesse round. É o primeiro momento em que o volume dela começa a pesar de verdade no placar.

- Usar chutes baixos no começo e migrar para cabeça depois. O padrão dela é 34% de golpes nas pernas no R1 e 64% na cabeça no R2. Se Luana não quebrar essa sequência, Karol organiza distância e depois aumenta o volume.

- No R3, prender na grade mesmo sem completar a queda. A precisão de queda cai para 37%, mas o clinch sobe para 20% e a dominância de controle chega a 77%. Para Karol, controlar o corpo pode valer mais que insistir na queda limpa.

---

## Capítulo 8: Perfil vs Média — Luana Santos

> Luana no contexto do top 15 do Peso Galo feminino — o grupo que a Karol Rosa também integra (9ª colocada). Os números dos capítulos anteriores ganham escala aqui.

**Categoria:** Peso Galo
**Gênero:** Feminino
**Grupo de comparação:** top15 (16 lutadores)
**Data da análise:** 2026-05-01

---

### Grupo de Comparação

| # | Lutador |
|---|---------|
| Campeão | Kayla Harrison |
| 1 | Julianna Peña |
| 2 | Raquel Pennington |
| 3 | Norma Dumont |
| 4 | Ketlen Vieira |
| 5 | Yana Santos |
| 6 | Irene Aldana |
| 7 | Ailin Perez |
| 8 | Macy Chiasson |
| 9 | Karol Rosa |
| 10 | Jacqueline Cavalcanti |
| 11 | Mayra Bueno Silva |
| 12 | Nora Cornolle |
| 13 | Miesha Tate |
| 14 | Joselyne Edwards |
| 15 | Luana Santos **(analisado)** |

---

### Pontos Mais Fortes no Grupo (1 métrica)

| Métrica | Valor | Média do Grupo | Posição | n |
|---------|------:|---------------:|----------:|--:|
| Finalizações tentadas/15min | 1.17 | 0.36 | 2ª | 16 |

Luana Santos é a 2ª do grupo em finalizações tentadas por 15 minutos, com 1.17 contra 0.36 da média do grupo. O número vem da cadeia principal do jogo dela: 62% de precisão nas quedas, 49% de controle médio e 0.70 queda aplicada por 5min. Ela derruba, mantém posição e caça a finalização.

---

### Acima da Média (42 métricas)

- **Derrotas**: 1, contra média de 3.88 no grupo
- **Derrotas por KO/TKO**: 0, contra média de 0.56
- **Derrotas por finalização**: 0, contra média de 0.56
- **Derrotas por KO/TKO (%)**: 0%, contra média de 10%
- **Derrotas por finalização (%)**: 0%, contra média de 14%
- *+37 métricas adicionais acima da média do grupo*

Luana Santos chega ao UFC com 5-1 e a única derrota foi por decisão. Em 6 lutas no UFC, não sofreu nocaute nem finalização. A taxa de sobrevivência em derrota está em 100%, contra 68% do grupo. Esse dado importa se a luta for para os juízes: ela é difícil de tirar da luta, mesmo quando perde minutos em pé.

---

### Abaixo da Média (43 métricas)

- **Golpes significativos conectados/min**: 2.34, 15ª do grupo
- **Saldo de striking/min**: -1.21, 14ª do grupo
- **Golpes no clinch/min**: 0.26, 14ª do grupo
- **Golpes no chão/min**: 0.03, 14ª do grupo
- **Golpes nas pernas/min**: 0.37, 12ª do grupo
- *+38 métricas adicionais abaixo da média do grupo*

O histórico curto explica parte dos totais, mas não explica o saldo de striking. -1.21 por minuto significa que Luana absorve mais do que conecta em pé, enquanto o grupo está em +0.72 na média. Ela ainda vence com esse perfil porque leva a luta para queda e controle antes que o déficit em pé vire dano acumulado.

---

### Métricas Neutras — Perfil (10 métricas)

- **Golpes em pé**: 89% dos golpes dela
- **Perfil de distância**: 0.78, acima da média do grupo de 0.37
- **Estilo equilibrado**: 0.17, abaixo da média de 0.45
- **Tempo médio de luta**: 69% da duração prevista, abaixo da média de 84%
- **Carreira no UFC**: 50%, perto da média do grupo de 55%
- *+5 métricas adicionais de perfil*

O par 89% dos golpes em pé + perfil de distância 0.78 mostra como Luana costuma chegar no grappling: ela trabalha à distância, cria ângulo e entra na queda. O estilo equilibrado em 0.17 confirma uma atleta especializada. Quando o takedown não entra, o plano B em pé ainda precisa de desenvolvimento.

---

### Resumo Quantitativo

| Classificação | Qtd | % |
|---------------|----:|--:|
| Pontos fortes de elite | 1 | 1% |
| Acima da Média | 42 | 41% |
| Na Média | 6 | 6% |
| Abaixo da Média | 43 | 42% |
| Métricas Neutras (Perfil) | 10 | 10% |
| **Total** | **102** | **100%** |

**1% em faixa de elite. 41% acima da média. 42% abaixo.**

Luana Santos é finalizadora de controle com exposição no striking e nos rounds tardios. A finalização depende do controle anterior. Contra Karol, que tem 29% de controle médio na carreira e 72% de defesa de queda, o acesso ao chão precisa ser construído com entrada limpa e estabilização.

---

## Capítulo 9: Cruzamento de Dados Frios

> Dados brutos lado a lado. O comparativo direto que sustenta toda a análise anterior.

### Ficha Técnica

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| Categoria | Peso Galo | Peso Galo | - |
| Postura | Destro | Destro | - |
| Ranking Categoria | 15 🔴 | 9 🟢 | **Karol Rosa** |
| Ranking PFP | Desranqueado | Desranqueado | - |
| Idade (anos) | 25 🟢 | 31 🔴 | **Luana Santos** |
| Altura (cm) | 168 🟢 | 165 🔴 | **Luana Santos** |
| Envergadura (cm) | 170 🔴 | 171 🟢 | **Karol Rosa** |
| Alcance Extra (cm) | 2 🔴 | 6 🟢 | **Karol Rosa** |

---

### Carreira Geral

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| Total de Lutas | 12 🔴 | 26 🟢 | **Karol Rosa** |
| Vitórias | 10 🔴 | 19 🟢 | **Karol Rosa** |
| Derrotas | 2 | 7 | - |
| Empates | 0 | 0 | Empate |
| Sequência de Vitórias Atual | 2 🟢 | 1 🔴 | **Luana Santos** |
| Taxa de Vitória Geral | 83% 🟢 | 73% 🔴 | **Luana Santos** |
| Vitórias por KO/TKO | 1 🔴 | 4 🟢 | **Karol Rosa** |
| Vitórias por Finalização | 5 🟢 | 2 🔴 | **Luana Santos** |
| Vitórias por Decisão | 4 🔴 | 13 🟢 | **Karol Rosa** |
| Vitórias no 1º Round | 4 🟢 | 0 🔴 | **Luana Santos** |
| Derrotas por KO/TKO | 0 | 0 | Empate |
| Derrotas por Finalização | 0 | 2 | - |
| Derrotas por Decisão | 2 | 5 | - |
| Tempo Médio de Luta | 10:21 | 15:00 | - |
| Taxa de Vitória no R1 | 20% 🟢 | 0% 🔴 | **Luana Santos** |

---

### Carreira no UFC

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| Lutas no UFC | 6 🔴 | 12 🟢 | **Karol Rosa** |
| Vitórias no UFC | 5 🔴 | 8 🟢 | **Karol Rosa** |
| Derrotas no UFC | 1 | 4 | - |
| Empates no UFC | 0 | 0 | Empate |
| No Contests no UFC | 0 | 0 | Empate |
| Vitórias KO/TKO no UFC | 1 🟢 | 0 🔴 | **Luana Santos** |
| Vitórias Finalização no UFC | 2 🟢 | 0 🔴 | **Luana Santos** |
| Vitórias Decisão no UFC | 2 🔴 | 8 🟢 | **Karol Rosa** |
| Derrotas KO/TKO no UFC | 0 | 0 | Empate |
| Derrotas Finalização no UFC | 0 | 0 | Empate |
| Derrotas Decisão no UFC | 1 | 4 | - |
| Tempo Total Lutado no UFC (min) | 62 🔴 | 180 🟢 | **Karol Rosa** |
| % Carreira no UFC | 50% 🟢 | 46% 🔴 | **Luana Santos** |

---

### Striking

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| Golpes Sig. Conectados/min | 2.34 🔴 | 5.37 🟢 | **Karol Rosa** |
| Golpes Sig. Absorvidos/min | 3.55 🟢 | 4.74 🔴 | **Luana Santos** |
| Precisão de Striking | 56% 🔴 | 57% 🟢 | **Karol Rosa** |
| Defesa de Striking | 64% 🟢 | 50% 🔴 | **Luana Santos** |
| Saldo de Striking/min | -1.21 🔴 | 0.63 🟢 | **Karol Rosa** |
| Knockdowns Causados/5min | 0.00 🔴 | 0.05 🟢 | **Karol Rosa** |
| Knockdowns Sofridos/5min | 0.00 🟢 | 0.05 🔴 | **Luana Santos** |
| Golpes p/ Nocautear | 145 | sem dado | - |
| Golpes p/ Ser Nocauteado | sem dado | sem dado | - |
| Golpes Em Pé/min | 2.70 🔴 | 4.71 🟢 | **Karol Rosa** |
| Golpes Clinche/min | 0.26 🔴 | 0.62 🟢 | **Karol Rosa** |
| Golpes Solo/min | 0.03 🔴 | 0.56 🟢 | **Karol Rosa** |

---

### Distribuição de Striking

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| % Golpes na Cabeça | 65% | 59% | - |
| % Golpes no Corpo | 23% | 16% | - |
| % Golpes nas Pernas | 12% | 26% | - |
| % Golpes Em Pé | 89% | 71% | - |
| % Golpes Clinche | 8% | 16% | - |
| % Golpes Solo | 3% | 13% | - |
| Golpes Cabeça/min | 1.75 | 3.44 | - |
| Golpes Corpo/min | 0.87 | 0.75 | - |
| Golpes Pernas/min | 0.37 | 1.69 | - |

---

### Grappling

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| Precisão de Quedas | 62% 🟢 | 45% 🔴 | **Luana Santos** |
| Defesa de Quedas | 80% 🟢 | 72% 🔴 | **Luana Santos** |
| Quedas Aplicadas/5min | 0.70 🟢 | 0.40 🔴 | **Luana Santos** |
| Quedas Sofridas/5min | 0.10 🟢 | 0.20 🔴 | **Luana Santos** |
| Tentativas de Queda/5min | 1.53 🟢 | 0.81 🔴 | **Luana Santos** |
| Tentativas Finalização Causadas/5min | 0.40 🟢 | 0.05 🔴 | **Luana Santos** |
| Tentativas Finalização Sofridas/5min | 0.10 🔴 | 0.00 🟢 | **Karol Rosa** |
| % Controle Médio | 49% 🟢 | 29% 🔴 | **Luana Santos** |

---

### Indicadores Compostos

| Dado | Luana Santos | Karol Rosa | Vantagem |
|------|:------------:|:----------:|:--------:|
| Resiliência ao Nocaute | 0.77 🔴 | 0.89 🟢 | **Karol Rosa** |
| DNA Estilo Equilibrado | 0.17 | 0.44 | - |
| Perfil Distância de Luta | 0.78 | 0.42 | - |
| Intervalo Médio entre Lutas (dias) | 170.80 | 196.64 | - |
| % Luta Lutada Médio | 69% | 100% | - |

---

> **Legenda:** 🟢 Vantagem | 🔴 Desvantagem | Empate = valores idênticos | - = sem dado ou sem vantagem direta
