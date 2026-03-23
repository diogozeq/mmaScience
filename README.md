# Relatório Final — Carlos Prates vs Jack Della Maddalena

> **Autor:** Diogo Zequini — Cientista de Dados | Compilado em 2026-03-20
>
> Este relatório analisa 8 lutas de Carlos Prates e 10 lutas de Jack Della Maddalena no UFC (2022-2025), com base em dados de UFC Stats, UFC.com e Tapology, processados com Python e algoritmos de machine learning para ajuste por qualidade de oponente. O relatório começa pelo que importa: as ações concretas. Os dados e análises que sustentam cada recomendação estão nos capítulos seguintes.

## Sumário

1. [Resumo Final — Melhores Ações para o Prates](#capitulo-1-resumo-final)
2. [Inteligência Adversária — O Que a Equipe do Jack Provavelmente Vai Planejar](#capitulo-2-inteligencia-adversaria)
3. [Insights Ocultos — Carlos Prates](#capitulo-3-insights-ocultos--carlos-prates)
   - [Onde Ele é Extremo na Categoria](#prates-onde-ele-e-extremo-na-categoria)
   - [O Paradoxo das Vitórias e Derrotas](#prates-o-paradoxo-das-vitorias-e-derrotas)
   - [Padrões de Contexto](#prates-padroes-de-contexto)
   - [O Modelo Ajustado vs a Realidade](#prates-o-modelo-apm-vs-a-realidade) (inclui modelo atualizado)
   - [Lutas Anômalas](#prates-lutas-anomalas)
   - [Sinais Fracos Combinados](#prates-sinais-fracos-combinados)
   - [Visão do Analista](#prates-visao-do-analista)
4. [Insights Ocultos — Jack Della Maddalena](#capitulo-4-insights-ocultos--jack-della-maddalena)
   - [Onde Ele é Extremo na Categoria](#jdm-onde-ele-e-extremo-na-categoria)
   - [O Paradoxo das Vitórias e Derrotas](#jdm-o-paradoxo-das-vitorias-e-derrotas)
   - [Padrões de Contexto](#jdm-padroes-de-contexto)
   - [O Modelo Ajustado vs a Realidade](#jdm-o-modelo-apm-vs-a-realidade) (inclui modelo atualizado)
   - [Lutas Anômalas](#jdm-lutas-anomalas)
   - [Sinais Fracos Combinados](#jdm-sinais-fracos-combinados)
   - [Visão do Analista](#jdm-visao-do-analista)
5. [Análise Subjetiva Luta a Luta — Carlos Prates](#capitulo-5-analise-subjetiva--carlos-prates)
   - [Médias de Carreira](#prates-sub-medias-de-carreira)
   - [Resumo do Recorte](#prates-sub-resumo-do-recorte)
   - [Vitórias Recentes](#prates-sub-vitorias-recentes)
   - [Derrotas Recentes](#prates-sub-derrotas-recentes)
   - [Padrões Transversais](#prates-sub-padroes-transversais)
   - [Visão do Coach](#prates-sub-visao-do-coach)
6. [Análise Subjetiva Luta a Luta — Jack Della Maddalena](#capitulo-6-analise-subjetiva--jack-della-maddalena)
   - [Médias de Carreira](#medias-de-carreira)
   - [Resumo do Recorte](#resumo-do-recorte)
   - [Vitórias Recentes](#vitorias-recentes)
   - [Derrotas Recentes](#derrotas-recentes)
   - [Padrões Transversais](#padroes-transversais)
   - [Visão do Analista](#visao-do-analista-1)
7. [Análise Round a Round — Carlos Prates](#capitulo-7-analise-round-a-round--carlos-prates)
   - [Perfil Geral](#perfil-geral)
   - [Dados Frios — Médias por Round](#dados-frios----medias-por-round)
   - [Dados Frios — Variações Médias Round a Round](#dados-frios----variacoes-medias-round-a-round)
   - [Dados Frios — Distribuição de Alvos e Posições por Round](#dados-frios----distribuicao-de-alvos-e-posicoes-por-round)
   - [Dados Frios — Detalhamento Luta a Luta](#dados-frios----detalhamento-luta-a-luta)
   - [Análise Técnica](#analise-tecnica)
   - [Brechas e Insights](#brechas-e-insights)
8. [Análise Round a Round — Jack Della Maddalena](#capitulo-8-analise-round-a-round--jack-della-maddalena)
   - [Perfil Geral](#jdm-rar-perfil-geral)
   - [Dados Frios — Médias por Round](#jdm-rar-medias-por-round)
   - [Dados Frios — Variações Médias Round a Round](#jdm-rar-variacoes)
   - [Dados Frios — Distribuição de Alvos e Posições](#jdm-rar-alvos-posicoes)
   - [Dados Frios — Detalhamento Luta a Luta](#jdm-rar-detalhamento)
   - [Análise Técnica](#jdm-rar-analise-tecnica)
   - [Brechas e Insights](#jdm-rar-brechas)
9. [Cruzamento de Dados](#capitulo-9-cruzamento-de-dados)
   - [Ficha Técnica](#ficha-tecnica)
   - [Carreira Geral](#carreira-geral)
   - [Carreira no UFC](#carreira-no-ufc)
   - [Striking](#striking)
   - [Grappling](#grappling)
   - [Índices Compostos](#indices-compostos)

---

<a name="capitulo-1-resumo-final"></a>
## Capítulo 1: Resumo Final — Melhores Ações para o Prates

> Os dados apontam 7 jogadas concretas, rankeadas por impacto. A primeira define o round 1.

Em ordem de importância, este é o caminho mais consistente para o Prates vencer segundo o conjunto dos dados:

1. **Tratar os rounds 1 e 2 como janela principal de vitória.** É onde o poder de knockdown e a taxa de interrupção do Prates mais aparecem, antes de o ritmo longo de volume e precisão do Jack ganhar corpo.

2. **Proteger o corpo como prioridade defensiva.** O ataque ao corpo do Jack não é detalhe; é um padrão recorrente e um dos melhores caminhos técnicos dele para construir a luta.

3. **Variar os alvos desde cedo, em vez de caçar só a cabeça.** As melhores vitórias do Prates aparecem quando ele distribui melhor os golpes e dificulta a leitura do adversário.

4. **Não aceitar uma luta limpa em média-curta, com trocas longas e ritmo contínuo.** Essa é a faixa em que o Jack tende a combinar melhor precisão com volume. O ideal para o Prates é entrar para causar dano e sair, sem ficar preso na sequência do outro lado.

5. **Ganhar a luta no impacto, não na contagem.** Os dados do Prates premiam golpes decisivos; os do Jack premiam acúmulo. Quanto mais a luta virar disputa de volume puro, mais o cenário tende a favorecer o australiano.

6. **Usar clinch e grappling apenas como recurso pontual de quebra de ritmo.** Há brechas defensivas do Jack nesse setor, mas o histórico do Prates não sustenta um plano de wrestling ofensivo como rota principal.

7. **Se a luta alongar, trocar urgência por disciplina.** Nesse cenário, o mais importante passa a ser negar o acúmulo de volume do Jack, manter seleção de golpes e não entregar a luta em trocas contínuas.

---

<a name="capitulo-2-inteligencia-adversaria"></a>
## Capítulo 2: Inteligência Adversária — O Que a Equipe do Jack Provavelmente Vai Planejar

> Os mesmos dados que sustentam o Capítulo 1 apontam o caminho provável do outro lado. Saber o que esperar é metade da preparação.

Se a equipe do Jack fizer o dever de casa com dados, este é o plano mais provável que vão montar:

1. **Sobreviver os primeiros 10 minutos como prioridade absoluta.** Todos os 9 knockdowns do Prates no UFC aconteceram nos rounds 1 e 2 — zero no R3 em diante. 81% do volume ofensivo dele (191 de 235 golpes sig.) se concentra nesses dois rounds. A precisão dele cai de 61% (R2) para 36% (R4). Se o Jack chegar ao minuto 10 sem dano relevante, a luta muda de figura.

2. **Atacar o corpo desde o R1, sem esperar.** O ataque ao corpo do Jack é elite: entre os 6% melhores da divisão quando ajustado, com 71% de precisão (147 acertos em 207 tentativas). Golpes no corpo degradam a velocidade de reação do Prates exatamente dentro da janela onde ele é mais perigoso, criam dilema de guarda (baixar o cotovelo abre a cabeça) e interrompem o setup de chutes nas pernas.

3. **Acumular volume em vez de caçar o nocaute.** O Jack conecta 5.57 golpes sig./min contra 3.77 do Prates, com saldo de +1.73/min vs -0.76/min. A precisão do Jack é real (entre os 7% melhores quando ajustada), enquanto a defesa do Prates é porosa (oponentes acertam 54% contra ele, rank 70/84 na divisão). O volume natural do Jack já cria o cenário que levou à derrota do Prates contra Garry sem precisar de estratégia especial.

4. **Usar o clinch como zona segura e quebra de ritmo.** O Prates tem 2 golpes no clinch em toda a carreira UFC (percentil 1% da divisão) — é território onde ele não tem resposta. O Jack tem eficiência de 77% no clinch e aumenta o volume ali nos rounds tardios (de 2.1 golpes/round no R1 para 4.0 no R5). Cada clinch retira o Prates do único ambiente onde é letal.

5. **Negar a troca aberta e estática nos primeiros rounds.** O paradoxo dos dados: o Prates absorve mais golpes quando ganha (5.5/min) do que quando perde (4.9/min). Ele precisa de trocação aberta para acessar o contragolpe. Movimento lateral, saídas de ângulo após combinações e recusa de ficar plantado na média distância negam essa condição.

6. **Forçar o Prates a ficar previsível nos alvos.** Nas vitórias, a distribuição dele é equilibrada (38% cabeça, 29% corpo, 32% pernas). Na derrota contra Garry: 54% na cabeça, pernas caindo para 14%, precisão na cabeça a 39%. Pressão constante e mudança de ângulos tendem a empurrar o Prates para atacar cabeça — exatamente o alvo que o Jack melhor defende (63% de defesa bruta, rank 4/93 na divisão para golpes na cabeça).

7. **Alongar a luta e confiar no plano de decisão.** Tempo médio de luta: Jack 11:59 vs Prates 8:48 — diferença de 3:11 por luta. O Jack está no percentil 97% de duração de luta; o Prates no percentil 32%. 44% das vitórias do Jack no UFC são por decisão. O Prates tem 0% de vitórias por decisão no UFC. A assimetria de experiência em lutas longas é objetiva: a única luta do Prates acima de 15 minutos terminou em derrota.

8. **Explorar grappling a partir do R3, não antes.** A defesa de queda do Prates cai de 87% (R1) para 33% (R3) — e o controle do oponente triplica. Ele tem 0 reversões em toda a carreira registrada no banco. Quando vai ao chão, permanece lá. A equipe do Jack provavelmente vai reservar tentativas de queda para os rounds tardios, quando a defesa degrada e o desgaste do corpo já se acumulou.

9. **Replicar o blueprint Garry com mais volume.** Garry fez 19 tentativas de queda, converteu 4, acumulou 189 segundos de controle. O resultado: 0 knockdowns do Prates em 5 rounds, saldo de -2.5 sig./min. O Garry venceu com pressão posicional, não com striking. O Jack tem o mesmo recurso de pressão posicional, mas com volume de striking superior (5.57/min vs ~3.5/min do Garry) — pode combinar as duas coisas.

10. **Tratar o chute de pernas do Prates como ameaça menor.** Após ajuste por qualidade de oponente, o Prates está entre os 1% piores da divisão em chutes de perna reais — os oponentes dele historicamente defendem pouco esse ataque. O Jack pode absorver esses chutes sem alterar a guarda e manter foco no plano principal. A exceção seria se o Prates mudar radicalmente o alvo dos chutes (como fez contra Edwards com 52% nas pernas), mas isso reduz a ameaça à cabeça.

---

<a name="capitulo-3-insights-ocultos--carlos-prates"></a>
## Capítulo 3: Insights Ocultos — Carlos Prates

> Percentis extremos, paradoxos e sinais que só aparecem quando se cruza tudo. Aqui estão os dados que nenhum scout convencional entrega.

> **Como funciona o modelo ajustado?** Quando olhamos os números brutos de um lutador (precisão, defesa, volume), eles misturam a habilidade dele com a qualidade dos adversários que enfrentou. O modelo ajustado separa essas duas coisas: desconta o efeito do oponente e mostra o que é habilidade real do lutador vs o que é inflado ou deflacionado pelos caras que ele cruzou. Exemplo: se um lutador tem 60% de precisão mas só enfrentou oponentes com defesa fraca, a precisão real dele é menor. O modelo corrige isso. Nos rankings abaixo, "entre os X% melhores" significa que, descontando o efeito dos oponentes, ele é melhor que a maioria da divisão naquela métrica. "Entre os X% piores" é o contrário.

<a name="prates-onde-ele-e-extremo-na-categoria"></a>
### Onde Ele é Extremo na Categoria (Peso Meio-Médio)

Métricas onde Prates está entre os 10% melhores ou 10% piores da divisão — e que nenhum outro relatório menciona diretamente.

| Métrica | Valor | Posição | N da Categoria |
|---------|-------|---------|----------------|
| Knockdowns/5min | 0.7 | Entre os 5% melhores | 84 |
| Tentativas de queda (carreira UFC) | 1 | Entre os 5% piores | 84 |
| Golpes no clinch (total UFC) | 2 | Entre os 8% piores | 84 |
| Finalizações/5min | 0.0 | Último da divisão | 84 |

**O que isso revela:**

- Taxa de KD melhor que 95% da divisão combinada com quase nenhuma tentativa de queda (só 5% da divisão tenta menos). O poder de nocaute substitui o wrestling ofensivo.
- 2 golpes no clinch em 7 lutas UFC, 0 finalizações tentadas. Opera numa faixa de distância específica e raramente se desvia.

---

<a name="prates-o-paradoxo-das-vitorias-e-derrotas"></a>
### O Paradoxo das Vitórias e Derrotas

Métricas que se comportam ao contrário do esperado quando ele ganha vs quando ele perde.

| Métrica | Média Vitórias (n=6) | Média Derrota (n=1) | Ratio | Direção Esperada |
|---------|---------------------|---------------------|-------|-----------------|
| Golpes sig. absorvidos/min | 5.5/min | 4.9/min | 1.1x | Menor é melhor |
| Defesa de striking | 44% | 48% | 0.9x | Maior é melhor |
| Média sig. acertos/luta | 29 | 63 | 0.5x | Maior é melhor |
| % golpes na cabeça | 38% | 54% | 0.7x | Neutro |
| % golpes nas pernas | 32% | 24% | 1.3x | Neutro |
| Defesa de queda | 95% | 87% | 1.1x | Maior é melhor |

**O que isso revela:**

- Absorve mais golpes quando ganha (5.5/min vs 4.9/min) e com defesa pior (44% vs 48%). Aceita trocação aberta como parte do jogo; quando o adversário evita a troca, perde acesso ao contragolpe.
- Vitórias: distribuição equilibrada entre cabeça (38%), corpo (29%) e pernas (32%). Derrota: 54% na cabeça. Diversificação de alvos precede as vitórias.
- Média de 29 golpes sig. por luta nas vitórias vs 63 na derrota (0.5x). Vence com menos golpes -- resultado depende de timing e potência, não de volume. A derrota (5 rounds vs Garry) inflou o volume pelo tempo de luta.

---

<a name="prates-padroes-de-contexto"></a>
### Padrões de Contexto

#### Intervalo entre Lutas

| Situação | Intervalo Médio | N |
|----------|----------------|---|
| Antes de vitória | 95 dias | 5 |
| Antes de derrota | 168 dias | 1 |

#### Tendência Cronológica

| Fase | Lutas | Taxa Vitória |
|------|-------|-------------|
| Primeira metade (lutas 1-3) | 3 | 100% |
| Segunda metade (lutas 4-7) | 4 | 75% |

#### Migração de Alvos ao Longo da Carreira

| Fase | % Cabeça | % Corpo | % Pernas |
|------|----------|---------|----------|
| Primeira metade | 24% | 37% | 38% |
| Segunda metade | 53% | 21% | 26% |

**O que isso revela:**

- Intervalo antes da derrota (168 dias) foi 1.8x maior que antes das vitórias (95 dias). Amostra de derrotas: n=1.
- Inversão de estratégia na carreira: de corpo+pernas (75%) para cabeça (53%), com defesa de striking subindo de 39% para 48%.

---

<a name="prates-o-modelo-apm-vs-a-realidade"></a>
### O Modelo Ajustado vs a Realidade

Cruzamento entre o modelo ajustado por adversário e os dados brutos.

#### O Grande Paradoxo: Precisão e Defesa Invertidas

| Métrica | Valor Bruto | Ranking Ajustado | Efeito dos Oponentes |
|---------|-------------|---------------------|---------------------|
| Precisão de striking | 53% | Entre os 4% piores | Adversários cedem muita precisão (entre os 1% que mais cedem) |
| Defesa de striking | 44% | Entre os 4% melhores | Médio (oponentes são precisos) |
| Golpes sig./min | 4.0/min | Entre os 4% piores | Adversários cedem volume acima da média (entre os 16% que mais cedem) |

- Precisão bruta de 53% cai para entre os 4% piores da divisão após ajuste -- oponentes concedem alta precisão a qualquer um. A precisão real é menor do que os números brutos sugerem.
- Defesa bruta de 44% sobe para entre os 4% melhores após ajuste -- oponentes são strikers precisos acima da média. A defesa é melhor do que os números crus indicam.
- Volume de 4.0/min bruto cai para entre os 4% piores após ajuste. Não é lutador de volume quando se desconta o efeito dos oponentes.

#### O Mito do Chutador de Pernas

| Métrica | Valor Bruto | Ranking Ajustado | Efeito dos Oponentes |
|---------|-------------|---------------------|---------------------|
| Tentativas de chute perna/min | 1.4/min | Entre os 1% piores | Adversários defendem pouco esse ataque (entre os 14% que mais cedem) |
| % golpes nas pernas | 29% | Entre os 2% piores | Adversários cedem muito esse alvo (entre os 3% que mais cedem) |

- Números brutos sugerem que ele chuta pernas com frequência, mas os adversários costumam defender pouco esse ataque. Após ajuste, a tendência real de atacar pernas fica entre as mais baixas da divisão. Contra alguém que defenda bem essa faixa, esse volume pode cair bastante.

#### Dominância de Wrestling Defensivo

| Métrica | Ranking Ajustado | Interpretação |
|---------|---------------------|---------------|
| Defesa de queda | Entre os 4% melhores | Elite |
| Saldo de quedas | Entre os 4% melhores | Quase nunca é derrubado em relação ao esperado |
| % controle de luta | Entre os 6% melhores | Potencial de controle alto mas não utilizado |

- Tendência de controle de luta entre os 6% melhores (valor real: 5%). A capacidade de controlar existe, mas as lutas acabam antes de se materializar. Se forçado ao chão, pode ter mais recursos do que o histórico mostra.

#### Modelo Atualizado: Poder de KD Ajustado por Qualidade do Oponente

Modelo estatístico atualizado que mede cada performance considerando a qualidade do oponente. Modelos de comparação par-a-par posicionam Prates como classificado #1 a #4 em poder ofensivo de knockdown no UFC inteiro (melhor que 99.7% dos lutadores, atrás apenas de Tom Aspinall, Manuel Torres e Uros Medic).

**Top 5 performances positivas mais extraordinárias (índice de relevância):**

| Relevância | Metrica | Oponente | Observado | Esperado | O que significa |
|---------|---------|----------|-----------|----------|----------------|
| 5.04 | KD/min | Neil Magny | 0.41 | 0.16 | 2 KDs em 4.8 min contra oponente com defesa de KD 2.33x acima da média |
| 4.11 | % perna | Leon Edwards | 52% | 34% | % de pernas 1.5x acima do esperado contra Leon, que normalmente não recebe nessa taxa |
| 4.02 | KD/min | Li Jingliang | 0.33 | 0.21 | 3 KDs contra quem nunca havia caído em 62 min |
| 2.80 | Def. queda | Geoff Neal | 100% | 76% | 100% de defesa contra wrestler ofensivo |
| 2.72 | % corpo | Trevin Giles | 49% | 26% | 49% dos golpes no corpo vs 26% esperado — desvio de alvos |

**O caso Prates vs Leon no KD — o que os modelos dizem:**

Modelos de comparação par-a-par (com precisão de 92%) indicam probabilidade de 39-59% de Prates derrubar Leon. Leon nunca havia tomado KD porque seus oponentes anteriores tinham baixo poder de KD: Belal Muhammad (entre os 15% piores em KD), Colby Covington (entre os 22% piores), Gunnar Nelson (entre os 3% piores), Sean Brady (entre os 25% piores). Apenas Usman representava ameaça real e falhou 2x. Prates (#1-#4 em KD no UFC) entrava na faixa de maior probabilidade de conseguir esse KD.

**Precisão vs Leon (relevância 2.68):** 66% de precisão contra esperado de 50%, com Leon tendo defesa 16% acima da média.

**Top 5 piores performances reais (excluindo lutas que acabaram rápido em KO):**

| Relevância | Metrica | Oponente | Observado | Esperado | O que significa |
|---------|---------|----------|-----------|----------|----------------|
| -2.85 | Queda ritmo | Ian Machado Garry | -2.14 | -0.88 | Caiu de ritmo 2.4x mais que esperado — a única derrota |
| -2.63 | Controle | Charles Radtke | 1% | 17% | Sem jogo de chão mesmo vencendo |
| -2.45 | Reversões | Trevin Giles | 0 | 0.007/min | Não recupera posição quando vai ao chão |
| -2.43 | Saldo quedas | Leon Edwards | -0.31 | +0.04 | Leon derrubou e controlou — vulnerabilidade real no grappling |
| -2.06 | Def. striking | Trevin Giles | 33% | 54% | Absorveu muito golpe (mas venceu por KO) |

Fraquezas reais concentradas no chão: controle, reversões, queda de ritmo, defesa de queda em rounds tardios. Em pé domina; no grappling é vulnerável.

---

<a name="prates-lutas-anomalas"></a>
### Lutas Anômalas

Lutas onde Prates agiu completamente fora do padrão — desvios extremos no próprio histórico, detectados pelo modelo ajustado.

| Luta | Métrica | O que aconteceu | Desvio |
|------|---------|----------------|--------|
| vs Trevin Giles (2024) | Distribuição cabeça | Atacou 8% cabeça quando o esperado era 62% | -2.4x abaixo |
| vs Trevin Giles (2024) | Distribuição corpo | Atacou 49% corpo quando o esperado era 21% | +1.8x acima |
| vs Trevin Giles (2024) | Chutes de perna/min | 2.4/min vs esperado 0.8/min | +1.8x acima |
| vs Ian Machado Garry (2025) | Tempo de luta | 1500s vs esperado 686s | +2.2x acima |
| vs Leon Edwards (2025) | % golpes pernas | 52% vs esperado 19% | +1.8x acima |

**O que isso revela:**

- Contra Giles: abandonou cabeça (8% vs média de 50%), migrou para corpo (49%) e pernas. KO no R2. Variação radical de alvos como tática.
- Contra Edwards: pernas em 52% (vs média de 25-30%). As duas maiores vitórias de prestígio envolveram desvios radicais da estratégia habitual -- indica capacidade de adaptação tática sob demanda.
- Contra Garry: única luta com duração 2.2x acima do esperado, e única derrota. Ainda não mostrou um repertório equivalente quando a luta se prolonga.

---

<a name="prates-sinais-fracos-combinados"></a>
### Sinais Fracos Combinados

Métricas que sozinhas não chamam atenção, mas juntas formam um padrão.

- **Saldo de striking negativo (-0.1/min, entre os 13% piores quando ajustado) + knockdowns entre os 5% melhores:** Perde o jogo de volume, ganha o jogo de impacto. Saldo de striking subestima Prates porque trata todos os golpes como iguais.

- **% do tempo de luta utilizado entre os 19% piores + tempo de luta entre os 32% mais curtos:** Usa 1/5 do tempo disponível em média. 100% das vitórias UFC por KO/TKO, 0% por decisão. Sem histórico de vitória por outra via no UFC.

- **Oponentes tentam takedowns 87% acima da média nele + defesa de queda entre os 4% melhores quando ajustado:** Adversários sabem que precisam tirá-lo dos pés, mas quase ninguém consegue. Defesa de queda treinada para esse cenário.

- **Queda de ritmo entre rounds entre os 5% menores da divisão + volume que sobe R1 para R2:** Um dos que menos perde ritmo entre rounds na divisão. R1 para leitura, R2 para execução.

---

<a name="prates-visao-do-analista"></a>
### Visão do Analista

- Conforme detalhado na seção do modelo ajustado: precisão inflada pelos oponentes (entre os 4% piores quando ajustado), defesa melhor do que parece (entre os 4% melhores quando ajustado), e chutes nas pernas favorecidos por adversários que defendem pouco esse ataque (entre os 1% piores quando ajustado). Contra um oponente com boa defesa de striking e boa leitura desses chutes, os números brutos provavelmente superestimam esse lado do jogo dele.

- Padrão de vitória: menos volume, mais distribuição de alvos, aceita dano. Assinatura de contragolpeador. As lutas contra Giles e Edwards também mostram capacidade real de ajustar o plano de ataque quando necessário.

- Se a luta passar dos 2 rounds, ainda há pouca evidência de um plano vencedor alternativo no UFC. A única luta longa do recorte (vs Garry, 2.2x acima do esperado) terminou em derrota.

---

<a name="capitulo-4-insights-ocultos--jack-della-maddalena"></a>
## Capítulo 4: Insights Ocultos — Jack Della Maddalena

> Mesma metodologia de modelo ajustado do Capítulo 3 (Insights Ocultos — Carlos Prates). Os rankings abaixo mostram onde JDM se destaca ou é vulnerável quando se desconta o efeito dos oponentes.

<a name="jdm-onde-ele-e-extremo-na-categoria"></a>
### Onde Ele é Extremo na Categoria (Peso Meio-Médio)

Métricas onde Della Maddalena está entre os 10% melhores ou 10% piores da divisão — e que nenhum outro relatório menciona diretamente.

| Métrica | Valor | Posição | N da Categoria |
|---------|-------|---------|----------------|
| Defesa de striking (bruta) | 63% | Entre os 5% melhores | 84 |
| Vitórias no 1º round | 4 | Entre os 6% melhores | 84 |
| Vitórias por KO/TKO (carreira) | 12 | Entre os 9% melhores | 84 |

**O que isso revela:**

- Defesa de striking bruta de 63% (uma das quatro melhores marcas da divisão) combinada com 4 vitórias no R1 (melhor que 94% da divisão). Combinação rara de defesa e capacidade de finalização precoce.
- Porém, a seção do modelo ajustado mostra que essa defesa é parcialmente inflada pela qualidade dos oponentes.

---

<a name="jdm-o-paradoxo-das-vitorias-e-derrotas"></a>
### O Paradoxo das Vitórias e Derrotas

Métricas que se comportam ao contrário do esperado quando ele ganha vs quando ele perde.

| Métrica | Média Vitórias (n=8) | Média Derrota (n=1) | Ratio | Direção Esperada |
|---------|---------------------|---------------------|-------|-----------------|
| Golpes sig./min | 7.8/min | 0.7/min | 11.1x | Maior é melhor |
| Golpes sig. absorvidos/min | 4.4/min | 1.2/min | 3.7x | Menor é melhor |
| KD/5min | 1.2 | 0.0 | -- | Maior é melhor |
| % golpes na cabeça | 67% | 56% | 1.2x | Neutro |
| % golpes nas pernas | 9% | 11% | 0.8x | Neutro |
| Quedas sofridas/luta | 1.8 | 4.0 | 0.4x | Menor é melhor |

**O que isso revela:**

- Absorve mais golpes nas vitórias (4.4/min) do que na derrota (1.2/min) -- mesmo padrão de Prates. Trocação aberta favorece ambos os lutadores. Na derrota contra Makhachev, a troca praticamente não existiu (0.7/min de volume).
- Knockdowns: 1.2/5min nas vitórias vs 0.0 na derrota. Poder de nocaute depende de ter tempo em pé para se materializar.
- Quedas sofridas dobram na derrota (4.0 vs 1.8/luta). Quando o oponente derruba com consistência, o jogo de striking perde força.

---

<a name="jdm-padroes-de-contexto"></a>
### Padrões de Contexto

#### Distribuição por Método

| Método | Lutas | Vitórias |
|--------|-------|----------|
| KO/TKO | 4 | 4 |
| Decisão | 4 | 3 |
| Finalização | 1 | 1 |

#### Tendência Cronológica

| Fase | Lutas | Taxa Vitória |
|------|-------|-------------|
| Primeira metade (lutas 1-4) | 4 | 100% |
| Segunda metade (lutas 5-9) | 5 | 80% |

**O que isso revela:**

- Divisão equilibrada entre KO/TKO e decisão. Dois modos de operação distintos.
- Finalização contra Randy Brown (GnP no R1): único método alternativo, com a única tentativa significativa de submissão da carreira (desvio alto em relação ao padrão dele).

---

<a name="jdm-o-modelo-apm-vs-a-realidade"></a>
### O Modelo Ajustado vs a Realidade

#### O Grande Paradoxo: O Espelho Invertido de Prates

| Métrica | Valor Bruto | Ranking Ajustado | Efeito dos Oponentes |
|---------|-------------|---------------------|---------------------|
| Precisão de striking | 54% | Entre os 7% melhores | Baixo (adversários raramente cedem essa métrica) |
| Defesa de striking | 63% | Entre os 14% piores | Baixo (adversários costumam acertar pouco) |
| Volume total/min | 8.2/min | Entre os 10% melhores | Adversários cedem um pouco acima da média (entre os 14% que mais cedem) |

- Precisão bruta de 54% sobe para entre os 7% melhores da divisão após ajuste. Os adversários não costumam ceder precisão -- mérito do próprio Jack.
- Defesa bruta de 63% (entre os 5% melhores sem ajuste) cai para entre os 14% piores após ajuste. Em geral, os adversários dele acertam pouco mesmo contra outros rivais. Contra strikers precisos, essa defesa pode cair bastante.
- **Espelho de Prates:** Prates tem precisão inflada + defesa real. Della Maddalena tem precisão real + defesa inflada. Vulnerabilidades opostas.

#### Ataque ao Corpo como Marca

| Métrica | Ranking Ajustado | Interpretação |
|---------|---------------------|---------------|
| % golpes no corpo | Entre os 6% melhores | Ataque ao corpo elite |
| % golpes nas pernas | Entre os 9% piores | Quase não chuta pernas |
| % golpes a distância | Entre os 13% piores | Menos dependente de distância pura |
| % golpes no clinch | Entre os 13% melhores | Trabalha clinch acima da média |

- Entre os 6% melhores em ataque ao corpo, confirmado como desvio significativo em 3 lutas: Roberts (4x esperado), Emeev (3.2x), Holland (2.7x).
- Corpo entre os 6% melhores + pernas entre os 9% piores: mapa de alvos é cabeça + corpo, quase zero pernas. Inverso dos strikers que usam o chute baixo como base do jogo.
- Clinch entre os 13% melhores: atua bem em média-curta. A precisão alta pode estar ligada a golpear de mais perto.

#### Potencial de Controle Pouco Usado

| Métrica | Ranking Ajustado | Valor Bruto | Interpretação |
|---------|-------------|-------------|---------------|
| % controle de luta | Entre os 2% melhores | 5% | Potencial máximo, uso mínimo |
| % do tempo de luta utilizado | Entre os 2% melhores | 63% | Luta a luta inteira |
| Tempo de luta | Entre os 4% melhores | 699s média | Tendência a lutas longas |

- Tendência de controle entre os 2% melhores (segundo mais alto entre 84 meio-médios), mas controle real de apenas 5%. Potencial não utilizado porque o striking resolve antes.
- % do tempo de luta utilizado entre os 2% melhores: usa 63% do tempo disponível (vs 50% da divisão). Diferente de Prates, ocupa o octógono por mais tempo mantendo eficiência.

#### Modelo Atualizado: Desempenhos Ajustados por Qualidade do Oponente

Modelo estatístico atualizado que mede cada performance considerando a qualidade do oponente, aplicado a Della Maddalena.

**Top 4 performances positivas mais extraordinárias (índice de relevância):**

| Relevância | Metrica | Oponente | Observado | Esperado | O que significa |
|---------|---------|----------|-----------|----------|----------------|
| 5.55 | Sub/min | Randy Brown | 0.45 | 0.26 | Unica luta com tentativas de finalizacao relevantes — venceu por GnP |
| 4.64 | Golpes sig./min | Kevin Holland | 7.0 | 3.4 | Volume 2x acima do esperado contra oponente com defesa 24% acima da média |
| 4.52 | KD/min | Ramazan Emeev | 0.39 | 0.21 | KD contra oponente com defesa de KD 2.44x acima da média |
| 4.24 | KD/min | Randy Brown | 0.45 | 0.16 | KD rapido contra oponente com historico defensivo solido |

**Insight chave:** KD contra Emeev (relevância 4.52) -- defesa de KD do Emeev 2.44x acima da média. JDM conseguiu 1 KD em 2.5 min e nocauteou. Poder de KD ofensivo posicionado entre os 13% melhores da divisão (modelos de comparação par-a-par), abaixo de Prates (melhor que 99.7% da divisão). Poder dele vem de volume e precisão, não de impacto puro.

**Top 5 piores performances reais (excluindo lutas que acabaram rápido em KO):**

| Relevância | Metrica | Oponente | Observado | Esperado | O que significa |
|---------|---------|----------|-----------|----------|----------------|
| -4.92 | % perna | Pete Rodriguez | 0% | 16% | Zero chutes nas pernas — reforça que esse golpe quase não entra no jogo dele |
| -2.98 | Controle | Pete Rodriguez | 1% | 19% | Sem trabalho de chão mesmo dominando |
| -2.84 | Saldo quedas | Gilbert Burns | -0.51 | -0.10 | Burns derrubou pesado — 7 TDs em 11 tentativas |
| -2.80 | % distância | Randy Brown | 36% | 75% | Lutou maioria no clinch, não na distância — adaptação tática |
| -2.62 | % cabeça | Islam Makhachev | 56% | 63% | Pouco acesso à cabeça com pressão de grappling constante |

Padrão negativo: não chuta pernas (entre os 9% piores quando ajustado, relevância -4.92), não controla no chão, saldo de quedas desaba contra grapplers de elite. Diferença em relação a Prates: tem plano B de volume e decisão (metade das vitórias UFC).

---

<a name="jdm-lutas-anomalas"></a>
### Lutas Anômalas

Lutas onde Della Maddalena agiu completamente fora do padrão.

| Luta | Métrica | O que aconteceu | Desvio |
|------|---------|----------------|--------|
| vs Pete Rodriguez (2022) | Volume sig./min | 14.4/min vs média 8.8/min | +2.1x acima |
| vs Pete Rodriguez (2022) | Tentativas distância/min | 26.1/min vs esperado 7.4/min | +3.7x acima (ajustado) |
| vs Danny Roberts (2022) | Golpes corpo/min | 4.7/min vs esperado 1.2/min | +3.3x acima (ajustado) |
| vs Randy Brown (2023) | Tentativas de submissão | 0.45/min vs esperado 0.04/min | +2.9x acima (ajustado) |
| vs Burns (2024) | Saldo de quedas | -0.51/min vs esperado 0.00/min | -1.9x abaixo (ajustado) |

**O que isso revela:**

- Pete Rodriguez: volume 3.7x acima do esperado após ajuste, quase tudo a distância. Maior desvio positivo de volume de striking.
- Danny Roberts: corpo 3.3x acima do esperado, consistente com o padrão forte de ataque ao corpo dele. Defesa de striking nessa luta: 85%, bem acima do padrão habitual.
- Randy Brown: submissão com desvio alto -- único desvio significativo para grappling ofensivo. Recurso disponível mas raramente ativado.

---

<a name="jdm-sinais-fracos-combinados"></a>
### Sinais Fracos Combinados

Métricas que sozinhas não chamam atenção, mas juntas formam um padrão.

- **Reversões entre os 4% piores (quando ajustado) + defesa de queda binária (0% a 85%):** Não reverte posição quando derrubado. Defesa de queda funciona antes do chão ou não funciona -- sem meio-termo. Contra Burns, compensou com striking entre as quedas. Contra Islam, não teve essa chance.

- **Volume entre os 10% melhores (quando ajustado) + knockdowns entre os 13% melhores:** Volume alto, mas poder de nocaute bom sem ser elite quando se desconta o efeito dos oponentes. Desgasta mais do que nocauteia, explicando as decisões.

- **Precisão entre os 7% melhores + corpo entre os 6% melhores + clinch entre os 13% melhores + distância entre os 13% piores:** Atua melhor em média-curta, com precisão de elite. Essa faixa pode ser explorada por lutadores com jab e footwork que consigam manter distância.

- **% do tempo de luta utilizado entre os 2% melhores + tempo entre os 4% mais longos:** Precisão alta mantida sob volume alto ao longo de 63% do tempo disponível. Cardio técnico como diferencial.

---

<a name="jdm-visao-do-analista"></a>
### Visão do Analista

- Conforme seção do modelo ajustado: defesa de striking inflada (63% bruto, entre os 14% piores quando ajustado) e precisão real (entre os 7% melhores quando ajustado). Prates, com precisão real quando ajustada e potência de knockdown fora da curva no UFC, é o tipo de oponente que testa diretamente a fragilidade defensiva de JDM.

- Prioridade para a equipe do Prates: proteção de corpo. Ataque ao corpo forte e recorrente, confirmado em 3 lutas com desvios claros acima do padrão. Ignorar esse caminho aqui seria erro de leitura do adversário.

- Reversões entre os 4% piores e defesa de queda binária são a vulnerabilidade principal, mas Prates não tem wrestling ofensivo para explorar isso (entre os 5% piores em tentativas de queda). Esse gap de JDM é mais relevante contra grapplers.

- JDM opera como lutador de volume com precisão alta, mas também tem poder para interromper quando encontra espaço. O diferencial mais estável dele é sustentar ritmo e precisão ao longo da luta. A questão para esta luta é se Prates consegue nocautear antes que esse ritmo se imponha, algo que costuma aparecer a partir do R2-R3.

---

<a name="capitulo-5-analise-subjetiva--carlos-prates"></a>
## Capítulo 5: Análise Subjetiva Luta a Luta — Carlos Prates

<a name="prates-sub-medias-de-carreira"></a>
### Médias de Carreira

| Métrica | Média dele |
|---------|:---------:|
| Golpes Sig. Conectados/min | 3.77 |
| Golpes Sig. Absorvidos/min | 4.53 |
| Precisão Striking | 55% |
| Defesa Striking | 47% |
| Knockdowns/15min | 2.13 |
| Quedas Aplicadas/15min | 0.21 |
| Precisão de Quedas | 100% |
| Defesa de Quedas | 80% |
| Tentativas de Sub/15min | 0.0 |

> `ufc_lutadores_detalhes` → `slpm_conectados_min`, `sapm_absorvidos_min`, `perc_precisao_striking`, `perc_defesa_striking`, `media_knockdowns_15min`, `media_quedas_15min`, `perc_precisao_quedas`, `perc_defesa_quedas`, `media_finalizacoes_15min`

> Base de comparação. Nos bullets de cada luta, destacamos desvios deste padrão.

---

<a name="prates-sub-resumo-do-recorte"></a>
### Resumo do Recorte

- Lutas analisadas: 5 (4 vitórias + 1 derrota)
- Período: 17/08/2024 a 15/11/2025
- Dados detalhados (lutador + oponente) disponíveis em 5 de 5 lutas
- Dados round a round disponíveis em 5 de 5 lutas

---

<a name="prates-sub-vitorias-recentes"></a>
### Vitórias Recentes

#### 1. vs Leon Edwards — UFC 312 (15/11/2025)
**KO/TKO | R2 1:28 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Carlos Prates | Leon Edwards |
|---------|:---------:|:----------:|
| Golpes Sig. Conectados | 21 | 12 |
| Golpes Sig. Tentados | 32 | 17 |
| Precisão Sig. Striking | 66% | 71% |
| Knockdowns | 1 | 0 |
| Golpes Totais Conectados | 24 | 25 |
| Golpes Totais Tentados | 35 | 30 |
| Quedas Aplicadas / Tentadas | 0/0 | 2/3 |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:01 | 3:00 |
| Controle (%) | 0% | 46% |

> `ufc_lutas_detalhes` → `ufc_total_kd`, `ufc_total_sig_str_acertos`, `ufc_total_sig_str_tentativas`, `ufc_total_sig_str_pct`, `ufc_total_tot_str_acertos`, `ufc_total_tot_str_tentativas`, `ufc_total_td_acertos`, `ufc_total_td_tentativas`, `ufc_total_sub_tentativas`, `ufc_total_ctrl_tempo`, `ufc_total_ctrl_pct`

##### Análise Subjetiva

- Precisão de 66% contra a média de 55% — 11 pontos acima do normal dele. E contra um cara com 71% de defesa bruta. Leon cedeu controle de 46% do tempo e ainda assim não conseguiu capitalizar no chão. O Prates resolveu em 88 segundos de R2 o que Leon segurou por 5 minutos de R1.

- Volume no R1 foi tímido: 1.8 sig/min, metade da média dele de 3.77. No R2 saltou para 8.18/min — mais que o dobro. O padrão de R1 como leitura e R2 como execução ficou mais claro aqui do que em qualquer outra luta.

- 52% dos golpes significativos foram nas pernas (11 de 21). A média de carreira dele é 25% nas pernas. Mudou o mapa de alvos radicalmente contra um cara que ninguém costumava atacar assim. A adaptação tática não foi acidente.

---

#### 2. vs Geoff Neal — UFC Fight Night (16/08/2025)
**KO/TKO | R1 4:59 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Carlos Prates | Geoff Neal |
|---------|:---------:|:----------:|
| Golpes Sig. Conectados | 32 | 25 |
| Golpes Sig. Tentados | 60 | 49 |
| Precisão Sig. Striking | 53% | 51% |
| Knockdowns | 1 | 0 |
| Golpes Totais Conectados | 32 | 26 |
| Golpes Totais Tentados | 60 | 50 |
| Quedas Aplicadas / Tentadas | 0/0 | 0/1 |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:00 | 0:15 |
| Controle (%) | 0% | 5% |

> `ufc_lutas_detalhes` → `ufc_total_kd`, `ufc_total_sig_str_acertos`, `ufc_total_sig_str_tentativas`, `ufc_total_sig_str_pct`, `ufc_total_tot_str_acertos`, `ufc_total_tot_str_tentativas`, `ufc_total_td_acertos`, `ufc_total_td_tentativas`, `ufc_total_sub_tentativas`, `ufc_total_ctrl_tempo`, `ufc_total_ctrl_pct`

##### Análise Subjetiva

- 6.42 sig/min — 70% acima da média de 3.77. Essa foi a luta de maior volume por minuto entre as 4 vitórias recentes. Tentativas de 12.04/min, quase o triplo do que tentou contra Edwards. O Prates abriu a guarda e saiu atirando de um jeito que não repete em todo fight.

- Neal absorveu 5.02/min e conectou 51% — foi uma trocação real. A defesa do Prates ficou em 49% (próxima da média de 47%), mas o saldo terminou positivo em +1.4/min. O KO saiu dentro de uma guerra equilibrada nos números, não de uma dominação.

- Distribuição de alvos mais limpa que o normal: 53% cabeça, 25% corpo, 22% pernas. Próxima do padrão de vitórias dele. Contra Neal, não precisou desviar muito do perfil habitual pra resolver.

---

#### 3. vs Neil Magny — UFC 309 (09/11/2024)
**KO/TKO | R1 4:50 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Carlos Prates | Neil Magny |
|---------|:---------:|:----------:|
| Golpes Sig. Conectados | 12 | 10 |
| Golpes Sig. Tentados | 21 | 20 |
| Precisão Sig. Striking | 57% | 50% |
| Knockdowns | 2 | 0 |
| Golpes Totais Conectados | 13 | 23 |
| Golpes Totais Tentados | 22 | 33 |
| Quedas Aplicadas / Tentadas | 1/1 | 0/7 |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 1:09 | 1:31 |
| Controle (%) | 24% | 31% |

> `ufc_lutas_detalhes` → `ufc_total_kd`, `ufc_total_sig_str_acertos`, `ufc_total_sig_str_tentativas`, `ufc_total_sig_str_pct`, `ufc_total_tot_str_acertos`, `ufc_total_tot_str_tentativas`, `ufc_total_td_acertos`, `ufc_total_td_tentativas`, `ufc_total_sub_tentativas`, `ufc_total_ctrl_tempo`, `ufc_total_ctrl_pct`

##### Análise Subjetiva

- 2 knockdowns em 12 golpes significativos. A média dele é 2.13 KD por 15 minutos — aqui fez 2 em menos de 5. O ratio de 1 KD a cada 6 golpes sig é absurdo. Magny tem defesa de queda sólida (0/7 tentativas de queda dele falharam), mas não aguentou o poder puro.

- Volume de 2.48 sig/min — 34% abaixo da média de 3.77. Mas controlou 24% do tempo com 1 queda em 1 tentativa. Única luta das 4 vitórias onde ele aplicou takedown e trabalhou controle. Um Prates diferente aparece quando o oponente pressiona com wrestling e falha.

- Magny tentou 7 quedas e não converteu nenhuma. Defesa de 100% contra a média dele de 80%. Contra o cara com mais tentativas de queda entre as 4 vitórias, o Prates foi perfeito na defesa.

---

#### 4. vs Li Jingliang — UFC Fight Night (17/08/2024)
**KO/TKO | R2 4:02 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Carlos Prates | Li Jingliang |
|---------|:---------:|:----------:|
| Golpes Sig. Conectados | 55 | 41 |
| Golpes Sig. Tentados | 84 | 111 |
| Precisão Sig. Striking | 65% | 37% |
| Knockdowns | 3 | 0 |
| Golpes Totais Conectados | 55 | 41 |
| Golpes Totais Tentados | 84 | 111 |
| Quedas Aplicadas / Tentadas | 0/0 | 0/0 |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:04 | 0:23 |
| Controle (%) | 1% | 4% |

> `ufc_lutas_detalhes` → `ufc_total_kd`, `ufc_total_sig_str_acertos`, `ufc_total_sig_str_tentativas`, `ufc_total_sig_str_pct`, `ufc_total_tot_str_acertos`, `ufc_total_tot_str_tentativas`, `ufc_total_td_acertos`, `ufc_total_td_tentativas`, `ufc_total_sub_tentativas`, `ufc_total_ctrl_tempo`, `ufc_total_ctrl_pct`

##### Análise Subjetiva

- 3 knockdowns numa luta — a média dele é 2.13 por 15 minutos, aqui fez 3 em 9 minutos. Jingliang tentou 111 golpes significativos e conectou 37%. O Prates absorveu o volume todo e respondeu com precisão de 65% — 10 pontos acima do normal. A troca aberta é exatamente onde ele mata.

- Migração clara entre rounds: R1 a 5.0 sig/min com saldo de -0.2 (perdendo). R2 saltou para 7.44/min com saldo de +3.72. A precisão do Jingliang desabou de 39% para 33%. O Prates leu a luta no primeiro round e executou no segundo.

- 80% dos golpes na cabeça (44 de 55), contra a média de carreira de 54%. Contra Jingliang, foi quase tudo pra cima. A variação de alvos que normalmente marca as vitórias dele não apareceu aqui — e ainda assim nocauteou. Às vezes a potência pura compensa.

---

<a name="prates-sub-derrotas-recentes"></a>
### Derrotas Recentes

#### 1. vs Ian Machado Garry — UFC (26/04/2025)
**Decisão | R5 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Carlos Prates | Ian Machado Garry |
|---------|:---------:|:----------:|
| Golpes Sig. Conectados | 63 | 126 |
| Golpes Sig. Tentados | 129 | 242 |
| Precisão Sig. Striking | 49% | 52% |
| Knockdowns | 0 | 0 |
| Golpes Totais Conectados | 64 | 141 |
| Golpes Totais Tentados | 132 | 259 |
| Quedas Aplicadas / Tentadas | 0/0 | 4/19 |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 1:46 | 3:09 |
| Controle (%) | 7% | 13% |

> `ufc_lutas_detalhes` → `ufc_total_kd`, `ufc_total_sig_str_acertos`, `ufc_total_sig_str_tentativas`, `ufc_total_sig_str_pct`, `ufc_total_tot_str_acertos`, `ufc_total_tot_str_tentativas`, `ufc_total_td_acertos`, `ufc_total_td_tentativas`, `ufc_total_sub_tentativas`, `ufc_total_ctrl_tempo`, `ufc_total_ctrl_pct`

##### Análise Subjetiva

- 0 knockdowns em 25 minutos — a média dele é 2.13 por 15 minutos. Em nenhuma das 4 vitórias analisadas ele ficou zerado. A ausência de KD não é só estatística, é o sinal de que o poder que define as vitórias dele simplesmente não apareceu.

- Volume de 2.52 sig/min contra a média de 3.77 — 33% abaixo do normal. Mas o dado que mata: saldo de -2.52/min. Nas 4 vitórias, o pior saldo foi +0.41 contra Magny. Aqui foi negativo de sobra. Garry não precisou nocautear — bastou produzir volume consistente que o Prates não conseguiu acompanhar.

- A queda de ritmo entre rounds foi de -2.14, contra a média de -0.13 das 4 vitórias. No R1 conectou 1.4/min, no R2 subiu para 2.4, mas a partir do R3 estagnou enquanto Garry acelerava. O R2 costuma ser o round de execução dele — aqui, a execução não veio.

- Garry tentou 19 quedas e converteu 4. A defesa do Prates ficou em 79% (próxima da média de 80%), mas o controle do Garry subiu de 4% no R1 para 28% no R3 e 19% no R4. Não foi a queda em si — foi a pressão posicional acumulada que tirou o Prates do jogo dele.

---

<a name="prates-sub-padroes-transversais"></a>
### Padrões Transversais

#### Nas Vitórias

- As 4 vitórias somam 1419 segundos de luta (média de 355 segundos). A derrota durou 1500 segundos sozinha. Todas as vitórias terminaram em KO/TKO entre o R1 e o R2. O Prates tem uma janela de operação clara e curta — quando ela fecha, não há plano B registrado no UFC.

- O saldo de striking foi positivo nas 4 vitórias (+0.41 a +1.55/min) com knockdowns em todas. Na derrota, saldo de -2.52 e 0 KD. A correlação entre saldo positivo e nocaute é quase perfeita nesse recorte: quando ganha o jogo de trocação, finaliza; quando perde, não tem outra rota.

#### Vitórias vs Derrota — O que muda?

- Precisão média nas vitórias: 60%. Na derrota: 49%. A queda de 11 pontos coincide com uma mudança no perfil de alvos: 80% cabeça contra Jingliang, 75% contra Magny — mas contra Garry, 60% cabeça com 14% pernas (contra 25% da média). Quando a diversificação de alvos sumiu, a precisão acompanhou.

- Defesa de queda nas vitórias: 100% contra Magny, 100% contra Neal. Na derrota: 79% nominalmente, mas com Garry acumulando controle crescente ao longo dos rounds. O número bruto de defesa de queda esconde a erosão posicional que acontece quando a luta se alonga.

---

<a name="prates-sub-visao-do-coach"></a>
### Visão do Coach

#### O que os dados sugerem

- O Prates opera num modo binário: ou nocauteia até o R2, ou a luta escapa. Nas 4 vitórias, média de 5.9 minutos. Na derrota, 25 minutos. Não existe meio-termo nos dados recentes — nenhuma vitória sequer passou do R2.

- O R2 como round de execução é o padrão mais consistente: contra Jingliang subiu de 5.0 para 7.44/min, contra Edwards de 1.8 para 8.18/min. A leitura de R1 seguida de explosão no R2 aparece em todas as vitórias de 2 rounds. Se o oponente neutralizar o R2, entra em território desconhecido pro Prates.

#### Pontos de atenção

- Contra Garry, a queda de ritmo de -2.14 foi a pior de toda a amostra. Nas vitórias, a média foi -0.13. A degradação a partir do R3 não é gradual — é um despenhadeiro. Se a preparação física não mudou desde a luta com Garry, rounds tardios continuam sendo a zona de risco.

- 0 tentativas de finalização em todas as 5 lutas. 0 reversões. Quando vai ao chão, fica lá. O wrestling defensivo funcionou (100% vs Magny, 100% vs Neal), mas quando falha, não há recurso. Esse gap fica exposto contra qualquer oponente que consiga manter a pressão de queda por mais de 2 rounds.

---

<a name="capitulo-6-analise-subjetiva--jack-della-maddalena"></a>
## Capítulo 6: Análise Subjetiva Luta a Luta — Jack Della Maddalena

> Luta por luta, round por round — o que Jack fez de diferente em cada vitória e onde ele quebrou na derrota. Dados objetivos seguidos de leitura analítica.

### Médias de Carreira

| Métrica | Média dele |
|---------|:---------:|
| Golpes Sig. Conectados/min | 5.57 |
| Golpes Sig. Absorvidos/min | 3.84 |
| Precisão Striking | 51% |
| Defesa Striking | 63% |
| Knockdowns/5min | 0.3 |
| Quedas Aplicadas/5min | 0.04 |
| Precisão de Quedas | 10% |
| Defesa de Quedas | 64% |
| Tentativas de Sub/5min | 0.03 |

> Base de comparação. Nos bullets de cada luta, destacamos desvios deste padrão.

---

### Resumo do Recorte

- Lutas analisadas: 5 (4 vitórias + 1 derrota)
- Período: 15/07/2023 a 15/11/2025
- Dados detalhados (lutador + oponente) disponíveis em 5 de 5 lutas
- Dados round a round disponíveis em 5 de 5 lutas

---

### Vitórias Recentes

#### 1. vs Belal Muhammad — UFC 315 (10/05/2025)
**Decisão | R5 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Della Maddalena | Belal Muhammad |
|---------|:---------------:|:--------------:|
| Golpes Sig. Conectados | 178 | 132 |
| Golpes Sig. Tentados | 342 | 318 |
| Precisão Sig. Striking | 52% | 42% |
| Knockdowns | 0 | 0 |
| Golpes Totais Conectados | 200 | 155 |
| Golpes Totais Tentados | 364 | 349 |
| Quedas Aplicadas / Tentadas | 0/3 | 3/9 |
| Precisão de Quedas | 0% | 33% |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:40 | 3:21 |
| Controle (%) | 3% | 13% |

##### Análise Subjetiva

- 7.12 golpes sig./min (28% acima da média de 5.57/min), com ritmo crescente: 5.6/min no R1 a 10.6/min no R5. Acelerou conforme identificou o cansaço do oponente.
- Defesa de quedas de 67% (próxima da média de 64%), mas Muhammad tentou 9 vezes com 3:21 de controle vs 0:40 de Jack. Venceu no striking puro apesar de perder o grappling.
- R5: 53 golpes sig. em 5 minutos com 64% de precisão, contra 44-56% nos rounds anteriores. Performance de cardio consolidada nos rounds finais.

---

#### 2. vs Gilbert Burns — UFC 299 (09/03/2024)
**KO/TKO | R3 3:43 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Della Maddalena | Gilbert Burns |
|---------|:---------------:|:-------------:|
| Golpes Sig. Conectados | 67 | 27 |
| Golpes Sig. Tentados | 123 | 58 |
| Precisão Sig. Striking | 54% | 47% |
| Knockdowns | 1 | 0 |
| Golpes Totais Conectados | 85 | 31 |
| Golpes Totais Tentados | 146 | 63 |
| Quedas Aplicadas / Tentadas | 0/1 | 7/11 |
| Precisão de Quedas | 0% | 64% |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:16 | 5:07 |
| Controle (%) | 2% | 37% |

##### Análise Subjetiva

- Burns: 7 quedas em 11 tentativas, 5:07 de controle -- e perdeu. Jack a 4.88 sig./min (abaixo da média de 5.57), mas com saldo de +2.92/min sobre Burns. O striking em pé compensou o domínio no solo.
- R3 decisivo: de 4.2/min (R2) para 7.53/min, precisão de 44% para 76%. 16 dos 67 golpes sig. foram no chão -- maior volume no solo entre as 4 vitórias analisadas.
- Defesa de quedas de 36% (vs média de 64%). Burns foi mais eficiente que os oponentes habituais, mas o KO no R3 veio quando Jack encontrou espaço para golpear em pé.

---

#### 3. vs Kevin Holland — UFC Fight Night: Grasso vs. Shevchenko 2 (16/09/2023)
**Decisão | R3 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Della Maddalena | Kevin Holland |
|---------|:---------------:|:-------------:|
| Golpes Sig. Conectados | 105 | 127 |
| Golpes Sig. Tentados | 190 | 356 |
| Precisão Sig. Striking | 55% | 36% |
| Knockdowns | 0 | 0 |
| Golpes Totais Conectados | 105 | 127 |
| Golpes Totais Tentados | 190 | 356 |
| Quedas Aplicadas / Tentadas | 0/0 | 0/2 |
| Precisão de Quedas | -- | 0% |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:00 | 0:00 |
| Controle (%) | 0% | 0% |

##### Análise Subjetiva

- Holland: 356 tentativas vs 190 de Jack, mas Jack conectou 55% contra 36% de Holland. Volume conectado próximo (105 vs 127), com metade do esforço. Eficiência decidiu.
- Saldo de -1.47/min -- única vitória com saldo negativo. Holland era difícil de parar e manteve pressão de volume que impediu a finalização.
- Desaceleração progressiva: 8.2/min (R1), 6.8/min (R2), 6.0/min (R3). No R2 migrou para corpo e pernas (41% e 29%) antes de voltar à cabeça no R3.

---

#### 4. vs Bassil Hafez — UFC Fight Night: Holm vs. Bueno Silva (15/07/2023)
**Decisão | R3 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Della Maddalena | Bassil Hafez |
|---------|:---------------:|:------------:|
| Golpes Sig. Conectados | 83 | 32 |
| Golpes Sig. Tentados | 137 | 124 |
| Precisão Sig. Striking | 61% | 26% |
| Knockdowns | 0 | 0 |
| Golpes Totais Conectados | 149 | 48 |
| Golpes Totais Tentados | 212 | 141 |
| Quedas Aplicadas / Tentadas | 1/2 | 3/20 |
| Precisão de Quedas | 50% | 15% |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 1:19 | 6:48 |
| Controle (%) | 9% | 45% |

##### Análise Subjetiva

- Precisão de 61% (10pp acima da média de 51%), saldo de +3.40/min -- maior entre as quatro vitórias analisadas. Hafez tentou 20 quedas, converteu 3. No R3: 8.6/min com 63% de precisão, mesmo cedendo 70 segundos de controle.
- 6:48 de controle de Hafez, mas Jack ganhou os três rounds no striking. Defesa de quedas em 85% (vs média de 64%) -- ajustou posicionamento ao longo da luta.
- Aceleração progressiva: 2.6/min (R1), 5.4/min (R2), 8.6/min (R3). Mesmo padrão da vitória sobre Muhammad.

---

### Derrotas Recentes

#### 1. vs Islam Makhachev — UFC 322 (15/11/2025)
**Decisão | R5 5:00 | Peso Meio-Médio**

##### Dados Objetivos

| Métrica | Della Maddalena | Islam Makhachev |
|---------|:---------------:|:---------------:|
| Golpes Sig. Conectados | 18 | 30 |
| Golpes Sig. Tentados | 61 | 57 |
| Precisão Sig. Striking | 30% | 53% |
| Knockdowns | 0 | 0 |
| Golpes Totais Conectados | 30 | 140 |
| Golpes Totais Tentados | 74 | 188 |
| Quedas Aplicadas / Tentadas | 0/1 | 4/4 |
| Precisão de Quedas | 0% | 100% |
| Tentativas de Submissão | 0 | 0 |
| Controle (tempo) | 0:00 | 19:10 |
| Controle (%) | 0% | 77% |

##### Análise Subjetiva

- 0.72 golpes sig./min (87% abaixo da média de 5.57). Makhachev: 4 quedas em 4 tentativas, 19:10 de controle em 25 minutos (77% do tempo). Striking de Jack neutralizado.
- R4: 1 golpe sig. em 11 tentativas (0.2/min, 9% precisão). Defesa de quedas de 0%. A pressão de grappling corrompeu o timing de striking mesmo nos momentos em pé.
- Golpes totais: Makhachev 140, Jack 30. Controle de Jack: zero. Nas vitórias anteriores (mesmo contra Burns e Hafez), sempre teve algum volume de resposta.

---

### Padrões Transversais

#### Nas Vitórias

- Volume de striking cresce ao longo dos rounds nas lutas que vão a decisão (Muhammad: 5.6 a 10.6/min; Hafez: 2.6 a 8.6/min; Burns: R3 com mais que o dobro dos rounds anteriores). Padrão de aceleração progressiva consistente.
- Nas três vitórias com dados de quedas, terminou negativo no saldo de quedas mas venceu todas. O striking em pé compensou o grappling cedido. Essa equação tem um limite, que a derrota para Makhachev expôs.

#### Nas Derrotas

- Uma derrota no recorte: com conversão de takedown a 100% e controle acima de 75% do tempo total, o striking de Jack foi neutralizado como fator.

#### Vitórias vs Derrota — O que muda?

- A diferença está na capacidade de criar espaço para golpear. Contra Burns, Hafez e Muhammad, manteve volumes relevantes em pé. Contra Makhachev, o grappling reduziu o striking a 0.72/min.
- Defesa de quedas nas vitórias: 36% (Burns) a 85% (Hafez). Na derrota: 0%. O diferencial de Makhachev não foi só a conversão de quedas (100%), mas a manutenção do controle após derrubar (19:10 no total).

---

### Visão do Analista

#### O que os dados sugerem

- Jack acelera ao longo dos rounds, mas esse rendimento depende de tempo em pé. O ponto de desenvolvimento mais claro é a transição defesa de queda para retomada de posição -- não quedas isoladas, mas sequências.
- Precisão de 51% de média, chegando a 55-61% com espaço. A qualidade do striking não é o problema; o acesso a ele é.

#### Pontos de atenção

- Derrota para Makhachev: 0.72/min de striking, 0% de defesa de quedas, 0 segundos de controle. O recorte sugere que grapplers de elite conseguem reduzir bastante o volume dele em pé.
- Vitória sobre Holland com saldo negativo (-1.47/min): Holland impôs 356 tentativas em 3 rounds. Um oponente com volume alto de striking combinado com grappling pode exceder a margem que Jack normalmente mantém.

---

<a name="capitulo-7-analise-round-a-round--carlos-prates"></a>
## Capítulo 7: Análise Round a Round — Carlos Prates

> Como Prates se comporta em cada round — volume, precisão, knockdowns, grappling. Os dados que mostram onde ele acelera e onde fica vulnerável conforme a luta avança.

### Perfil Geral
- Total de lutas analisadas: 7
- Categoria: Peso Meio-Médio
- Resultado geral: 6V-1D
- Vitórias por método: 6 KO/TKO
- Derrotas por método: 1 Decisão
- Lutas com dados de rounds 4-5: 1 (vs Ian Machado Garry)

### Dados Frios — Médias por Round

#### Striking

| Métrica | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
|---------|----------|----------|----------|----------|----------|
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
|---------|----------|----------|----------|----------|----------|
| Quedas conectadas/5min | 0.1 | 0.0 | 0.0 | 0.0 | 0.0 |
| Quedas oponente/5min | 0.3 | 0.0 | 2.0 | 2.0 | 0.0 |
| Defesa de queda (%) | 87% | 100% | 33% | 71% | 100% |
| Controle (%) | 4% | 3% | 6% | 0% | 20% |
| Controle oponente (%) | 15% | 11% | 28% | 19% | 11% |
| Dominância controle (%) | 29% | 52% | 18% | 0% | 64% |

#### Saldos

| Métrica | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
|---------|----------|----------|----------|----------|----------|
| Saldo sig./min | -0.2 | -0.2 | -3.2 | -2.2 | -1.2 |
| Saldo quedas/5min | -0.1 | 0.0 | -2.0 | -2.0 | 0.0 |
| Saldo controle (pp) | -12pp | -9pp | -22pp | -19pp | +9pp |

### Dados Frios — Variações Médias Round a Round

#### Striking

| Métrica | R1→R2 (n=4) | R2→R3 (n=1) | R3→R4 (n=1) | R4→R5 (n=1) |
|---------|-------------|-------------|-------------|-------------|
| Δ Golpes sig./min | +2.1 | -0.4 | +0.4 | +2.0 |
| Δ Tentativas sig./min | +2.7 | -0.4 | +2.6 | +1.0 |
| Δ Precisão sig. (pp) | +6pp | -5pp | -14pp | +22pp |
| Δ Knockdowns/5min | +1.5 | 0.0 | 0.0 | 0.0 |

#### Saldos

| Métrica | R1→R2 (n=4) | R2→R3 (n=1) | R3→R4 (n=1) | R4→R5 (n=1) |
|---------|-------------|-------------|-------------|-------------|
| Δ Saldo sig./min | +0.7 | +1.2 | +1.0 | +1.0 |
| Δ Saldo quedas/5min | +0.5 | -2.0 | 0.0 | +2.0 |
| Δ Saldo controle (pp) | +7pp | -30pp | +3pp | +28pp |
| Δ Controle (pp) | +2pp | -2pp | -6pp | +20pp |

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos -- Prates (%)

| Alvo | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
|------|----------|----------|----------|----------|----------|
| Cabeça | 42% | 44% | 60% | 75% | 77% |
| Corpo | 20% | 26% | 40% | 17% | 23% |
| Perna | 38% | 30% | 0% | 8% | 0% |

#### Alvos -- Oponentes (%)

| Alvo | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
|------|----------|----------|----------|----------|----------|
| Cabeça | 46% | 46% | 73% | 65% | 79% |
| Corpo | 13% | 5% | 15% | 13% | 7% |
| Perna | 41% | 49% | 12% | 22% | 14% |

#### Posição -- Prates (%)

| Posição | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
|---------|----------|----------|----------|----------|----------|
| Distância | 96% | 98% | 100% | 100% | 41% |
| Clinch | 2% | 0% | 0% | 0% | 5% |
| Chão | 2% | 2% | 0% | 0% | 55% |

#### Posição -- Oponentes (%)

| Posição | R1 (n=7) | R2 (n=4) | R3 (n=1) | R4 (n=1) | R5 (n=1) |
|---------|----------|----------|----------|----------|----------|
| Distância | 91% | 99% | 100% | 100% | 93% |
| Clinch | 6% | 1% | 0% | 0% | 7% |
| Chão | 4% | 0% | 0% | 0% | 0% |

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Res. | Método | Round | Tempo | Sig./min | Prec. | KD | Saldo sig./min | Sig. oponente/min | Controle (%) | Controle oponente (%) |
|------|----------|------|--------|-------|-------|----------|-------|----|----------------|-------------------|----------|-------------------|
| 10/02/2024 | Trevin Giles | V | KO/TKO | 2 | 4:03 | 4.1 | 51% | 1 | -3.4 | 7.6 | 0% | 0% |
| 08/06/2024 | Charles Radtke | V | KO/TKO | 1 | 4:47 | 3.1 | 42% | 1 | +0.2 | 2.9 | 1% | 7% |
| 17/08/2024 | Li Jingliang | V | KO/TKO | 2 | 4:02 | 6.1 | 65% | 3 | +1.6 | 4.5 | 1% | 0% |
| 09/11/2024 | Neil Magny | V | KO/TKO | 1 | 4:50 | 2.5 | 57% | 2 | +0.4 | 2.1 | 24% | 7% |
| 26/04/2025 | Ian Machado Garry | D | Decisão | 5 | 5:00 | 2.5 | 49% | 0 | -2.5 | 5.0 | 7% | 30% |
| 16/08/2025 | Geoff Neal | V | KO/TKO | 1 | 4:59 | 6.4 | 53% | 1 | +1.4 | 5.0 | 0% | 5% |
| 15/11/2025 | Leon Edwards | V | KO/TKO | 2 | 1:28 | 3.3 | 66% | 1 | +1.4 | 1.9 | 0% | 30% |

### Análise Técnica

- Saldo de striking negativo em todos os 5 rounds na média, mas volume próprio sobe do R1 para o R2 com precisão acompanhando -- aceleração seletiva no segundo round, não descontrolada.
- Knockdowns exclusivamente nos rounds 1 e 2 (média 0.7 e 1.0), zero nos rounds tardios. Saldo de controle piora progressivamente. Capacidade de finalização concentrada no início da luta.
- Defesa de queda cai de 87% (R1) para 33% (R3, n=1 vs Garry), com controle do oponente triplicando. Vulnerabilidade ao grappling cresce com a duração da luta.
- Saldo de striking melhora a cada transição de round (+0.7, +1.2, +1.0, +1.0), mesmo com saldo absoluto negativo -- há adaptação tática intra-luta.
- Contra Giles: saldo sig. de -3.4/min (pior da carreira), mas KO no R2. O saldo de volume não capta golpes de potência decisivos.

### Brechas e Insights

**1.** Distribuição de cabeça sobe de 42% (R1) para 77% (R5), com precisão caindo a 36% no R4 antes de voltar a 58% no R5. A recuperação coincide com mudança de posição (distância 41%, chão 55% no R5).

**2.** Controle próprio irrelevante nos R1-R4 (0-6%), mas salta para 20% no R5 com 55% dos golpes do chão. Transição tática de striker puro para ground-and-pound em rounds tardios.

**3.** 9 knockdowns em 6 vitórias (média 1.5/luta). Única derrota: 0 KD em 5 rounds. Ausência de knockdowns como principal preditor de resultado adverso, acima de volume ou saldo.

**4.** Tentativas de queda dos oponentes sobem de 2.0/5min (R1) para 7.0/5min (R4), com defesa caindo de 87% para 71%. Pressão de wrestling escala com o tempo e a resposta defensiva não acompanha.

---

<a name="capitulo-8-analise-round-a-round--jack-della-maddalena"></a>
## Capítulo 8: Análise Round a Round — Jack Della Maddalena

> O comportamento do Jack muda de round para round — e entender essa dinâmica é decisivo para a estratégia. Volume, precisão, grappling e onde ele é mais perigoso conforme a luta avança.

### Perfil Geral
- Total de lutas analisadas: 9
- Categoria: Peso Meio-Médio
- Resultado geral: 8V-1D
- Vitórias por método: 3 Decisão, 4 KO/TKO, 1 Finalização
- Derrotas por método: 1 Decisão
- Lutas com dados de rounds 4-5: 2 (Belal Muhammad, Islam Makhachev)

### Dados Frios — Médias por Round

#### Striking

| Métrica | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|---------|----------|----------|----------|----------|----------|
| Golpes sig. conectados/min | 6.5 | 4.6 | 6.1 | 3.4 | 5.4 |
| Tentativas sig./min | 12.8 | 8.8 | 11.0 | 7.0 | 8.9 |
| Precisão sig. (%) | 48% | 52% | 56% | 33% | 40% |
| Knockdowns/5min | 1.0 | 0.0 | 0.3 | 0.0 | 0.0 |
| Golpes sig. oponente/min | 4.0 | 4.2 | 3.5 | 3.8 | 2.7 |
| Precisão sig. oponente (%) | 34% | 40% | 30% | 53% | 22% |

**R4 (n=2) — alerta de amostra pequena:** Makhachev (0.2 sig/min, 9% precisão) puxa a média para baixo; Muhammad (6.6 sig/min, 56% precisão) está no extremo oposto. A média de 3.4/min não representa nenhuma das duas lutas individualmente.

**R5 (n=2) — alerta de amostra pequena:** Makhachev (0.2 sig/min) vs Muhammad (10.6 sig/min). Média de 5.4/min é artefato.

#### Grappling

| Métrica | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|---------|----------|----------|----------|----------|----------|
| Takedowns/5min | 0.0 | 0.0 | 0.2 | 0.0 | 0.0 |
| Tentativas TD/5min | 0.2 | 0.2 | 0.4 | 0.0 | 1.0 |
| Precisão TD (%) | 0% | 0% | 50% | -- | 0% |
| Submissões/5min | 0.3 | 0.0 | 0.0 | 0.0 | 0.0 |
| Controle (%) | 3% | 0% | 6% | 5% | 2% |
| TD oponente/5min | 1.0 | 0.4 | 0.7 | 1.0 | 1.5 |
| Precisão TD oponente (%) | 52% | 25% | 44% | 67% | 100% |
| Controle oponente (%) | 22% | 32% | 31% | 47% | 63% |
| Defesa de TD (%) | 48% | 75% | 56% | 33% | 0% |

#### Saldos e Dominância

| Métrica | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|---------|----------|----------|----------|----------|----------|
| Saldo sig./min | +2.5 | +0.4 | +2.6 | -0.4 | +2.7 |
| Saldo TD/5min | -1.0 | -0.4 | -0.5 | -1.0 | -1.5 |
| Saldo controle (pp) | -18pp | -32pp | -24pp | -43pp | -61pp |
| Dominância striking (%) | 61% | 52% | 65% | 32% | 83% |
| Dominância TD (%) | 0% | 0% | 33% | 0% | 0% |
| Dominância controle (%) | 35% | 1% | 19% | 13% | 4% |

### Dados Frios — Variações Médias Round a Round

#### Striking

| Métrica | R1→R2 (n=5) | R2→R3 (n=5) | R3→R4 (n=2) | R4→R5 (n=2) |
|---------|-------------|-------------|-------------|-------------|
| Variação sig. conectados/min | +0.4 | +1.5 | -0.9 | +2.0 |
| Variação sig. conectados (%) | +18% | +68% | -46% | +30% |
| Variação tentativas sig./min | +0.4 | +2.1 | -2.6 | +1.9 |
| Variação precisão sig. (pp) | +7pp | +4pp | -12pp | +8pp |
| Variação knockdowns/5min | 0.0 | +0.3 | 0.0 | 0.0 |

#### Grappling e Controle

| Métrica | R1→R2 (n=5) | R2→R3 (n=5) | R3→R4 (n=2) | R4→R5 (n=2) |
|---------|-------------|-------------|-------------|-------------|
| Variação TD/5min | 0.0 | +0.2 | 0.0 | 0.0 |
| Variação tentativas TD/5min | -0.2 | +0.2 | -0.5 | +1.0 |
| Variação controle (pp) | +0pp | +6pp | +4pp | -3pp |

#### Saldos

| Métrica | R1→R2 (n=5) | R2→R3 (n=5) | R3→R4 (n=2) | R4→R5 (n=2) |
|---------|-------------|-------------|-------------|-------------|
| Variação saldo sig./min | -0.1 | +2.2 | -0.4 | +3.1 |
| Variação saldo TD/5min | +1.0 | -0.1 | -0.5 | -0.5 |
| Variação saldo controle (pp) | +2pp | +8pp | -9pp | -18pp |

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos — Della Maddalena (%)

| Alvo | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|------|----------|----------|----------|----------|----------|
| Cabeça | 66% | 57% | 64% | 41% | 84% |
| Corpo | 24% | 33% | 27% | 6% | 15% |
| Perna | 10% | 10% | 9% | 53% | 1% |

#### Alvos — Oponente (%)

| Alvo | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|------|----------|----------|----------|----------|----------|
| Cabeça | 53% | 77% | 67% | 70% | 96% |
| Corpo | 19% | 11% | 21% | 16% | 4% |
| Perna | 29% | 13% | 13% | 14% | 0% |

#### Posição — Della Maddalena (%)

| Posição | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|---------|----------|----------|----------|----------|----------|
| Distância | 81% | 97% | 72% | 98% | 92% |
| Clinch | 9% | 3% | 16% | 2% | 8% |
| Chão | 10% | 0% | 12% | 0% | 0% |

#### Posição — Oponente (%)

| Posição | R1 (n=9) | R2 (n=5) | R3 (n=5) | R4 (n=2) | R5 (n=2) |
|---------|----------|----------|----------|----------|----------|
| Distância | 91% | 81% | 84% | 90% | 93% |
| Clinch | 8% | 8% | 11% | 8% | 4% |
| Chão | 1% | 11% | 5% | 2% | 4% |

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Res. | Método | Rds | Sig/min | Tent. sig/min | Precisão | KD/min | Saldo sig/min | Def. sig (%) | Def. TD (%) | Ctrl (%) | Cab (%) | Corpo (%) | Dist (%) |
|------|----------|------|--------|-----|---------|---------------|----------|--------|---------------|--------------|-------------|----------|---------|-----------|----------|
| 22/01/2022 | Pete Rodriguez | V | KO/TKO | 1 | 14.4 | 27.2 | 53% | 0.3 | +6.0 | 64% | -- | 1% | 88% | 12% | 93% |
| 11/06/2022 | Ramazan Emeev | V | KO/TKO | 1 | 7.1 | 14.2 | 50% | 0.4 | +4.3 | 71% | 50% | 2% | 61% | 39% | 61% |
| 19/11/2022 | Danny Roberts | V | KO/TKO | 1 | 9.7 | 17.7 | 55% | 0.6 | +8.2 | 85% | 100% | 17% | 70% | 27% | 82% |
| 11/02/2023 | Randy Brown | V | Finalização | 1 | 6.3 | 14.0 | 45% | 0.5 | +1.4 | 72% | -- | 11% | 64% | 7% | 36% |
| 15/07/2023 | Bassil Hafez | V | Decisão | 3 | 5.5 | 9.1 | 61% | 0.0 | +3.4 | 74% | 85% | 9% | 66% | 33% | 82% |
| 16/09/2023 | Kevin Holland | V | Decisão | 3 | 7.0 | 12.7 | 55% | 0.0 | -1.5 | 64% | 100% | 0% | 44% | 34% | 90% |
| 09/03/2024 | Gilbert Burns | V | KO/TKO | 3 | 4.9 | 9.0 | 54% | 0.1 | +2.9 | 53% | 36% | 2% | 81% | 13% | 70% |
| 10/05/2025 | Belal Muhammad | V | Decisão | 5 | 7.1 | 13.7 | 52% | 0.0 | +1.8 | 58% | 67% | 3% | 63% | 26% | 94% |
| 15/11/2025 | Islam Makhachev | D | Decisão | 5 | 0.7 | 2.4 | 30% | 0.0 | -0.5 | 47% | 0% | 0% | 56% | 33% | 78% |

### Análise Técnica

- Volume cai do R1 para o R2 mas precisão sobe -- transição de explosão inicial para seletividade, não fadiga.
- Saldo de striking positivo nos rounds 1-3 (+2.5 a +2.6/min), mas dominância de controle na direção oposta, com oponentes acumulando tempo crescente. Vantagem no striking coexiste com vulnerabilidade posicional.
- Defesa de takedown deteriora de 75% (R2) a 0% (R5), enquanto volume ofensivo de TD do oponente sobe. Resistência à queda degrada mais rápido que o cardio de striking.
- Nas 4 finalizações antecipadas (Rodriguez, Emeev, Roberts, Brown), saldo sig/min médio no R1 foi +5.0 vs +1.0 nas lutas que foram à distância. Desfecho rápido depende de abrir vantagem de striking no início.
- Precisão do oponente cai no R3 (30%) enquanto a dele sobe ao pico (56%). Pressão cumulativa degrada a eficiência adversária.

### Brechas e Insights

**1.** Saldo sig/min positivo em R1-R3, mas saldo de controle sempre negativo. Ganha em pé, perde a guerra posicional. Se o oponente converter controle em dano, a equação muda.

**2.** Volume cai 29% do R1 para R2 (12.8 para 8.8 tentativas/min), mas precisão sobe 4pp. Proporção acerto/tentativa melhora -- economia de energia calculada.

**3.** No R3: clinch sobe de 3% (R2) para 16%, chão de 0% para 12%, e é o round com maior saldo de striking (+2.6/min). Agressividade posicional tardia ligada a pressionar adversários já desgastados.

**4.** Oponentes concentram golpes na cabeça de forma crescente (53% R1 a 96% R5), mas sem ganho de precisão (22% no R5). Abandonam corpo em rounds tardios sem retorno proporcional.

**5.** Contra Holland: saldo de -1.5/min (único negativo entre vitórias) com controle adversário 0%. Pressão de volume à distância, sem grappling, é o cenário mais difícil entre oponentes que ficam em pé.

---

<a name="capitulo-9-cruzamento-de-dados"></a>
## Capítulo 9: Cruzamento de Dados

> Números lado a lado, sem interpretação — a matéria-prima de tudo que veio nos capítulos anteriores.

### Ficha Técnica

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
|------|:-------------:|:--------------------:|:--------:|
| Categoria | Peso Meio-Médio | Peso Meio-Médio | - |
| Postura | Ambidestro | Ambidestro | - |
| Ranking Categoria | 5 | 1 | - |
| Ranking Libra por Libra | Desranqueado | 14 | - |
| Idade (anos) | 32 🔴 | 29 🟢 | **Jack Della Maddalena** |
| Altura (cm) | 185 🟢 | 180 🔴 | **Carlos Prates** |
| Envergadura (cm) | 198 🟢 | 185 🔴 | **Carlos Prates** |
| Alcance Extra (cm) | 13 🟢 | 5 🔴 | **Carlos Prates** |

---

### Carreira Geral

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
|------|:-------------:|:--------------------:|:--------:|
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
| Derrotas por KO/TKO | 2 🟢 | 1 🟢 | - |
| Derrotas por Finalização | 3 🔴 | 1 🟢 | **Jack Della Maddalena** |
| Derrotas por Decisão | 2 | 1 🟢 | **Jack Della Maddalena** |
| % de Derrotas Via Rápida | 71% 🔴 | 67% 🟢 | **Jack Della Maddalena** |
| Dist. Vitórias: % KO/TKO | 78% | 67% | - |
| Dist. Vitórias: % Finalização | 13% | 11% | - |
| Dist. Vitórias: % Decisão | 9% | 22% | - |
| Dist. Derrotas: % KO/TKO | 29% | 33% | - |
| Dist. Derrotas: % Finalização | 43% | 33% | - |
| Dist. Derrotas: % Decisão | 29% | 33% | - |
| Tempo Médio de Luta | 08:48 | 11:59 | - |
| Intervalo Médio Entre Lutas (dias) | 107.33 | 174.13 | - |

---

### Carreira no UFC

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
|------|:-------------:|:--------------------:|:--------:|
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
| Dist. Vitórias UFC: % KO/TKO | 100% | 44% | - |
| Dist. Vitórias UFC: % Finalização | 0% | 11% | - |
| Dist. Vitórias UFC: % Decisão | 0% | 44% | - |
| Dist. Derrotas UFC: % KO/TKO | 0% | 0% | - |
| Dist. Derrotas UFC: % Finalização | 0% | 0% | - |
| Dist. Derrotas UFC: % Decisão | 100% | 100% | - |

---

### Striking

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
|------|:-------------:|:--------------------:|:--------:|
| Golpes Sig. Conectados/min | 3.77 🔴 | 5.57 🟢 | **Jack Della Maddalena** |
| Golpes Sig. Absorvidos/min | 4.53 🔴 | 3.84 🟢 | **Jack Della Maddalena** |
| Precisão de Striking | 55% 🟢 | 51% 🔴 | **Carlos Prates** |
| Defesa de Striking | 47% 🔴 | 63% 🟢 | **Jack Della Maddalena** |
| Saldo de Striking por Minuto | -0.76 🔴 | 1.73 🟢 | **Jack Della Maddalena** |
| Knockdowns Causados por 5min | 0.7 🟢 | 0.3 🔴 | **Carlos Prates** |
| Knockdowns Sofridos por 5min | 0.0 | 0.0 | Empate |
| Golpes na Cabeça por Minuto | 2.02 🔴 | 3.42 🟢 | **Jack Della Maddalena** |
| Golpes no Corpo por Minuto | 0.82 🔴 | 1.40 🟢 | **Jack Della Maddalena** |
| Golpes nas Pernas por Minuto | 0.92 🟢 | 0.51 🔴 | **Carlos Prates** |
| Golpes em Pé por Minuto | 3.52 🔴 | 4.51 🟢 | **Jack Della Maddalena** |
| Golpes no Clinche por Minuto | 0.03 🔴 | 0.49 🟢 | **Jack Della Maddalena** |
| Golpes no Solo por Minuto | 0.21 🔴 | 0.33 🟢 | **Jack Della Maddalena** |
| Golpes p/ Nocautear (média) | 38 🟢 | 167 🔴 | **Carlos Prates** |
| Dist. Alvo: % Cabeça | 54% | 64% | - |
| Dist. Alvo: % Corpo | 22% | 26% | - |
| Dist. Alvo: % Pernas | 25% | 9% | - |
| Dist. Posição: % Em Pé | 94% | 85% | - |
| Dist. Posição: % Clinche | 1% | 9% | - |
| Dist. Posição: % Solo | 6% | 6% | - |

---

### Grappling

| Dado | Carlos Prates | Jack Della Maddalena | Vantagem |
|------|:-------------:|:--------------------:|:--------:|
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
|------|:-------------:|:--------------------:|:--------:|
| Resiliência a Nocaute | 81% 🔴 | 85% 🟢 | **Jack Della Maddalena** |
| Taxa de Vitória no 1º Round | 43% 🔴 | 44% 🟢 | **Jack Della Maddalena** |
| Taxa de Vitória Geral | 77% 🔴 | 86% 🟢 | **Jack Della Maddalena** |
| Golpes p/ Ser Nocauteado (média) | sem dado | sem dado | - |
| % Luta Combatida (médio) | 50% 🔴 | 63% 🟢 | **Jack Della Maddalena** |
| DNA de Estilo Equilibrado | 0.1 | sem dado | - |
| Perfil de Distância de Luta | 0.86 | sem dado | - |

> **Legenda:** 🟢 Vantagem | 🔴 Desvantagem | Empate = valores idênticos | - = sem dado ou sem vantagem direta
