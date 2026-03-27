# Relatório Final — Carlos Prates vs Jack Della Maddalena

> **Autor:** Diogo Zequini — Cientista de Dados
> 
> Este relatório analisa 7 lutas de Carlos Prates e 9 lutas de Jack Della Maddalena no UFC (2022-2025), com base em dados de UFC Stats, UFC.com e Tapology, processados com Python e algoritmos de Machine Learning para ajuste por qualidade de oponente.

## Sumário

1.  [Melhores Ações para o Prates](#capitulo-1-resumo-final)
2.  [O Que a Equipe do Jack Provavelmente Vai Planejar](#capitulo-2-inteligencia-adversaria)
3.  [Insights Ocultos — Carlos Prates](#capitulo-3-insights-ocultos--carlos-prates)
4.  [Insights Ocultos — Jack Della Maddalena](#capitulo-4-insights-ocultos--jack-della-maddalena)
5.  [Análise Subjetiva Luta a Luta — Carlos Prates](#capitulo-5-analise-subjetiva--carlos-prates)
    -   [Médias de Carreira](#prates-sub-medias-de-carreira)
    -   [Resumo do Recorte](#prates-sub-resumo-do-recorte)
    -   [Vitórias Recentes](#prates-sub-vitorias-recentes)
    -   [Derrotas Recentes](#prates-sub-derrotas-recentes)
6.  [Análise Subjetiva Luta a Luta — Jack Della Maddalena](#capitulo-6-analise-subjetiva--jack-della-maddalena)
    -   [Médias de Carreira](#medias-de-carreira)
    -   [Resumo do Recorte](#resumo-do-recorte)
    -   [Vitórias Recentes](#vitorias-recentes)
    -   [Derrotas Recentes](#derrotas-recentes)
7.  [Análise Round a Round — Carlos Prates](#capitulo-7-analise-round-a-round--carlos-prates)
    -   [Perfil Geral](#perfil-geral)
    -   [Dados Frios — Médias por Round](#dados-frios----medias-por-round)
    -   [Dados Frios — Variações Médias Round a Round](#dados-frios----variacoes-medias-round-a-round)
    -   [Dados Frios — Distribuição de Alvos e Posições por Round](#dados-frios----distribuicao-de-alvos-e-posicoes-por-round)
    -   [Dados Frios — Detalhamento Luta a Luta](#dados-frios----detalhamento-luta-a-luta)
    -   [Análise Técnica](#analise-tecnica)
    -   [Brechas e Insights](#brechas-e-insights)
8.  [Análise Round a Round — Jack Della Maddalena](#capitulo-8-analise-round-a-round--jack-della-maddalena)
    -   [Perfil Geral](#jdm-rar-perfil-geral)
    -   [Dados Frios — Médias por Round](#jdm-rar-medias-por-round)
    -   [Dados Frios — Variações Médias Round a Round](#jdm-rar-variacoes)
    -   [Dados Frios — Distribuição de Alvos e Posições](#jdm-rar-alvos-posicoes)
    -   [Dados Frios — Detalhamento Luta a Luta](#jdm-rar-detalhamento)
    -   [Análise Técnica](#jdm-rar-analise-tecnica)
    -   [Brechas e Insights](#jdm-rar-brechas)
9.  [Cruzamento de Dados Frios](#capitulo-9-cruzamento-de-dados)
    -   [Ficha Técnica](#ficha-tecnica)
    -   [Carreira Geral](#carreira-geral)
    -   [Carreira no UFC](#carreira-no-ufc)
    -   [Striking](#striking)
    -   [Grappling](#grappling)
    -   [Índices Compostos](#indices-compostos)

---

## Capítulo 1: Melhores Ações para o Prates

> Os capítulos 1 a 4 formam uma leitura contínua. O Cap 1 define o que fazer. O Cap 2 antecipa o que o outro lado vai fazer. Os Caps 3 e 4 mostram de qual luta vem cada conclusão, com o que era esperado, o que aconteceu e por quê.

Em ordem de importância:

1.  **Tratar os rounds 1 e 2 como janela principal de vitória.** Todos os 9 knockdowns do Prates no UFC aconteceram nos R1 e R2. 81% do volume ofensivo dele (191 de 235 golpes sig.) se concentra nesses dois rounds, e a precisão média por round sobe de 53% no R1 para 61% no R2. O Jack nunca foi nocauteado no UFC, mas os adversários que enfrentou tinham poder de nocaute consistentemente abaixo da mediana da divisão. A janela existe e é muito favorável, mas a partir do terceiro essa vantagem inverte para o JDM.
    
2.  **Proteger o corpo como prioridade defensiva.** O ataque ao corpo que o Jack faz é sistemático: 71% de precisão (147 acertos em 207 tentativas), com desvios positivos em 3 lutas: vs Roberts 4x acima do padrão, vs Emeev 3.2x, vs Holland 2.7x. Esse é um dos caminhos mais consistentes para o Jack construir vantagem, principalmente a partir do R3, pelo Prates ter uma aceitação de 62% dos golpes tentados nessa região.
    
3.  **Variar os alvos desde cedo, em vez de caçar só a cabeça.** Nas vitórias: 38% cabeça, 29% corpo, 32% pernas. Na derrota: 54% cabeça, pernas em 14%, precisão na cabeça caindo para 39%. O Jack tem 63% de defesa bruta na cabeça (4ª da divisão), atacar concentrado ali é jogar no ponto mais forte dele. 
    
4.  **Tratar o chute de pernas como arma específica contra este adversário.** O JDM absorve chutes de pernas 4.02x acima do padrão histórico de quem o enfrentou. Exemplos de casos que não eram pra ter acontecido: Holland entregou 35 (vs média de 10.56 em outras lutas), Makhachev entregou 10 (vs média de 1.36) e Rodriguez entregou 7 (vs média de 1.00). Combinados: 52 conectados contra 12.92 esperados. Nessas 3 lutas, o JDM devolveu apenas 25, tomou 2.08x mais do que entregou contra caras que não são referência nisso.
    
5.  **Não aceitar uma luta limpa em média-curta, com trocas longas e ritmo contínuo.** O Jack conecta 5.57 sig./min contra 3.77 do Prates, saldo +1.73/min vs -0.76/min. A precisão dele é real, não inflada pelos oponentes, confirmado nas lutas contra adversários com defesa acima da média. O Garry parou o Prates com pressão posicional e volume, sem nocaute. O Jack também tem essa capacidade mas com striking muito superior. Cada troca longa e contínua na média distância é um round que funciona para o jogo do JDM.
    
6.  **Ganhar a luta no impacto, não na contagem.** Nas 6 vitórias, o Prates absorveu 5.5 sig./min com saldo positivo. Na derrota contra Garry absorveu menos (4.9/min) e perdeu. O diferencial do Prates não é volume: é potência no momento certo. Cada round que vira disputa de pontos é um round onde esse diferencial não existe e o do Jack sim.
    
7.  **Usar clinch e grappling apenas como recurso pontual de quebra de ritmo.** O Prates usa quase nada do clinch no UFC. O Jack não usa clinch de forma linear: escala nos rounds finais. Vs Hafez, 1 clinch shot no R1 e 10 no R3; vs Belal, 1 no R1 e 8 no R5. A média do R1 (2.1) esconde o pico tardio (4.0 no R5), com 77% de eficiência. O risco real do clinch aparece no R3+, não no início.
    
8.  **Se a luta alongar, trocar urgência por disciplina.** O Prates tem 0 vitórias por decisão no UFC (100% foram KO/TKO). O Jack tem 4/9 por decisão. A única luta longa (vs Garry, 25 min): saldo de -2.52 sig./min, 0 knockdowns. Nesse cenário, o caminho deixa de ser forçar o KO e passa a ser negar volume e aguardar o erro.
    

---

## Capítulo 2: O que provavelmente a equipe do JDM planejou

1.  **Corpo como ponto de entrada, não variação tática.** Em três lutas distintas, JDM atacou o corpo 2.7x a 4x acima do padrão esperado para aquele oponente.  O efeito sobre o Prates tem duas camadas: a direta, que é a aceitação de 62% dos golpes tentados nessa região; e a indireta, que é o cotovelo baixando para defender o fígado exatamente no momento em que a cabeça fica exposta. Isso precisa ser reconhecido e respondido desde o R1.
    
2.  **Volume vai parecer controlado no R1 e dobrar no R3 e diante.** Vs Belal: 5.6 sig./min no R1, 10.6/min no R5. Vs Hafez: 2.6/min no R1, 8.6/min no R3. O padrão não é explosão de oportunidade: o JDM chega em cada round com mais volume acumulado do anterior. O problema específico para o Prates é que essa curva de aceleração cruza a janela onde ele tenta fechar a luta. No R1 o JDM vai parecer administrável. No R2, a diferença de ritmo já está instalada, e o Prates ainda não fechou.
    
3.  **O plano não depende de um nocaute,** **o do Prates provavelmente sim.** JDM precisa em média de 146 golpes significativos para nocautear; o Prates precisa de 43. São mecanismos opostos: acúmulo progressivo de dano versus timing único de alto impacto. O JDM ganhou por decisão, por finalização e por KO tardio. O Prates ganhou todas as 7 lutas no UFC por KO/TKO, com 0 vitórias por decisão. Quanto mais a luta avança sem um nocaute, mais o cenário favorece o modo de operar do JDM e mais o Prates está em território sem histórico positivo.
    
4.  Queda no R3 como reset de posicionamento, não busca de finalização. JDM usa 5% de controle real na carreira porque o striking resolve antes. Mas a lógica muda no R3: a defesa de queda do Prates caiu de 87% (R1) para 33% (R3) nos dados disponíveis, e os oponentes que percebem isso escalam as tentativas. Uma queda ou até tentativa no R3/R4 contra um Prates desgastado não precisa finalizar para ser efetiva: muda o posicionamento, consome o tempo que o Prates precisaria para encontrar o timing, e abre golpes de corpo na sequência do levantamento. (improvável mas achei melhor mapear)
    

---

## Capítulo 3: Insights Ocultos — Carlos Prates

> Os dois capítulos anteriores definem os planos. A partir daqui, mostramos de onde vem cada conclusão: qual luta, o que era esperado, o que aconteceu e por quê. Recorte: 7 lutas UFC (6V-1D).

### Insights Positivos

1.  **vs Giles: virou o plano de ataque de cabeça para baixo e nocauteou.** O padrão de carreira do Prates é 54% dos golpes na cabeça. Contra Giles, inverteu para 8% cabeça e 49% corpo. O esperado era uma luta na média distância buscando a cabeça. O que aconteceu: saiu completamente do padrão e encontrou o KO no R2. O motivo provável é que leu o adversário e mudou no meio da luta, o que indica capacidade de adaptação tática real, não dependência de um único plano.
    
2.  **vs Edwards: maior concentração de chutes baixos da carreira, seguida de KO.** Média de carreira em pernas: 25-30%. Contra Edwards: 52%, a mais alta de qualquer luta registrada. O esperado era que mantivesse o padrão de distribuição habitual. O que aconteceu: priorizou pernas de forma inédita e nocauteou no R2. Junto com Giles (item anterior), forma um padrão: as duas maiores vitórias vieram dos dois maiores desvios do plano habitual.
    
3.  **vs Edwards (R1): maior desvantagem posicional da carreira, sem efeito no round seguinte.** No R1, tomou saldo de queda negativo e ficou mais tempo no chão do que em qualquer outra luta. O esperado era que isso afetasse o ritmo ofensivo. O que aconteceu: encontrou o KO em 88 segundos no R2. O dado importa porque mostra que pressão de grappling no R1 não necessariamente compromete o poder de finalização do Prates no round seguinte.
    
4.  **vs Magny: defesa de queda sob pressão máxima de wrestling.** Magny tentou 7 quedas, a maior insistência de wrestling que o Prates enfrentou. O esperado era que pelo menos 2-3 conectassem, dado o volume. O que aconteceu: 95% de defesa. Os oponentes tentam quedas 87% acima da média contra ele, como se soubessem que precisam tirar dos pés. Quase ninguém consegue enquanto ele está fresco.
    
5.  **vs todos os oponentes: a defesa de striking é melhor do que o 47% sugere.** O número bruto (47%) parece fraco. O esperado é que isso indicasse defesa ruim. O que os dados mostram: os adversários do Prates (Neal, Edwards, Garry, Li Jingliang) são strikers acima da média da divisão, muito melhor do que o JDM enfrentou em striking, o que deprime o número artificialmente. Quando se ajusta pela qualidade de quem o atacou, a defesa real sobe muito. 47% é um número contra um elenco difícil, não contra a média.
    

---

### Insights Negativos

1.  **vs todas as vitórias: a precisão de 55% é um pouco inflada.** O esperado ao ver 55% de precisão é que o Prates acerte bem. O que os dados mostram: os adversários dele cedem precisão para quase todos que lutaram. O Prates está entre os que mais se beneficiam desse efeito, top1-4 do UFC. Contra adversários com defesa real (como o JDM provou ser no Cap 4), esse inflador desaparece.
    
2.  **vs Garry (25 min): único teste longo, e tudo piorou.** O esperado para um atleta com 6 KOs em 7 lutas era que mantivesse o ritmo mesmo em luta longa. O que aconteceu: queda de ritmo 2.4x acima do esperado (-2.14/min vs -0.88 esperado), volume 33% abaixo da média de carreira, 0 knockdowns. Foram 63 golpes conectados em 5 rounds contra média de 29 nas vitórias. O volume alto apareceu justamente quando estava perdendo.
    
3.  **vs Garry (R3-R5): defesa de queda colapsou e os oponentes leram isso em tempo real.** No R1, a defesa de queda foi 87%. No R3, caiu para 33%. O esperado era que a defesa se mantivesse estável. O que aconteceu: as tentativas de queda dos adversários subiram de 2/5min no R1 para 7/5min no R4, como se percebessem a queda. A resposta defensiva não acompanhou. Dado de 1 luta, mas o padrão dentro dessa luta é progressivo e consistente. 
    
4.  **vs histórico de chutes baixos: o volume contra o JDM pode cair por hábito.** O esperado ao ver o volume de chutes baixos do Prates é que ele entregue isso contra qualquer um. O que os dados mostram: os adversários históricos dele defendem pouco esse ataque, inflando o número. O JDM é genuinamente vulnerável (52 chutes absorvidos de Holland, Makhachev e Rodriguez), mas o risco é o Prates não comprometer o volume necessário porque nunca precisou forçar.
    

---

## Capítulo 4: Insights Ocultos — Jack Della Maddalena

> Mesma lógica do capítulo anterior, agora pelo lado do JDM. Recorte: 9 lutas UFC (8V-1D).

### Insights Positivos

1.  **vs Holland: 55% de precisão e volume dobrado contra quem defende de verdade.** Holland tem defesa de striking acima da média da divisão e tentou 356 golpes. O esperado era que o JDM conectasse menos e fosse forçado a desacelerar sob essa pressão. O que aconteceu: manteve 55% de precisão (igual à média de carreira) e dobrou o volume esperado. O dado importa porque é o teste mais duro de precisão que existe no currículo dele.
    
2.  **vs Burns: produziu no chão mesmo ficando por baixo.** Burns derrubou o JDM 7 vezes em 11 tentativas e controlou 37% do tempo. O esperado era que o JDM fosse neutralizado no solo. O que aconteceu: produziu 16 golpes no chão (24% do volume da luta) mesmo ficando por baixo, e venceu. O dado revela um recurso que ele quase nunca precisa usar (5% de controle de carreira) porque o striking resolve antes, mas que existe quando necessário.
    
3.  **vs Belal (5 rounds): eficiência mantida do R1 ao R5.** Belal é referência em cardio e volume. O esperado era que o ritmo do JDM caísse na segunda metade. O que aconteceu: manteve eficiência em todos os 5 rounds, utilizando 63% do tempo de luta (vs ~50% da divisão). Junto com Holland (volume extremo) e Burns (pressão de grappling), são três formatos diferentes de adversidade onde o cardio técnico se confirmou.
    
4.  **vs Emeev: nocauteou adversário com histórico baixo de knockdown em 2.5 minutos.** Emeev absorvia poucos knockdowns contra outros oponentes. O esperado era uma luta mais longa, sem KO precoce. O que aconteceu: 1 knockdown e nocaute antes de completar o R1. O dado importa porque mostra que o poder de finalização do JDM funciona mesmo contra adversários que normalmente não caem.
    
5.  **vs Roberts, Emeev e Holland: ataque ao corpo com desvios de 2.7x a 4x acima do esperado.** Em três lutas com adversários de estilos diferentes, o volume ao corpo ficou muito acima do que esses oponentes recebem de outros rivais. Vs Roberts: 4x acima do esperado. Vs Emeev: 3.2x. Vs Holland: 2.7x. O esperado era que o ataque ao corpo variasse com o estilo do oponente. O que os dados mostram: é o plano A independente de quem está na frente, e é de onde vem a recomendação defensiva do Cap 1.
    

---

### Insights Negativos

1.  **vs Makhachev: defesa de queda zerou e o striking sumiu junto.** Média de carreira em defesa de queda: 64%. Contra Makhachev: 0% (4 em 4 tentativas convertidas). O esperado era que resistisse pelo menos parcialmente. O que aconteceu: volume ofensivo caiu para 0.72 sig/min contra média de 5.57/min. O padrão é binário: quando a defesa de queda colapsa (Burns: 36%, 7 em 11), o striking colapsa junto. Quando sustenta (Hafez: 85%, Holland: 100%), o JDM opera normal.
    
2.  **vs todos os oponentes com poder de KO: nenhum testou de verdade.** O JDM nunca foi nocauteado em 27 rounds no UFC. O esperado é que isso indicasse queixo resistente. Seus adversários são abaixo da mediana da divisão em poder de knockdown. Nenhum se aproxima do Prates nesse atributo. Os 27 rounds são reais, mas calculados contra um elenco que quase não tinha poder de nocaute.
    
3.  **vs Pete Rodriguez: zero chutes baixos quando o esperado era 16%.** O mapa de alvos do JDM é cabeça + corpo. O esperado era que variasse pelo menos um pouco com chutes nas pernas. O que aconteceu: 0% de chutes baixos contra Rodriguez, num contexto onde 16% era o padrão da divisão. 
    
4.  **vs todos os oponentes: a defesa de 63% é produto mais do elenco do que do JDM:** O esperado ao ver 63% de defesa de striking é que o JDM defenda bem só que é inflado pela capacidade contra quem ele lutou. Ajustado pela qualidade real dos atacantes, a defesa cai de forma expressiva. É o espelho exato do que acontece com a precisão do Prates (Cap 3): os dois têm um número-chave que parece forte na superfície e enfraquece quando se olha quem estava do outro lado.
    

---

## Capítulo 5: Análise Subjetiva Luta a Luta — Carlos Prates

> Gerado em 26/03/2026 | Últimas 4 vitórias e 1 derrota analisadas

### Médias de Carreira

| Métrica | Média dele |
| --- | :-: |
| Golpes Sig. Conectados/min | 3.77 |
| Golpes Sig. Absorvidos/min | 4.53 |
| Precisão Striking | 55% |
| Defesa Striking | 47% |
| Knockdowns/15min | 2.13 |
| Quedas Aplicadas/15min | 0.21 |
| Precisão de Quedas | 100% |
| Defesa de Quedas | 80% |
| Tentativas de Sub/15min | 0.0 |

> Esses são os números normais dele. Nos bullets de cada luta, mostramos onde ele saiu desse padrão.

---

### Resumo do Recorte

-   Lutas analisadas: 5 (4 vitórias + 1 derrota)
-   Período: 17/08/2024 a 15/11/2025
-   Dados detalhados (lutador + oponente) disponíveis em todas as 5 lutas

---

### Vitórias Recentes

#### 1\. vs Leon Edwards — UFC 322: Della Maddalena vs. Makhachev (15/11/2025)

**KO/TKO | R2 1:28 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Prates | Edwards |
| --- | :-: | :-: |
| Sig Strikes Conectados | 21 | 12 |
| Sig Strikes Tentados | 32 | 17 |
| Precisão (%) | 66% | 71% |
| Knockdowns | 1 | 0 |
| Quedas Aplicadas | 0/0 | 2/3 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:01 | 3:00 |
| Controle (%) | 0% | 46% |

##### Pontos Positivos

-   No R2 foi um outro lutador: saiu de 53% de precisão no R1 para 80% em apenas 88 segundos — a aceleração de golpes significativos por minuto foi de 1.80 para 8.18. Não é só pressão, é leitura de timing.
-   Fez 52% dos golpes significativos nas pernas — bem acima do perfil normal dele, que é majoritariamente cabeça e corpo. A mudança de alvo funcionou como distração antes do combo finalizador no R2.
-   Conseguiu 66% de precisão geral contra um dos defensores mais sólidos do octógono, superando a sua própria média de carreira de 55% numa luta em que tomou knockdown two-leg takedowns.

##### Pontos Negativos

-   Ficou 3 minutos inteiros sob controle de Edwards no R1 sem conseguir se levantar — e isso com 0 segundos de controle no final da luta. Quando está no chão, o volume ofensivo dele some quase por completo.
-   Absorveu 2 quedas de Edwards com apenas 3 tentativas. A defesa de quedas média dele é 80%, aqui foi 33%. Sinal de que quando o oponente insiste no takedown no momento certo — pós-troca — a guarda dele abre.

---

#### 2\. vs Geoff Neal — UFC 319: Du Plessis vs. Chimaev (16/08/2025)

**KO/TKO | R1 4:59 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Prates | Neal |
| --- | :-: | :-: |
| Sig Strikes Conectados | 32 | 25 |
| Sig Strikes Tentados | 60 | 49 |
| Precisão (%) | 53% | 51% |
| Knockdowns | 1 | 0 |
| Quedas Aplicadas | 0/0 | 0/1 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:00 | 0:15 |
| Controle (%) | 0% | 5% |

##### Pontos Positivos

-   6.42 golpes significativos por minuto — quase o dobro da média dele de 3.77/min — numa luta que durou praticamente o round inteiro. Não foi explosão de 30 segundos; sustentou volume alto por quase 5 minutos.
-   Defesa de quedas de 100%: Neal tentou 1 queda, não concluiu. Importante porque Neal costuma usar o clinche para desequilibrar.
-   53% de precisão com 60 tentativas em 5 minutos sem descanso — na mesma faixa da sua média de 55%, mas com volume muito acima. O equilíbrio entre quantidade e acerto foi melhor do que o padrão sugeria.

##### Pontos Negativos

-   Tomou 25 golpes significativos de Neal em quase 5 minutos completos — absorveu 5.02/min, bem acima dos 4.53/min que é a média de carreira dele. Em troca de soco, Neal é perigoso e Prates ficou exposto por mais tempo do que o habitual nas vitórias.
-   Precisão de 53% — embora parecida com a média — esconde que ele tentou 60 golpes para conectar 32. Em lutas mais longas isso pode se transformar em gás desnecessário.

---

#### 3\. vs Neil Magny — UFC Fight Night: Magny vs. Prates (09/11/2024)

**KO/TKO | R1 4:50 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Prates | Magny |
| --- | :-: | :-: |
| Sig Strikes Conectados | 12 | 10 |
| Sig Strikes Tentados | 21 | 20 |
| Precisão (%) | 57% | 50% |
| Knockdowns | 2 | 0 |
| Quedas Aplicadas | 1/1 | 0/7 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 1:09 | 1:31 |
| Controle (%) | 24% | 31% |

##### Pontos Positivos

-   2 knockdowns em um único round com apenas 12 golpes conectados — um knockdown a cada 6 golpes. A média de carreira é 2.13 knockdowns a cada 15 minutos; aqui ele atingiu isso em menos de 5 minutos.
-   100% de aproveitamento nas quedas (1/1) — raro para o perfil dele, que praticamente não usa o grappling. Quando levou, usou o tempo no chão pra somar controle e golpes no solo, que representaram 17% dos golpes dessa luta.
-   Magny tentou 7 quedas e não completou nenhuma. Prates defendeu tudo isso mantendo o jogo em pé, onde ele é mais perigoso.

##### Pontos Negativos

-   Volume muito baixo para o padrão dele: 2.48 golpes significativos por minuto, contra a média de 3.77/min. A luta foi curta e terminou bem, mas o ritmo estava abaixo — pode ser estratégia ou pode ser dificuldade de abrir Magny no início.
-   Ficou 1:31 sob controle de Magny — mais tempo do que ele ficou no controle. Em volume total de strikes foi próximo (12 x 10), mas a dinâmica positional esteve mais favorável ao adversário que o placar final sugere.

---

#### 4\. vs Li Jingliang — UFC 305: Du Plessis vs. Adesanya (17/08/2024)

**KO/TKO | R2 4:02 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Prates | Jingliang |
| --- | :-: | :-: |
| Sig Strikes Conectados | 55 | 41 |
| Sig Strikes Tentados | 84 | 111 |
| Precisão (%) | 65% | 37% |
| Knockdowns | 3 | 0 |
| Quedas Aplicadas | 0/0 | 0/0 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:04 | 0:23 |
| Controle (%) | 1% | 4% |

##### Pontos Positivos

-   3 knockdowns em 2 rounds — o melhor desempenho de knockdowns no recorte. No R1 já tinha 1 knockdown com 69% de precisão, e escalou no R2 para 63% com 2 knockdowns adicionais em 4 minutos. Cada vez que levantou a intensidade, o resultado apareceu imediatamente.
-   65% de precisão com 84 tentativas — 10 pontos acima da média de carreira de 55% e com volume alto. Esses dois fatores juntos raramente aparecem ao mesmo tempo.
-   Jingliang tentou 111 golpes e conectou 41 — 37% de precisão. Prates com 6.09 golpes/min (acima da sua média de 3.77/min) e saldo de +1.55/min favorável — desempenho acima do padrão de carreira na troca em pé.

##### Pontos Negativos

-   80% dos golpes do Prates foram na cabeça nessa luta — muito acima do perfil usual dele. Quando o oponente decifra o padrão (que aqui não aconteceu porque a luta acabou cedo), a concentração de volume num alvo só vira vulnerabilidade.
-   Nenhum volume de grappling em ambos os lados, mas Jingliang chegou a 23 segundos de controle. Prates respondeu com apenas 4 segundos — quando acaba no chão, a dimensão de controle some completamente.

---

### Derrotas Recentes

#### 1\. vs Ian Machado Garry — UFC Fight Night: Machado Garry vs. Prates (26/04/2025)

**Decisão | R5 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Prates | Garry |
| --- | :-: | :-: |
| Sig Strikes Conectados | 63 | 126 |
| Sig Strikes Tentados | 129 | 242 |
| Precisão (%) | 49% | 52% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 0/0 | 4/19 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 1:46 | 3:09 |
| Controle (%) | 7% | 13% |

##### Pontos Positivos

-   No R5 chegou a 4.40 golpes/min e 58% de precisão — os melhores números da luta. Mesmo perdendo nos rounds anteriores, o motor físico ainda estava rodando no último round: 22 golpes conectados em 5 minutos, com 61 segundos de controle.
-   49% de precisão ao longo de 25 minutos é apenas 6 pontos abaixo da média dele. Não foi desmoronamento técnico — foi volume insuficiente diante de quem jogou no pontual acumulado durante todos os rounds.

##### Pontos Negativos

-   Garry conectou o dobro de golpes: 126 x 63. A diferença não foi de precisão — foi de volume. Prates tentou 129 e Garry tentou 242. Quando a luta vai a distância, quem dita o quanto de ação acontece vence o placar, e Prates nunca conseguiu mudar esse ritmo.
-   A defesa de quedas virou o fator decisivo: Garry tentou 19 quedas e completou 4 — 21% de aproveitamento, mas acumulou controle rounds seguidos. A média de defesa de quedas de Prates é 80%; aqui foi 79%, próximo ao normal, mas Garry simplesmente insistiu até completar 4 vezes.
-   19% dos golpes significativos de Prates vieram do chão — o perfil mais alto de ground-and-pound no recorte, mas no contexto errado: ele estava embaixo sendo controlado, não dominando. Os 12 golpes no solo saíram de posição de desvantagem.
-   2.52 golpes significativos por minuto ao longo de 25 minutos — 33% abaixo da média de carreira de 3.77/min. Em cada round tentou mais do que conectou, e nunca conseguiu a sequência que geralmente precede suas finalizações rápidas.

---

## Capítulo 6: Análise Subjetiva Luta a Luta — Jack Della Maddalena

> Gerado em 26/03/2026 | Últimas 4 vitórias e 1 derrota analisadas

### Médias de Carreira

| Métrica | Média dele |
| --- | :-: |
| Golpes Sig. Conectados/min | 5.57 |
| Golpes Sig. Absorvidos/min | 3.84 |
| Precisão Striking | 51% |
| Defesa Striking | 63% |
| Quedas Aplicadas/15min | 0.13 |
| Defesa de Quedas | 64% |
| Tentativas de Sub/15min | 0.1 |

> Esses são os números normais dele. Nos bullets de cada luta, mostramos onde ele saiu desse padrão.

---

### Resumo do Recorte

-   Lutas analisadas: 5 (4 vitórias + 1 derrota)
-   Período: 15/07/2023 a 15/11/2025
-   Dados detalhados (lutador + oponente) disponíveis em 5 de 5 lutas

---

### Vitórias Recentes

#### 1\. vs Belal Muhammad — UFC 315: Muhammad vs. Della Maddalena (10/05/2025)

**Decisão | R5 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Jack Della Maddalena | Belal Muhammad |
| --- | :-: | :-: |
| Sig Strikes Conectados | 178 | 132 |
| Sig Strikes Tentados | 342 | 318 |
| Precisão (%) | 52% | 42% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 0/3 | 3/9 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:40 | 3:21 |
| Controle (%) | 3% | 13% |

##### Pontos Positivos

-   Volume 28% acima da média dele (7.12/min vs 5.57/min de carreira) e a precisão se manteve em 52% — exatamente no padrão normal. Mais agressivo sem abrir a guarda, o que não é comum nele.
-   No R5 conectou 53 golpes em 5 minutos (10.6/min) — mais que o dobro da média dos R1 a R4 da mesma luta. Aceleração consistente com o padrão documentado em outras lutas longas.
-   Defesa de quedas de 67% numa luta onde o Belal tentou 9 quedas — acima da média de carreira dele (64%). Segurou o chão contra o grappler mais insistente da categoria.

##### Pontos Negativos

-   Controle de 3% com desvantagem de 3min21s para o oponente. Pelo perfil de Belal, era esperado perder o controle de quadra, mas o JDM ficou passivo demais no chão — levou 3 quedas sem resposta.
-   Defesa de striking caiu 5 pontos em relação à média (58% vs 63%). Num nocaute não chegou, mas no acumulado de 25 minutos a queda na defesa pesou nos scorecards.

---

#### 2\. vs Gilbert Burns — UFC 299: O'Malley vs. Vera 2 (09/03/2024)

**KO/TKO | R3 3:43 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Jack Della Maddalena | Gilbert Burns |
| --- | :-: | :-: |
| Sig Strikes Conectados | 67 | 27 |
| Sig Strikes Tentados | 123 | 58 |
| Precisão (%) | 54% | 47% |
| Knockdowns | 1 | 0 |
| Quedas Aplicadas | 0/1 | 7/11 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:16 | 5:07 |
| Controle (%) | 2% | 37% |

##### Pontos Positivos

-   Conectou 16 golpes no chão de 67 totais (24% do volume dele nessa luta) mesmo tendo ficado quase todo o tempo embaixo. O Burns levou a luta pro chão 7 vezes, mas o JDM continuou produzindo de costas — o que não é o padrão normal dele (menos de 1% do volume em pé).
-   Saldo de 2.92 golpes significativos por minuto a favor — muito acima da média de carreira dele (0 a 3.84 de saldo). Claramente venceu a troca de longe mesmo sendo derrubado repetidamente.

##### Pontos Negativos

-   Defesa de quedas de 36% — a média de carreira dele é 64%, quase o dobro. O Burns completou 7 das 11 tentativas, o que mostra que o wrestling funcionou muito bem no R1 e R2.
-   Defesa de striking caiu 10 pontos em relação ao padrão (53% vs 63%). O Burns conectava 47% dos ataques — num lutador que tipicamente bate em 37% dos adversários, isso é preocupante. O JDM sobreviveu no striking e fez o nocaute, mas tomou pancada demais durante o caminho.

---

#### 3\. vs Kevin Holland — UFC Fight Night: Grasso vs. Shevchenko 2 (16/09/2023)

**Decisão | R3 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Jack Della Maddalena | Kevin Holland |
| --- | :-: | :-: |
| Sig Strikes Conectados | 105 | 127 |
| Sig Strikes Tentados | 190 | 356 |
| Precisão (%) | 55% | 36% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 0/0 | 0/2 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:00 | 0:00 |
| Controle (%) | 0% | 0% |

##### Pontos Positivos

-   Venceu uma luta onde tomou mais golpes no cômputo geral (127 vs 105) mas manteve precisão de 55% — 4 pontos acima da média. Prova que qualidade bate quantidade: o Holland tentou 356 golpes, o JDM 190. Economizou energia, não desperdiçou tentativas.
-   Defesa de quedas de 100% (Holland tentou 2, não completou nenhuma). Bem acima dos 64% de carreira — aproveitou que o Holland não é wrestler e fechou esse caminho completamente.

##### Pontos Negativos

-   Saldo de -1.47 golpes/min — o único caso entre as vitórias analisadas onde o oponente conectou mais por minuto. Ganhou a luta na precisão, não no volume. Com adversários mais certeiros que o Holland isso seria um problema.
-   R2 e R3 com saldo negativo (-3.0 e -1.6), o Holland tomou a luta no meio. Só sobreviveu porque o R1 foi forte (8.2/min) e a precisão do adversário era ruim. Padrão de entrada rápida e queda de ritmo é algo a observar.

---

#### 4\. vs Bassil Hafez — UFC Fight Night: Holm vs. Bueno Silva (15/07/2023)

**Decisão | R3 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Jack Della Maddalena | Bassil Hafez |
| --- | :-: | :-: |
| Sig Strikes Conectados | 83 | 32 |
| Sig Strikes Tentados | 137 | 124 |
| Precisão (%) | 61% | 26% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/2 | 3/20 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 1:19 | 6:48 |
| Controle (%) | 9% | 45% |

##### Pontos Positivos

-   Precisão de 61% — 10 pontos acima da média de carreira (51%). Uma das melhores performances de eficiência registradas. Conectou mais da metade dos golpes contra um oponente que trocou ativamente com ele.
-   Defesa de striking de 74% e quedas de 85% — ambas as mais altas entre as 5 lutas analisadas. A versão mais completa defensivamente: parou 17 das 20 tentativas de queda do Hafez e bloqueou quase 3 em cada 4 ataques.
-   No R3 conectou 8.6/min com saldo de 7.2 golpes/min a favor — muito acima do padrão (5.57/min). A luta foi encontrando o ritmo round a round: R1 abaixo do padrão (2.6/min), R2 no padrão (5.4/min), R3 explodindo.

##### Pontos Negativos

-   Perdeu o controle no R1 de forma acentuada: o Hafez aplicou 3 quedas e ficou 199 segundos em cima. O JDM saiu do R1 em desvantagem nítida no chão, numa luta que parecia fácil no papel. O problema não foi o striker — foi o grappler que o pegou desprevenido.
-   Saldo de controle final: 6:48 para o Hafez vs 1:19 para o JDM. Mesmo dominando em pé, perdeu o controle de tempo de solo por 5 minutos. Numa luta mais fechada, isso poderia ter pesado nos scorecards.

---

### Derrotas Recentes

#### 1\. vs Islam Makhachev — UFC 322: Della Maddalena vs. Makhachev (15/11/2025)

**Decisão | R5 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Jack Della Maddalena | Islam Makhachev |
| --- | :-: | :-: |
| Sig Strikes Conectados | 18 | 30 |
| Sig Strikes Tentados | 61 | 57 |
| Precisão (%) | 30% | 53% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 0/1 | 4/4 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:00 | 19:10 |
| Controle (%) | 0% | 77% |

##### Pontos Negativos

-   Volume colapsou 87% abaixo da média: 0.72 golpes sig/min vs 5.57/min de carreira. Esse número não é exagero — foram apenas 18 golpes conectados em 25 minutos. A luta praticamente não existiu no lado ofensivo do JDM.
-   Precisão de 30% — 21 pontos abaixo da média dele (51%). Mas o problema não era a mira: era que ele quase não conseguiu atacar. Nos R4 e R5 conectou apenas 1 golpe por round. Ficou totalmente neutralizado no chão sem conseguir produzir.
-   Defesa de quedas de 0% — o Makhachev completou as 4 tentativas das 4 que tentou. A média de carreira do JDM é 64% de defesa. Nunca visto esse colapso nas lutas analisadas; nos outros confrontos contra grapplers (Burns, Hafez) segurou ao menos parte das quedas.
-   19 minutos e 10 segundos de controle do Makhachev — o equivalente a quase 4 rounds inteiros embaixo. O JDM ficou 0 segundos em cima durante toda a luta. Os rounds R4 e R5 foram de rendição: 1 golpe conectado por round, saldo negativo, sem saída.

##### Pontos Positivos

-   Aguentou 25 minutos sem ser finalizado contra o maior grappler da categoria, sem receber um único nocaute. Absorveu o controle e manteve o jogo em pé o suficiente para ver a decisão. É resistência, não vitória — mas mostra que o queixo e o cardio não foram o problema.
-   Defesa de striking de 47% — caiu 16 pontos em relação à média (63%), mas num contexto de 19 minutos de controle do oponente, receber menos da metade dos ataques em pé é o que salvou a luta de virar finalização. Não foi bom, mas poderia ter sido pior dadas as circunstâncias.

---

## Capítulo 7: Análise Round a Round — Carlos Prates

> Como Prates se comporta em cada round — volume, precisão, knockdowns, grappling. Os dados que mostram onde ele acelera e onde fica vulnerável conforme a luta avança.

### Perfil Geral

-   Total de lutas analisadas: 7
-   Categoria: Peso Meio-Médio
-   Resultado geral: 6V-1D
-   Vitórias por método: 6 KO/TKO
-   Derrotas por método: 1 Decisão
-   Lutas com dados de rounds 4-5: 1 (vs Ian Machado Garry)

**Amostra pequena:** os dados de Prates nos rounds 3, 4 e 5 vêm de apenas 1 luta do recorte (vs Ian Machado Garry). Use esses números como sinal direcional, não como padrão consolidado.

### Dados Frios — Médias por Round

#### Striking

| Métrica | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Golpes sig. conectados/min | 3.6 | 5.3 | 2.0 | 2.4 | 4.4 |
| Tentativas sig./min | 6.6 | 8.4 | 4.0 | 6.6 | 7.6 |
| Precisão sig. (%) | 53% | 61% | 50% | 36% | 58% |
| Knockdowns | 0.7 | 1.0 | 0 | 0 | 0 |
| Knockdowns/5min | 0.7 | 1.8 | 0.0 | 0.0 | 0.0 |
| Golpes sig. oponente/min | 3.8 | 5.5 | 5.2 | 4.6 | 5.6 |
| Precisão sig. oponente (%) | 52% | 56% | 50% | 55% | 68% |
| Dominância striking (%) | 49% | 48% | 28% | 34% | 44% |

#### Grappling

| Métrica | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Quedas conectadas/5min | 0.1 | 0.0 | 0.0 | 0.0 | 0.0 |
| Quedas oponente/5min | 0.3 | 0.0 | 2.0 | 2.0 | 0.0 |
| Defesa de queda (%) | 87% | 100% | 33% | 71% | 100% |
| Controle (%) | 4% | 3% | 6% | 0% | 20% |
| Controle oponente (%) | 15% | 11% | 28% | 19% | 11% |
| Dominância controle (%) | 29% | 52% | 18% | 0% | 64% |

#### Saldos

| Métrica | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Saldo sig./min | \-0.2 | \-0.2 | \-3.2 | \-2.2 | \-1.2 |
| Saldo quedas/5min | \-0.1 | 0.0 | \-2.0 | \-2.0 | 0.0 |
| Saldo controle (pp) | \-12pp | \-9pp | \-22pp | \-19pp | +9pp |

### Dados Frios — Variações Médias Round a Round

#### Striking

| Métrica | R1→R2 (n=4) | R2→R3 (n=1) | R3→R4 (n=1) | R4→R5 (n=1) |
| --- | --- | --- | --- | --- |
| Δ Golpes sig./min | +2.1 | \-0.4 | +0.4 | +2.0 |
| Δ Tentativas sig./min | +2.7 | \-0.4 | +2.6 | +1.0 |
| Δ Precisão sig. (pp) | +6pp | \-5pp | \-14pp | +22pp |
| Δ Knockdowns/5min | +1.5 | 0.0 | 0.0 | 0.0 |

#### Saldos

| Métrica | R1→R2 (n=4) | R2→R3 (n=1) | R3→R4 (n=1) | R4→R5 (n=1) |
| --- | --- | --- | --- | --- |
| Δ Saldo sig./min | +0.7 | +1.2 | +1.0 | +1.0 |
| Δ Saldo quedas/5min | +0.5 | \-2.0 | 0.0 | +2.0 |
| Δ Saldo controle (pp) | +7pp | \-30pp | +3pp | +28pp |
| Δ Controle (pp) | +2pp | \-2pp | \-6pp | +20pp |

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos -- Prates (%)

| Alvo | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Cabeça | 42% | 44% | 60% | 75% | 77% |
| Corpo | 20% | 26% | 40% | 17% | 23% |
| Perna | 38% | 30% | 0% | 8% | 0% |

#### Alvos -- Oponentes (%)

| Alvo | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Cabeça | 46% | 46% | 73% | 65% | 79% |
| Corpo | 13% | 5% | 15% | 13% | 7% |
| Perna | 41% | 49% | 12% | 22% | 14% |

#### Posição -- Prates (%)

| Posição | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Distância | 96% | 98% | 100% | 100% | 41% |
| Clinch | 2% | 0% | 0% | 0% | 5% |
| Chão | 2% | 2% | 0% | 0% | 55% |

#### Posição -- Oponentes (%)

| Posição | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
| --- | --- | --- | --- | --- | --- |
| Distância | 91% | 99% | 100% | 100% | 93% |
| Clinch | 6% | 1% | 0% | 0% | 7% |
| Chão | 4% | 0% | 0% | 0% | 0% |

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Res. | Método | Round | Tempo | Sig./min | Prec. | KD | Saldo sig./min | Sig. oponente/min | Controle (%) | Controle oponente (%) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 10/02/2024 | Trevin Giles | V | KO/TKO | 2 | 4:03 | 4.1 | 51% | 1 | \-3.4 | 7.6 | 0% | 0% |
| 08/06/2024 | Charles Radtke | V | KO/TKO | 1 | 4:47 | 3.1 | 42% | 1 | +0.2 | 2.9 | 1% | 7% |
| 17/08/2024 | Li Jingliang | V | KO/TKO | 2 | 4:02 | 6.1 | 65% | 3 | +1.6 | 4.5 | 1% | 0% |
| 09/11/2024 | Neil Magny | V | KO/TKO | 1 | 4:50 | 2.5 | 57% | 2 | +0.4 | 2.1 | 24% | 7% |
| 26/04/2025 | Ian Machado Garry | D | Decisão | 5 | 5:00 | 2.5 | 49% | 0 | \-2.5 | 5.0 | 7% | 30% |
| 16/08/2025 | Geoff Neal | V | KO/TKO | 1 | 4:59 | 6.4 | 53% | 1 | +1.4 | 5.0 | 0% | 5% |
| 15/11/2025 | Leon Edwards | V | KO/TKO | 2 | 1:28 | 3.3 | 66% | 1 | +1.4 | 1.9 | 0% | 30% |

### Análise Técnica

-   Saldo de striking negativo em todos os 5 rounds na média, mas volume próprio sobe do R1 para o R2 com precisão acompanhando -- aceleração seletiva no segundo round, não descontrolada.
-   Knockdowns exclusivamente nos rounds 1 e 2 (média 0.7 e 1.0), zero nos rounds tardios. Saldo de controle piora progressivamente. Capacidade de finalização concentrada no início da luta.
-   Defesa de queda cai de 87% (R1) para 33% (R3, n=1 vs Garry), com controle do oponente triplicando. Vulnerabilidade ao grappling cresce com a duração da luta.
-   Saldo de striking melhora a cada transição de round (+0.7, +1.2, +1.0, +1.0), mesmo com saldo absoluto negativo -- há adaptação tática intra-luta.
-   Contra Giles: saldo sig. de -3.4/min (pior da carreira), mas KO no R2. O saldo de volume não capta golpes de potência decisivos.

### Brechas e Insights

**1.** Distribuição de cabeça sobe de 42% (R1) para 77% (R5), com precisão caindo a 36% no R4 antes de voltar a 58% no R5. A recuperação coincide com mudança de posição (distância 41%, chão 55% no R5).

**2.** Controle próprio irrelevante nos R1-R4 (0-6%), mas salta para 20% no R5 com 55% dos golpes do chão. Transição tática de striker puro para ground-and-pound em rounds tardios.

**3.** 9 knockdowns em 6 vitórias (média 1.5/luta). Única derrota: 0 KD em 5 rounds. Ausência de knockdowns como principal preditor de resultado adverso, acima de volume ou saldo.

**4.** Tentativas de queda dos oponentes sobem de 2.0/5min (R1) para 7.0/5min (R4), com defesa caindo de 87% para 71%. Pressão de wrestling escala com o tempo e a resposta defensiva não acompanha.

---

## Capítulo 8: Análise Round a Round — Jack Della Maddalena

### Perfil Geral

-   Total de lutas analisadas: 9
-   Categoria: Peso Meio-Médio
-   Resultado geral: 8V-1D
-   Vitórias por método: 3 Decisão, 4 KO/TKO, 1 Finalização
-   Derrotas por método: 1 Decisão
-   Lutas com dados de rounds 4-5: 2 (Belal Muhammad, Islam Makhachev)

### Dados Frios — Médias por Round

#### Striking

| Métrica | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Golpes sig. conectados/min | 6.5 | 4.6 | 6.1 | 3.4 | 5.4 |
| Tentativas sig./min | 12.8 | 8.8 | 11.0 | 7.0 | 8.9 |
| Precisão sig. (%) | 48% | 52% | 56% | 33% | 40% |
| Knockdowns/5min | 1.0 | 0.0 | 0.3 | 0.0 | 0.0 |
| Golpes sig. oponente/min | 4.0 | 4.2 | 3.5 | 3.8 | 2.7 |
| Precisão sig. oponente (%) | 34% | 40% | 30% | 53% | 22% |

**Amostra pequena:** R4 usa apenas 2 lutas. Makhachev (0.2 sig/min, 9% precisão) puxa a média para baixo; Muhammad (6.6 sig/min, 56% precisão) está no extremo oposto. A média de 3.4/min não representa nenhuma das duas lutas isoladamente.

**Amostra pequena:** R5 usa apenas 2 lutas. Makhachev (0.2 sig/min) e Muhammad (10.6 sig/min) puxam a média em direções opostas. A média de 5.4/min deve ser lida com cautela.

#### Grappling

| Métrica | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Takedowns/5min | 0.0 | 0.0 | 0.2 | 0.0 | 0.0 |
| Tentativas TD/5min | 0.2 | 0.2 | 0.4 | 0.0 | 1.0 |
| Precisão TD (%) | 0% | 0% | 50% | \-- | 0% |
| Submissões/5min | 0.3 | 0.0 | 0.0 | 0.0 | 0.0 |
| Controle (%) | 3% | 0% | 6% | 5% | 2% |
| TD oponente/5min | 1.0 | 0.4 | 0.7 | 1.0 | 1.5 |
| Precisão TD oponente (%) | 52% | 25% | 44% | 67% | 100% |
| Controle oponente (%) | 22% | 32% | 31% | 47% | 63% |
| Defesa de TD (%) | 48% | 75% | 56% | 33% | 0% |

#### Saldos e Dominância

| Métrica | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Saldo sig./min | +2.5 | +0.4 | +2.6 | \-0.4 | +2.7 |
| Saldo TD/5min | \-1.0 | \-0.4 | \-0.5 | \-1.0 | \-1.5 |
| Saldo controle (pp) | \-18pp | \-32pp | \-24pp | \-43pp | \-61pp |
| Dominância striking (%) | 61% | 52% | 65% | 32% | 83% |
| Dominância TD (%) | 0% | 0% | 33% | 0% | 0% |
| Dominância controle (%) | 35% | 1% | 19% | 13% | 4% |

### Dados Frios — Variações Médias Round a Round

#### Striking

| Métrica | R1→R2 (n=5) | R2→R3 (n=5) | R3→R4 (n=2) | R4→R5 (n=2) |
| --- | --- | --- | --- | --- |
| Variação sig. conectados/min | +0.4 | +1.5 | \-0.9 | +2.0 |
| Variação sig. conectados (%) | +18% | +68% | \-46% | +30% |
| Variação tentativas sig./min | +0.4 | +2.1 | \-2.6 | +1.9 |
| Variação precisão sig. (pp) | +7pp | +4pp | \-12pp | +8pp |
| Variação knockdowns/5min | 0.0 | +0.3 | 0.0 | 0.0 |

#### Grappling e Controle

| Métrica | R1→R2 (n=5) | R2→R3 (n=5) | R3→R4 (n=2) | R4→R5 (n=2) |
| --- | --- | --- | --- | --- |
| Variação TD/5min | 0.0 | +0.2 | 0.0 | 0.0 |
| Variação tentativas TD/5min | \-0.2 | +0.2 | \-0.5 | +1.0 |
| Variação controle (pp) | +0pp | +6pp | +4pp | \-3pp |

#### Saldos

| Métrica | R1→R2 (n=5) | R2→R3 (n=5) | R3→R4 (n=2) | R4→R5 (n=2) |
| --- | --- | --- | --- | --- |
| Variação saldo sig./min | \-0.1 | +2.2 | \-0.4 | +3.1 |
| Variação saldo TD/5min | +1.0 | \-0.1 | \-0.5 | \-0.5 |
| Variação saldo controle (pp) | +2pp | +8pp | \-9pp | \-18pp |

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos — Della Maddalena (%)

| Alvo | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Cabeça | 66% | 57% | 64% | 41% | 84% |
| Corpo | 24% | 33% | 27% | 6% | 15% |
| Perna | 10% | 10% | 9% | 53% | 1% |

#### Alvos — Oponente (%)

| Alvo | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Cabeça | 53% | 77% | 67% | 70% | 96% |
| Corpo | 19% | 11% | 21% | 16% | 4% |
| Perna | 29% | 13% | 13% | 14% | 0% |

#### Posição — Della Maddalena (%)

| Posição | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Distância | 81% | 97% | 72% | 98% | 92% |
| Clinch | 9% | 3% | 16% | 2% | 8% |
| Chão | 10% | 0% | 12% | 0% | 0% |

#### Posição — Oponente (%)

| Posição | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
| --- | --- | --- | --- | --- | --- |
| Distância | 91% | 81% | 84% | 90% | 93% |
| Clinch | 8% | 8% | 11% | 8% | 4% |
| Chão | 1% | 11% | 5% | 2% | 4% |

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Res. | Método | Rds | Sig/min | Tent. sig/min | Precisão | KD/min | Saldo sig/min | Def. sig (%) | Def. TD (%) | Ctrl (%) | Cab (%) | Corpo (%) | Dist (%) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 22/01/2022 | Pete Rodriguez | V | KO/TKO | 1 | 14.4 | 27.2 | 53% | 0.3 | +6.0 | 64% | \-- | 1% | 88% | 12% | 93% |
| 11/06/2022 | Ramazan Emeev | V | KO/TKO | 1 | 7.1 | 14.2 | 50% | 0.4 | +4.3 | 71% | 50% | 2% | 61% | 39% | 61% |
| 19/11/2022 | Danny Roberts | V | KO/TKO | 1 | 9.7 | 17.7 | 55% | 0.6 | +8.2 | 85% | 100% | 17% | 70% | 27% | 82% |
| 11/02/2023 | Randy Brown | V | Finalização | 1 | 6.3 | 14.0 | 45% | 0.5 | +1.4 | 72% | \-- | 11% | 64% | 7% | 36% |
| 15/07/2023 | Bassil Hafez | V | Decisão | 3 | 5.5 | 9.1 | 61% | 0.0 | +3.4 | 74% | 85% | 9% | 66% | 33% | 82% |
| 16/09/2023 | Kevin Holland | V | Decisão | 3 | 7.0 | 12.7 | 55% | 0.0 | \-1.5 | 64% | 100% | 0% | 44% | 34% | 90% |
| 09/03/2024 | Gilbert Burns | V | KO/TKO | 3 | 4.9 | 9.0 | 54% | 0.1 | +2.9 | 53% | 36% | 2% | 81% | 13% | 70% |
| 10/05/2025 | Belal Muhammad | V | Decisão | 5 | 7.1 | 13.7 | 52% | 0.0 | +1.8 | 58% | 67% | 3% | 63% | 26% | 94% |
| 15/11/2025 | Islam Makhachev | D | Decisão | 5 | 0.7 | 2.4 | 30% | 0.0 | \-0.5 | 47% | 0% | 0% | 56% | 33% | 78% |

### Análise Técnica

-   Volume cai do R1 para o R2 mas precisão sobe -- transição de explosão inicial para seletividade, não fadiga.
-   Saldo de striking positivo nos rounds 1-3 (+2.5 a +2.6/min), mas dominância de controle na direção oposta, com oponentes acumulando tempo crescente. Vantagem no striking coexiste com vulnerabilidade posicional.
-   Defesa de takedown deteriora de 75% (R2) a 0% (R5), enquanto volume ofensivo de TD do oponente sobe. Resistência à queda degrada mais rápido que o cardio de striking.
-   Nas 4 finalizações antecipadas (Rodriguez, Emeev, Roberts, Brown), saldo sig/min médio no R1 foi +5.0 vs +1.0 nas lutas que foram à distância. Desfecho rápido depende de abrir vantagem de striking no início.
-   Precisão do oponente cai no R3 (30%) enquanto a dele sobe ao pico (56%). Pressão cumulativa degrada a eficiência adversária.

### Brechas e Insights

**1.** Saldo sig/min positivo em R1-R3, mas saldo de controle sempre negativo. Leva vantagem em pé, mas cede terreno na disputa posicional. Se o oponente converter esse controle em dano, a equação muda.

**2.** Volume cai 29% do R1 para R2 (12.8 para 8.8 tentativas/min), mas precisão sobe 4pp. Proporção acerto/tentativa melhora -- economia de energia calculada.

**3.** No R3: clinch sobe de 3% (R2) para 16%, chão de 0% para 12%, e é o round com maior saldo de striking (+2.6/min). Agressividade posicional tardia ligada a pressionar adversários já desgastados.

**4.** Oponentes concentram golpes na cabeça de forma crescente (53% R1 a 96% R5), mas sem ganho de precisão (22% no R5). Abandonam corpo em rounds tardios sem retorno proporcional.

**5.** Contra Holland: saldo de -1.5/min (único negativo entre vitórias) com controle adversário 0%. Pressão de volume à distância, sem grappling, é o cenário mais difícil entre oponentes que ficam em pé.

---

## Capítulo 9: Cruzamento de Dados Frios

> Números lado a lado, sem interpretação — a matéria-prima de tudo que veio nos capítulos anteriores.

### Ficha Técnica

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
| --- | --- | --- | --- |
| Categoria | Peso Meio-Médio | Peso Meio-Médio | \- |
| Postura | Ambidestro | Ambidestro | \- |
| Ranking Categoria | 5 | 1 | \- |
| Ranking Libra por Libra | Desranqueado | 14 | \- |
| Idade (anos) | 32 🔴 | 29 🟢 | **Jack Della Maddalena** |
| Altura (cm) | 185 🟢 | 180 🔴 | **Carlos Prates** |
| Envergadura (cm) | 198 🟢 | 185 🔴 | **Carlos Prates** |
| Alcance Extra (cm) | 13 🟢 | 5 🔴 | **Carlos Prates** |

---

### Carreira Geral

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
| --- | --- | --- | --- |
| Total de Lutas | 30 🟢 | 21 🔴 | **Carlos Prates** |
| Vitórias | 23 🟢 | 18 🔴 | **Carlos Prates** |
| Derrotas | 7 🔴 | 3 🟢 | **Jack Della Maddalena** |
| Empates | 0 | 0 | Empate |
| Taxa de Vitória | 77% 🔴 | 86% 🟢 | **Jack Della Maddalena** |
| Sequência de Vitórias Atual | 2 🟢 | 0 🔴 | **Carlos Prates** |
| Vitórias por KO/TKO | 18 🟢 | 12 🔴 | **Carlos Prates** |
| Vitórias por Finalização | 3 🟢 | 2 🔴 | **Carlos Prates** |
| Vitórias por Decisão | 2 🔴 | 4 🟢 | **Jack Della Maddalena** |
| Vitórias no 1º Round | 10 🟢 | 8 🔴 | **Carlos Prates** |
| % de Vitórias Via Rápida | 91% 🟢 | 78% 🔴 | **Carlos Prates** |
| Derrotas por KO/TKO | 2 🟢 | 1 🟢 | \- |
| Derrotas por Finalização | 3 🔴 | 1 🟢 | **Jack Della Maddalena** |
| Derrotas por Decisão | 2 | 1 🟢 | **Jack Della Maddalena** |
| % de Derrotas Via Rápida | 71% 🔴 | 67% 🟢 | **Jack Della Maddalena** |
| Dist. Vitórias: % KO/TKO | 78% | 67% | \- |
| Dist. Vitórias: % Finalização | 13% | 11% | \- |
| Dist. Vitórias: % Decisão | 9% | 22% | \- |
| Dist. Derrotas: % KO/TKO | 29% | 33% | \- |
| Dist. Derrotas: % Finalização | 43% | 33% | \- |
| Dist. Derrotas: % Decisão | 29% | 33% | \- |
| Tempo Médio de Luta | 08:48 | 11:59 | \- |
| Intervalo Médio Entre Lutas (dias) | 107.33 | 174.13 | \- |

---

### Carreira no UFC

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
| --- | --- | --- | --- |
| Lutas no UFC | 8 🔴 | 10 🟢 | **Jack Della Maddalena** |
| Vitórias no UFC | 7 🔴 | 9 🟢 | **Jack Della Maddalena** |
| Derrotas no UFC | 1 | 1 | Empate |
| Empates no UFC | 0 | 0 | Empate |
| No Contests no UFC | 0 | 0 | Empate |
| Vitórias por KO/TKO no UFC | 7 🟢 | 4 🔴 | **Carlos Prates** |
| Vitórias por Finalização no UFC | 0 🔴 | 1 🟢 | **Jack Della Maddalena** |
| Vitórias por Decisão no UFC | 0 🔴 | 4 🟢 | **Jack Della Maddalena** |
| Derrotas por KO/TKO no UFC | 0 | 0 | Empate |
| Derrotas por Finalização no UFC | 0 | 0 | Empate |
| Derrotas por Decisão no UFC | 1 | 1 | Empate |
| % Carreira no UFC | 27% 🔴 | 48% 🟢 | **Jack Della Maddalena** |
| Tempo Total no UFC (min) | 70 🔴 | 120 🟢 | **Jack Della Maddalena** |
| Dist. Vitórias UFC: % KO/TKO | 100% | 44% | \- |
| Dist. Vitórias UFC: % Finalização | 0% | 11% | \- |
| Dist. Vitórias UFC: % Decisão | 0% | 44% | \- |
| Dist. Derrotas UFC: % KO/TKO | 0% | 0% | \- |
| Dist. Derrotas UFC: % Finalização | 0% | 0% | \- |
| Dist. Derrotas UFC: % Decisão | 100% | 100% | \- |

---

### Striking

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
| --- | --- | --- | --- |
| Golpes Sig. Conectados/min | 3.77 🔴 | 5.57 🟢 | **Jack Della Maddalena** |
| Golpes Sig. Absorvidos/min | 4.53 🔴 | 3.84 🟢 | **Jack Della Maddalena** |
| Precisão de Striking | 55% 🟢 | 51% 🔴 | **Carlos Prates** |
| Defesa de Striking | 47% 🔴 | 63% 🟢 | **Jack Della Maddalena** |
| Saldo de Striking por Minuto | \-0.76 🔴 | 1.73 🟢 | **Jack Della Maddalena** |
| Knockdowns Causados por 5min | 0.7 🟢 | 0.3 🔴 | **Carlos Prates** |
| Knockdowns Sofridos por 5min | 0.0 | 0.0 | Empate |
| Golpes na Cabeça por Minuto | 2.02 🔴 | 3.42 🟢 | **Jack Della Maddalena** |
| Golpes no Corpo por Minuto | 0.82 🔴 | 1.40 🟢 | **Jack Della Maddalena** |
| Golpes nas Pernas por Minuto | 0.92 🟢 | 0.51 🔴 | **Carlos Prates** |
| Golpes em Pé por Minuto | 3.52 🔴 | 4.51 🟢 | **Jack Della Maddalena** |
| Golpes no Clinche por Minuto | 0.03 🔴 | 0.49 🟢 | **Jack Della Maddalena** |
| Golpes no Solo por Minuto | 0.21 🔴 | 0.33 🟢 | **Jack Della Maddalena** |
| Golpes p/ Nocautear (média) | 38 🟢 | 167 🔴 | **Carlos Prates** |
| Dist. Alvo: % Cabeça | 54% | 64% | \- |
| Dist. Alvo: % Corpo | 22% | 26% | \- |
| Dist. Alvo: % Pernas | 25% | 9% | \- |
| Dist. Posição: % Em Pé | 94% | 85% | \- |
| Dist. Posição: % Clinche | 1% | 9% | \- |
| Dist. Posição: % Solo | 6% | 6% | \- |

---

### Grappling

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
| --- | --- | --- | --- |
| Precisão de Quedas | 100% 🟢 | 10% 🔴 | **Carlos Prates** |
| Defesa de Quedas | 80% 🟢 | 64% 🔴 | **Carlos Prates** |
| Quedas Aplicadas por 5min | 0.1 🟢 | 0.05 🔴 | **Carlos Prates** |
| Quedas Sofridas por 5min | 0.45 🟢 | 0.85 🔴 | **Carlos Prates** |
| Tentativas de Queda por 5min | 0.07 🟢 | 0.0 🔴 | **Carlos Prates** |
| Tentativas de Finalização Causadas por 5min | 0.0 🔴 | 0.05 🟢 | **Jack Della Maddalena** |
| Tentativas de Finalização Sofridas por 5min | 0.0 🟢 | 0.05 🔴 | **Carlos Prates** |
| % Controle Médio nas Lutas | 5% | 5% | Empate |

---

### Índices Compostos

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
| --- | --- | --- | --- |
| Resiliência a Nocaute | 81% 🔴 | 85% 🟢 | **Jack Della Maddalena** |
| Taxa de Vitória no 1º Round | 43% 🔴 | 44% 🟢 | **Jack Della Maddalena** |
| Taxa de Vitória Geral | 77% 🔴 | 86% 🟢 | **Jack Della Maddalena** |
| Golpes p/ Ser Nocauteado (média) | sem dado | sem dado | \- |
| % Luta Combatida (médio) | 50% 🔴 | 63% 🟢 | **Jack Della Maddalena** |
| DNA de Estilo Equilibrado | 0.1 | sem dado | \- |
| Perfil de Distância de Luta | 0.86 | sem dado | \- |

> **Legenda:** 🟢 Vantagem | 🔴 Desvantagem | Empate = valores idênticos | - = sem dado ou sem vantagem direta
