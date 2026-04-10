# Relatório Final — Karine Silva vs Jasmine Jasudavicius

> **Autor:** Diogo Zequini — Cientista de Dados
>
> Este relatório analisa 7 lutas de Karine Silva e 11 lutas de Jasmine Jasudavicius no UFC
> (2022–2025), com base em dados de UFC Stats, UFC.com e Tapology,
> processados com Python e algoritmos de Machine Learning para ajuste por qualidade
> de oponente.

---

## Sumário

1. [Caminhos Que os Números Abrem — Karine Silva](#capitulo-1-caminhos-que-os-numeros-abrem--karine-silva)
2. [Caminhos Que os Números Abrem — Jasmine Jasudavicius](#capitulo-2-caminhos-que-os-numeros-abrem--jasmine-jasudavicius)
3. [Insights Ocultos — Karine Silva](#capitulo-3-insights-ocultos--karine-silva)
   - [Insights Positivos](#insights-positivos)
   - [Insights Negativos](#insights-negativos)
4. [Insights Ocultos — Jasmine Jasudavicius](#capitulo-4-insights-ocultos--jasmine-jasudavicius)
   - [Insights Positivos](#insights-positivos-1)
   - [Insights Negativos](#insights-negativos-1)
5. [Análise Subjetiva Luta a Luta — Karine Silva](#capitulo-5-analise-subjetiva-luta-a-luta--karine-silva)
6. [Análise Subjetiva Luta a Luta — Jasmine Jasudavicius](#capitulo-6-analise-subjetiva-luta-a-luta--jasmine-jasudavicius)
7. [Análise Round a Round — Karine Silva](#capitulo-7-analise-round-a-round--karine-silva)
8. [Análise Round a Round — Jasmine Jasudavicius](#capitulo-8-analise-round-a-round--jasmine-jasudavicius)
9. [Perfil vs Média — Karine Silva](#capitulo-9-perfil-vs-media--karine-silva)
10. [Perfil vs Média — Jasmine Jasudavicius](#capitulo-10-perfil-vs-media--jasmine-jasudavicius)
11. [Cruzamento de Dados Frios](#capitulo-11-cruzamento-de-dados-frios)

---

## Capítulo 1: Melhores Ações para a Karine

> Os capítulos 1 e 2 não fecham estratégia de camp. Eles mostram quais caminhos os números deixam mais abertos para cada lado. Os Capítulos 3 e 4 explicam de qual luta saiu cada leitura.

Em ordem de importância:

1. **Chutes nas pernas aparecem como a porta de entrada mais limpa para a Karine.** Ela entrega 0.84 golpes de perna por minuto, contra 0.29/min da Jasmine, e a defesa de striking da Jasmine fica em 51%. O dado não manda chutar a qualquer custo. Ele mostra que esse ataque aparece como uma forma plausível de puxar reação, encurtar a distância e abrir o clinch.

2. **O R1 é a faixa em que o jogo de resolução da Karine mais aparece.** As 3 vitórias por finalização dela no UFC vieram no R1. A precisão de quedas cai de 83% no R1 para 39% no R3, e o único round com saldo positivo em pé é o primeiro (+0.3/min). Do outro lado, o R1 ainda é o round mais vulnerável da Jasmine em pé (-1.0/min), antes do controle crescer no R2. O dado não diz que a luta precisa acabar ali; diz que é ali que a vantagem estatística da Karine mais aparece.

3. **Clinch foi o contexto em que a queda da Karine melhor funcionou.** Contra Moroz, a única luta em que o clinch virou o eixo do ataque, Karine fechou 57% de precisão e finalizou em 4:59 do R1. Contra Viviane, quando precisou entrar mais de fora, foi 1 em 7 nas quedas e perdeu a luta. O dado não garante repetição automática, mas mostra com clareza onde a entrada dela saiu mais limpa.

4. **Tentativa de queda sem preparação em pé carrega custo alto contra esse perfil de defesa.** Nas vitórias por finalização, Karine bateu pouco, entrou bem e fechou rápido. Contra Viviane, tentou 7 quedas, teve saldo positivo em pé (+0.67/min) e ainda assim perdeu porque a luta foi decidida no grappling. Com a Jasmine defendendo 76% das quedas, esse é um caminho que existe, mas com risco alto se a entrada vier limpa demais para ela ler.

5. **Distribuição entre corpo e pernas aparece como um caminho mais estável do que foco na cabeça.** Jasmine coloca 70% do próprio ataque na cabeça, o que tende a puxar a atenção defensiva para essa zona. Nas melhores lutas da Karine, a distribuição foi mais equilibrada: Ariane com 30% cabeça, 33% corpo e 37% pernas; Moroz com chutes ajudando a entrar no clinch. O dado não fecha questão, mas sugere que a luta dela costuma ficar mais jogável quando os alvos se espalham.

6. **Depois do R1, os números abrem mais um caminho de gestão do que de aceleração.** No R2, Karine atinge 61% de precisão em pé, mas o saldo ainda fica negativo (-0.5/min) e o volume cai bastante. Quando a luta acelera sem controle, o R3 vira mais tentativa, menos precisão e saldo de -1.2/min. O dado não manda desacelerar sempre; ele mostra que a urgência tardia tem cobrado caro.

7. **No longo da luta, o histórico favorece mais o jogo de placar da Jasmine do que o da Karine.** Karine tem 2 vitórias por decisão em 7 lutas no UFC. Jasmine tem 5 vitórias por decisão em 8 vitórias no UFC. Uma aparece melhor quando a luta precisa ser resolvida cedo; a outra tem histórico mais forte quando vira disputa de round. Esse é menos um plano e mais o pano de fundo do confronto.

---

## Capítulo 2: O que provavelmente a equipe da Jasmine planejou

1. **Empurrar a luta além do R1 aparece como o dado mais favorável para a Jasmine.** O melhor jogo da Karine aparece quando ela derruba cedo e fecha a finalização logo depois. Jasmine defende 76% das quedas. Se essa primeira entrada não entra, a luta vai para os rounds em que o volume da Karine cai e o dela cresce. A luta da Viviane é a referência mais próxima: segurou a primeira onda, travou a queda e mudou o rumo da luta.

2. **Acúmulo de round aparece como caminho mais disponível do que dano de interrupção.** Jasmine não venceu por KO/TKO no UFC. O saldo em pé melhora do R1 para o R2 (-1.0/min para +0.3/min) e fecha neutro no R3. Karine faz o caminho contrário. Cada round sem finalização empurra a luta para um terreno em que a Jasmine costuma sobreviver melhor.

3. **Os números sugerem um possível trade-off: ceder parte do chute baixo para negar o clinch.** Karine usa 0.84 golpes de perna por minuto e costuma transformar esse ataque em entrada. O pior cenário para a Jasmine não parece ser tomar o chute isolado. Parece ser deixar esse chute virar clinch e depois queda. Não é recomendação fechada; é o custo relativo que os dados deixam entrever.

4. **O R3 é a faixa em que o jogo da Jasmine continua funcional e o da Karine perde força.** No terceiro round, a precisão de quedas da Karine cai para 39%, o saldo em pé vai para -1.2/min e o golpe de solo desaparece. A Jasmine ainda mantém 43% de controle e chega ao pico de volume em pé. Se a luta atravessa os dois primeiros rounds sem quebra, a tendência muda mais para o lado dela.

5. **Defesa de queda é o caminho mais claro para a Jasmine empurrar a luta para o placar.** Karine defende 14% das quedas no recorte UFC. Contra Viviane, a luta foi andando para esse lado: tentativa travada, posição ruim, desgaste aparecendo e round escorrendo. Com 76% de defesa, esse é o caminho estatístico mais nítido do lado da Jasmine, mesmo sem garantir que seja o único.

---

## Capítulo 3: Insights Ocultos — Karine Silva

> Os dois capítulos anteriores definem os planos. A partir daqui, mostramos de onde vem cada conclusão: qual luta, o que era esperado, o que aconteceu e por quê. Recorte: 7 lutas UFC (5V–2D).

### Onde Ela É Extrema na Categoria (Peso Mosca Feminino)

| Métrica | Valor | Posição na divisão |
|---------|-------|-------------------|
| Vitórias no 1º round | 3 | Entre as 4% melhores |
| Vitórias por finalização | 9 | Entre as 8% melhores |
| % golpes nas pernas | 33% | Entre as 8% melhores |
| Tentativas de submissão/min | baixo | Entre as 9% mais baixas |

**O que isso revela:**
- Karine tenta pouca submissão por minuto para o padrão da categoria, mas converte quando a janela aparece. Nas 3 vitórias por finalização no UFC, tentou 1 vez em cada luta e fechou as 3.
- Os chutes nas pernas aparecem junto desse padrão. Não é volume por volume. É ataque para abrir caminho.

---

---

### Insights Positivos

1. **vs Moroz: o clinch virou o centro da luta e saiu a melhor atuação do recorte.** Contra Moroz, o clinch saltou de 13% para 37% dos golpes. Vieram 6.02 golpes significativos por minuto, 57% de precisão e a finalização em 4:59 do R1. A melhor versão da Karine passou por esse caminho.

2. **vs Ariane e Dione: o corpo apareceu nas decisões ganhas, não nas perdidas.** Nas decisões ganhas, 34% dos golpes da Karine foram ao corpo. Nas derrotas, 18%. Quando ela distribui melhor os alvos, a luta costuma ficar mais controlável para ela.

3. **vs Dione: ganhou a decisão mais improvável do recorte sem dominar a luta no volume bruto.** Dione controlou mais tempo, quedou melhor e conectou mais golpes. Mesmo assim perdeu. A Karine conseguiu fazer mais peso nos momentos que contam do que o total da luta faz parecer.

---

### Insights Negativos

1. **vs Viviane: a derrota saiu inteira da defesa de queda.** Karine terminou com saldo positivo em pé (+0.67/min), mas teve 0% de defesa de queda contra 62% esperado. A luta virou porque ela não conseguiu travar a entrada que mais mudava o placar.

2. **Lutas longas: a janela de finalização fechou no R1 e o ground-and-pound caiu junto.** Nas 3 vitórias por finalização, foram 3 tentativas de sub e 3 conversões, todas no R1. Nas lutas que chegaram ao R3, essa via praticamente sumiu e o volume no chão caiu junto. Até aqui, o jogo dela ainda não mostrou a mesma força em 15 minutos.

3. **vs Maycee: quando o R1 não resolve, o controle pode virar rápido.** Contra Barber, o plano funcionou no começo, mas depois o controle mudou de lado e o saldo de striking caiu para -2.27/min, o pior do recorte. Quando a luta escapa do primeiro round, a Karine ainda não mostrou uma rota estável de recuperação.

---

## Capítulo 4: Insights Ocultos — Jasmine Jasudavicius

> Mesma lógica do capítulo anterior, agora pelo lado da Jasmine. Recorte: 11 lutas UFC (8V–3D).

### Onde Ela É Extrema na Categoria (Peso Mosca Feminino)

| Métrica | Valor | Percentil | N da Categoria | Posição |
|---------|-------|-----------|----------------|---------|
| Volume total de golpes/min | 8.66/min | 99% | 203 | Top 1% |
| % golpes no chão (estilo) | 19% | 99% | 203 | Top 1% |
| % golpes na cabeça (estilo) | 70% | 99% | 203 | Top 1% |
| % golpes no corpo (estilo) | 22% | 0.2% | 203 | Bottom 0.2% |

Três extremos aparecem juntos: muito volume, bastante ação no chão e ataque concentrado na cabeça. O desenho é simples de ler: derrubar, controlar e pontuar por cima.

---

### Insights Positivos

1. **vs Gabriella: ganhou uma luta em que os golpes significativos sozinhos não contam a história.** Foram 149 golpes totais, 24 significativos e 691 segundos de controle. O dado mostra isso com clareza: a Jasmine consegue ganhar lutas em que a sensação de domínio pesa mais do que o número puro de golpes limpos.

2. **Quando a queda entra, o resto cresce junto.** Nas vitórias, Jasmine converte 62% das quedas. Nas derrotas em que tentou, 10%. Quando o grappling funciona, o controle sobe e o striking fica mais confortável de executar.

---

### Insights Negativos

1. **vs Fiorot: a única luta de 11 com zero tentativas de queda.** Em todas as outras 10, Jasmine tentou pelo menos uma queda. Contra Fiorot: nenhuma, 0 segundos de controle e luta encerrada em 1:14 com saldo de -11.35/min. Não foi o plano dela funcionando mal. Foi o plano nem chegando a começar.

2. **Nas derrotas por decisão, a luta desmonta quando a queda não converte.** Contra Natalia e Tracy, a razão entre golpes totais e significativos caiu para 1.3x e 1.2x, o grappling travou e o saldo de striking ficou negativo. Quando ela não chega ao chão, o resto do jogo perde sustentação.

---

## Capítulo 5: Análise Subjetiva Luta a Luta — Karine Silva

> Recorte luta a luta. Os números que embasam os insights dos Capítulos 3 e 4.

### Médias de Carreira

| Métrica | Média dela |
|---------|:---------:|
| Golpes Sig. Conectados/min | 2.56 |
| Golpes Sig. Absorvidos/min | 2.94 |
| Precisão Striking | 42% |
| Defesa Striking | 49% |
| Quedas Aplicadas/15min | 2.65 |
| Precisão de Quedas | 60% |
| Defesa de Quedas | 14% |
| Tentativas de Finalização/15min | 2.00 |
| Distribuição de Golpes — Cabeça / Corpo / Pernas | 40% / 24% / 36% |

> Esses são os números normais dela. Nos bullets de cada luta, mostramos onde ela saiu desse padrão.

---

### Resumo do Recorte

- Lutas analisadas: 6 (4 vitórias + 2 derrotas)
- Período: 03/06/2023 a 06/12/2025
- Dados detalhados (lutadora + oponente) disponíveis em 6 de 6 lutas

---

### Vitórias Recentes

#### 1. vs Dione Barbosa — UFC 319: Du Plessis vs. Chimaev (16/08/2025)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Karine Silva | Dione Barbosa |
|---------|:-----------:|:-------------:|
| Sig Strikes Conectados | 26 | 31 |
| Sig Strikes Tentados | 70 | 87 |
| Precisão (%) | 37% | 36% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/3 | 3/4 |
| Tentativas de Sub | 2 | 1 |
| Controle (tempo) | 2:23 | 5:18 |
| Controle (%) | 16% | 35% |

##### Pontos Positivos

- Defesa de striking em 64% — a média dela é 49%, 15 pontos acima do normal. Dione tentou 87 golpes e conectou 31; Karine segurou bem as trocas em pé apesar do volume menor.
- Precisão de 37% com volume abaixo do normal pode parecer fraca, mas corpo e pernas somaram 58% dos acertos (9 no corpo, 6 nas pernas). A Karine não foi atrás da cabeça o tempo todo — distribuiu, e isso custou caro pra Dione nos rounds finais.

##### Pontos Negativos

- Dione ficou com 5:18 de controle vs 2:23 de Karine. No grappling, foi 3/4 (75%) de queda vs 1/3 (33%) de Karine — Dione dominou completamente essa dimensão e Karine sobreviveu no standup.
- 1.73 sig/min — a média dela é 2.56/min, 32% abaixo. Saldo de striking negativo (-0.33/min). Karine venceu uma decisão onde tomou mais golpes e ficou menos tempo em cima. Um dos resultados mais frágeis das vitórias analisadas.

---

#### 2. vs Ariane da Silva — UFC Fight Night: Nicolau vs. Perez (27/04/2024)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Karine Silva | Ariane da Silva |
|---------|:-----------:|:---------------:|
| Sig Strikes Conectados | 27 | 42 |
| Sig Strikes Tentados | 75 | 81 |
| Precisão (%) | 36% | 52% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 5/6 | 0/0 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 7:32 | 2:06 |
| Controle (%) | 50% | 14% |

##### Pontos Positivos

- 5/6 quedas com 83% de precisão — a média dela é 60%. Maior eficiência de derrubadas do recorte. O grappling foi o que ganhou essa luta: 7:32 de controle (50% do tempo total) contra uma Ariane que não tentou uma queda sequer.
- Karine distribuiu os golpes entre cabeça (30%), corpo (33%) e pernas (37%) — distribuição equilibrada e fora do padrão dela (normalmente cabeça-heavy com 40%). Pode ser estratégia para desgastar Ariane antes das quedas, ou adaptação espontânea ao perfil da oponente.

##### Pontos Negativos

- Ariane conectou 42 sig strikes vs 27 de Karine, com 52% de precisão vs 36%. No striking puro, a Karine perdeu: saldo de -1.0/min. Ela ganhou a luta pelo grappling, não pela troca em pé.
- Volume em 1.80/min — a média dela é 2.56/min, 30% abaixo. A Karine não foi lutar pra trocar; foi pra derrubar. Quando fica nesse modo de buscar queda sem volume no standup, fica vulnerável às combinações do oponente.

---

#### 3. vs Maryna Moroz — UFC 292: Sterling vs. O'Malley (19/08/2023)
**Finalização | R1 4:59 | Peso Mosca**

##### Dados Objetivos

| Métrica | Karine Silva | Maryna Moroz |
|---------|:-----------:|:------------:|
| Sig Strikes Conectados | 30 | 16 |
| Sig Strikes Tentados | 53 | 55 |
| Precisão (%) | 57% | 29% |
| Knockdowns | 1 | 0 |
| Quedas Aplicadas | 1/1 | 0/0 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 0:51 | 1:41 |
| Controle (%) | 17% | 34% |

##### Pontos Positivos

- 6.02 sig/min — a média dela é 2.56/min, 2.35x acima do normal. Foi o pico de volume ofensivo de todo o recorte, e com 57% de precisão (15 pontos acima da média). Volume alto com precisão alta ao mesmo tempo é raro — aqui as duas coisas apareceram juntas.
- Defesa de striking em 71% — a média dela é 49%, 22 pontos acima. Moroz tentou 55 golpes e conectou só 16. Karine atacou mais, absorveu menos — o cenário oposto do padrão dela, onde o saldo costuma ser negativo.

##### Pontos Negativos

- Controle de 0:51 (17%) contra 1:41 (34%) de Moroz — a Karine ficou menos tempo em posição dominante no chão, mesmo sendo quem finalizou. O 1 KD + 1 queda foi suficiente pra acabar, mas o controle do ground não estava no bolso dela.
- Amostra de R1 com 4:59 — a luta acabou em 1 round. Os números são bons, mas com um round só não dá pra consolidar padrão. Coloquei porque os dados internos do round são consistentes, mas é basicamente uma foto única.

---

#### 4. vs Ketlen Souza — UFC Fight Night: Kara-France vs. Albazi (03/06/2023)
**Finalização | R1 1:45 | Peso Mosca**

##### Dados Objetivos

| Métrica | Karine Silva | Ketlen Souza |
|---------|:-----------:|:------------:|
| Sig Strikes Conectados | 3 | 0 |
| Sig Strikes Tentados | 10 | 0 |
| Precisão (%) | 30% | -- |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/1 | 0/0 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 1:21 | 0:00 |
| Controle (%) | 77% | 0% |

##### Pontos Positivos

- 77% de controle em 1:45 de luta — Karine entrou, derrubou com 100% de precisão e não saiu de cima. Ketlen não conectou um golpe sequer e não tentou nenhuma queda. Foi domínio total e imediato.
- A finalização saiu com 1 queda, 1 tentativa de sub e 1:21 de controle em menos de 2 minutos. É o padrão de grappling dela funcionando no máximo sem precisar de muito volume de striking.

##### Pontos Negativos

- Luta de 1:45 gera dados muito limitados. Os 3 golpes conectados de 10 tentados (30% de precisão — 12 pontos abaixo da média) são ruído, não padrão. Não dá pra tirar conclusão de striking de uma luta com 10 tentativas totais.
- Ketlen não apresentou resistência alguma — nenhum strike, nenhuma queda tentada. O nível da oponente torna essa luta pouco informativa sobre onde Karine está taticamente. *(dado de 1:45 contra oponente passiva — usar como referência de grappling, não de striking)*

---

### Derrotas Recentes

#### 1. vs Maycee Barber — UFC 323: Dvalishvili vs. Yan 2 (06/12/2025)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Karine Silva | Maycee Barber |
|---------|:-----------:|:-------------:|
| Sig Strikes Conectados | 21 | 55 |
| Sig Strikes Tentados | 45 | 85 |
| Precisão (%) | 47% | 65% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 2/3 | 3/5 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 3:28 | 6:20 |
| Controle (%) | 23% | 42% |

##### Pontos Positivos

- Precisão de striking em 47% — a média dela é 42%, 5 pontos acima. Com volume abaixo do normal (1.40/min vs 2.56/min), ela foi seletiva. O problema não foi falta de acerto — foi volume muito baixo e desvantagem no saldo.
- 2/3 quedas com 67% de precisão. Karine dominou o R1 no grappling (2:49 de controle vs 0:21 de Barber no primeiro round). Havia um plano e funcionou no começo.

##### Pontos Negativos

- Barber conectou 55 vs 21 de Karine. Volume e saldo de -2.27 sig/min — o pior saldo de striking de todo o recorte. A defesa de striking colapsou para 35% (vs média de 49%, 14 pontos abaixo). Barber bateu na cabeça: 41 de 66 tentativas na cabeça (62% de precisão nessa região).
- O padrão por round conta a história: R1 Karine com 2:49 de controle, R2 Barber com 3:57, R3 Barber com 2:02. A Karine abriu bem no grappling e a luta foi escapando dos R2 em diante. Quando Barber acertou o ritmo, o volume de Karine (1.40/min geral) não foi suficiente pra reagir.

---

#### 2. vs Viviane Araujo — UFC 309: Jones vs. Miocic (16/11/2024)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Karine Silva | Viviane Araujo |
|---------|:-----------:|:--------------:|
| Sig Strikes Conectados | 58 | 48 |
| Sig Strikes Tentados | 132 | 85 |
| Precisão (%) | 44% | 56% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/7 | 3/3 |
| Tentativas de Sub | 1 | 1 |
| Controle (tempo) | 3:30 | 2:25 |
| Controle (%) | 23% | 16% |

##### Pontos Negativos

- 1/7 de quedas, 14% de precisão — a média dela é 60%. Seis tentativas desperdiçadas em uma luta de 3 rounds. Toda vez que Karine foi ao clinch pra buscar a queda, Viviane defendeu. O grappling que é a principal arma dela foi completamente neutralizado.
- Viviane foi 3/3 (100%) nas derrubadas. O contraste direto: Karine tentou 7x mais quedas e converteu 1, Viviane tentou 3 e converteu 3. A derrota não foi por falta de volume no striking (58 conectados vs 48 de Viviane, saldo positivo de +0.67/min) — foi porque a dimensão decisiva da luta, o grappling, ficou toda com Viviane.

---

## Capítulo 6: Análise Subjetiva Luta a Luta — Jasmine Jasudavicius

> Mesma lógica do capítulo anterior, agora pelo lado da Jasmine.

### Médias de Carreira

| Métrica | Média dela |
|---------|:---------:|
| Golpes Sig. Conectados/min | 3.47 |
| Golpes Sig. Absorvidos/min | 3.77 |
| Precisão Striking | 45% |
| Defesa Striking | 51% |
| Quedas Aplicadas/15min | 2.74 |
| Precisão de Quedas | 54% |
| Defesa de Quedas | 76% |
| Tentativas de Finalização/15min | 0.47 |
| Distribuição de Golpes — Cabeça / Corpo / Pernas | 74% / 17% / 9% |
| Distribuição por Posição — Em pé / Clinche / Solo | 74% / 7% / 19% |

> Esses são os números normais dela. Nos bullets de cada luta, mostramos onde ela saiu desse padrão.

---

### Resumo do Recorte

- Lutas analisadas: 7 (4 vitórias + 3 derrotas)
- Período: 18/06/2022 a 18/10/2025
- Dados detalhados (lutadora + oponente) disponíveis em 7 de 7 lutas

---

### Vitórias Recentes

#### 1. vs Jessica Andrade — UFC 315: Muhammad vs. Della Maddalena (10/05/2025)
**Finalização | R1 2:40 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Jessica Andrade |
|---------|:-------------------:|:---------------:|
| Sig Strikes Conectados | 11 | 4 |
| Sig Strikes Tentados | 18 | 8 |
| Precisão (%) | 61% | 50% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 1/2 | 0/0 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 1:12 | 0:00 |
| Controle (%) | 45% | 0% |

##### Pontos Positivos

- 61% de precisão em 18 tentativas — a média dela é 45%, 16 pontos acima do normal. Com luta curta (2:40), cada golpe pesou mais. 82% dos acertos na cabeça, contra uma das mais durões do Peso Mosca.
- Andrade não completou nenhuma queda e não ficou nenhum segundo em controle. Jasmine neutralizou completamente o grappling da principal ameaça da oponente, derrubou, e finalizou.

##### Pontos Negativos

- Luta de 2:40 — dados muito limitados. Os números são bons, mas com 18 tentativas e 1 round não dá pra consolidar padrão. Andrade pode ter entrado mal preparada para o grappling de Jasmine, o que infla a leitura da luta. *(dado de 1 round contra adversária que foi a 57kg — usar com cautela)*

---

#### 2. vs Mayra Bueno Silva — UFC Fight Night: Adesanya vs. Imavov (01/02/2025)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Mayra Bueno Silva |
|---------|:-------------------:|:-----------------:|
| Sig Strikes Conectados | 56 | 37 |
| Sig Strikes Tentados | 105 | 72 |
| Precisão (%) | 53% | 51% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 3/5 | 0/0 |
| Tentativas de Sub | 0 | 1 |
| Controle (tempo) | 7:11 | 0:00 |
| Controle (%) | 48% | 0% |

##### Pontos Positivos

- Jasmine venceu os dois mundos: 56 vs 37 no striking (saldo +1.27/min), 53% de precisão vs 51% de Mayra, e ainda dominou completamente no chão — 3/5 quedas, 7:11 de controle vs 0 segundo de Mayra. É difícil de conseguir as duas coisas ao mesmo tempo.
- 53% de precisão com 105 tentativas — 8 pontos acima da média dela. Controle consistente nos 3 rounds: 2:48 no R1, 1:20 no R2, 3:03 no R3. Não teve round ruim no chão.

##### Pontos Negativos

- Distribuição de golpes saiu completamente do padrão: 41% cabeça, 36% corpo, 23% pernas — normalmente Jasmine vai em 74% cabeça. Pode ter sido estratégia contra Mayra (BJJ pesada), pode ter sido adaptação forçada. Não dá pra cravar o motivo, mas o padrão foi o mais diferente do normal em todo o recorte de vitórias.

---

#### 3. vs Ariane da Silva — UFC Fight Night: Moreno vs. Albazi (02/11/2024)
**Finalização | R3 2:28 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Ariane da Silva |
|---------|:-------------------:|:---------------:|
| Sig Strikes Conectados | 36 | 42 |
| Sig Strikes Tentados | 84 | 92 |
| Precisão (%) | 43% | 46% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 3/5 | 0/0 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 5:44 | 0:00 |
| Controle (%) | 46% | 0% |

##### Pontos Positivos

- Ariane conectou mais golpes (42 vs 36) e foi mais precisa (46% vs 43%). Jasmine venceu por finalização no R3 mesmo perdendo no striking — a vitória veio inteiramente do grappling: 3/5 quedas, 5:44 de controle, e paciência pra forçar a finalização no terceiro round.
- O controle foi crescente: R1 apenas 32 segundos, R2 3:42, R3 1:30. Jasmine foi encontrando o ritmo do grappling progressivamente ao longo da luta.

##### Pontos Negativos

- Volume 17% abaixo da média (2.89/min vs 3.47/min) e saldo de striking negativo (-0.48/min). Ariane foi melhor em pé. Jasmine não tem margem pra dar a troca e depender 100% do grappling contra adversárias de alto nível — aqui funcionou, mas o risco é real.
- 81% dos golpes na cabeça, sem variar pra corpo ou pernas — praticamente o padrão normal dela. Contra adversárias com boa defesa de cabeça, essa previsibilidade no alvo pode custar caro.

---

#### 4. vs Fatima Kline — UFC Fight Night: Namajunas vs. Cortez (13/07/2024)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Fatima Kline |
|---------|:-------------------:|:------------:|
| Sig Strikes Conectados | 40 | 39 |
| Sig Strikes Tentados | 89 | 81 |
| Precisão (%) | 45% | 48% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 4/6 | 1/1 |
| Tentativas de Sub | 1 | 0 |
| Controle (tempo) | 7:48 | 0:52 |
| Controle (%) | 52% | 6% |

##### Pontos Positivos

- 7:48 de controle (52% da luta), distribuídos entre os 3 rounds: 2:32, 2:25, 2:51. Não foi um único round dominante — foi pressão constante no chão durante os 15 minutos. 4/6 quedas (67% de precisão, acima da média de 54%).
- Distribuição de golpes menos concentrada na cabeça do que o normal: 63% cabeça, 23% corpo, 15% pernas — contra 74/17/9 da média. Pode ter sido adaptação pra variar o alvo e abrir espaço para as quedas.

##### Pontos Negativos

- No striking foi praticamente um empate: 40 conectados vs 39 de Kline, 45% de precisão vs 48% de Kline. Saldo de +0.07/min — quase zero. Volume 23% abaixo da média (2.67/min vs 3.47/min). Jasmine venceu por controle, não por domínio no standup.
- Kline completou a única queda que tentou (100%) e ficou 52 segundos em controle. O grappling de Jasmine foi superior, mas não incontestavelmente — Kline tinha ferramentas no chão também.

---

### Derrotas Recentes

#### 1. vs Manon Fiorot — UFC Fight Night: De Ridder vs. Allen (18/10/2025)
**KO/TKO | R1 1:14 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Manon Fiorot |
|---------|:-------------------:|:------------:|
| Sig Strikes Conectados | 2 | 16 |
| Sig Strikes Tentados | 14 | 27 |
| Precisão (%) | 14% | 59% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 0/0 | 0/0 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 0:00 | 0:06 |
| Controle (%) | 0% | 8% |

##### Pontos Negativos

- 2/14 no striking, 14% de precisão — a média dela é 45%, 31 pontos abaixo. Em 1:14 de luta, Jasmine tentou 14 golpes e não achou o alvo. Fiorot conectou 16 de 27 (59%) e acabou com a luta. A defesa de striking ficou em 41% (vs média 51%) — Fiorot entrou e saiu sem resposta real.
- Saldo de -11.35 sig/min — o pior número de todo o recorte por larga margem. A luta foi tão curta que praticamente não houve tempo de reagir. Jasmine não chegou a tentar uma queda sequer, que é onde ela vive. Fiorot não deixou.

---

#### 2. vs Tracy Cortez — UFC Fight Night: Grasso vs. Shevchenko 2 (16/09/2023)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Tracy Cortez |
|---------|:-------------------:|:------------:|
| Sig Strikes Conectados | 77 | 103 |
| Sig Strikes Tentados | 206 | 212 |
| Precisão (%) | 37% | 49% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 2/10 | 0/1 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 3:00 | 0:26 |
| Controle (%) | 20% | 3% |

##### Pontos Negativos

- 2/10 quedas, 20% de precisão — a média dela é 54%. Jasmine tentou 10 vezes e completou 2. É o takedown game dela completamente travado. Cortez defendeu 8 de 10 tentativas. Sem a queda funcionando, Jasmine fica dependente do standup — e perdeu lá também: 77 vs 103, saldo de -1.73/min.
- 206 tentativas de striking com 37% de precisão — a média dela é 45%, 8 pontos abaixo com o maior volume do recorte. Foi uma luta de busca de solução que não encontrou: volume alto, quedas travadas, saldo negativo. R1 praticamente sem controle (5 segundos), R2 (1:52) e R3 (1:03) recuperando parcialmente, mas já tarde.

---

#### 3. vs Natalia Silva — UFC Fight Night: Kattar vs. Emmett (18/06/2022)
**Decisão | R3 5:00 | Peso Mosca**

##### Dados Objetivos

| Métrica | Jasmine Jasudavicius | Natalia Silva |
|---------|:-------------------:|:-------------:|
| Sig Strikes Conectados | 31 | 96 |
| Sig Strikes Tentados | 101 | 185 |
| Precisão (%) | 31% | 52% |
| Knockdowns | 0 | 0 |
| Quedas Aplicadas | 0/6 | 2/3 |
| Tentativas de Sub | 0 | 0 |
| Controle (tempo) | 3:37 | 1:07 |
| Controle (%) | 24% | 7% |

##### Pontos Negativos

- 0/6 quedas, 0% de precisão — a média dela é 54%. Seis tentativas sem converter nenhuma. Natalia travou completamente o grappling de Jasmine e ainda completou 2/3 das próprias. Resultado: Natalia conectou 96 vs 31 de Jasmine com saldo de -4.33/min. Quando o takedown não funciona e o striker adversário é bom, é esse placar.
- 31% de precisão no striking — 14 pontos abaixo da média. 58% dos golpes de Jasmine foram no corpo (vs média de 17%) — o padrão mais desviante de todo o recorte. É o estilo mais raro que ela usa e não rendeu: 31 acertos de 101 tentativas. Natalia ficou no standup, acertou mais do que o dobro e ganhou com folga.

---

## Capítulo 7: Análise Round a Round — Karine Silva

> Como Karine se comporta em cada round — volume, precisão, knockdowns, grappling.

### Perfil Geral

- **Total de lutas analisadas:** 7
- **Categoria:** Peso Mosca
- **Resultado geral:** 5V–2D (nos dados disponíveis)
- **Vitórias por método:** 3 Finalização (todas no R1), 2 Decisão
- **Derrotas por método:** 2 Decisão
- **Lutas com dados de R2 e R3:** 4 (vs Ariane da Silva, vs Viviane Araujo, vs Dione Barbosa, vs Maycee Barber)

---

### Dados Frios — Médias por Round

| Métrica | R1 (n=7) | R2 (n=4) | R3 (n=4) |
|---------|:--------:|:--------:|:--------:|
| **Striking** | | | |
| Golpes sig. conectados/min | 2.9 | 2.1 | 2.4 |
| Tentativas/min | 8.0 | 3.5 | 6.2 |
| Precisão | 35% | 61% | 33% |
| KD/5min | 0.1 | 0.0 | 0.0 |
| **Grappling** | | | |
| Quedas/5min | 1.0 | 1.0 | 0.8 |
| Precisão de quedas | 83% | 58% | 39% |
| Subm. tentativas/5min | 0.7 | 0.3 | 0.5 |
| **Posicional** | | | |
| Controle (%) | 30% | 39% | 21% |
| **Saldos** | | | |
| Saldo sig./min | +0.3 | -0.5 | -1.2 |
| Saldo quedas/5min | +0.8 | +0.3 | -0.5 |

---

### Dados Frios — Variações Médias Round a Round

| Métrica | R1→R2 (n=4) | R2→R3 (n=4) |
|---------|:-----------:|:-----------:|
| Vol. sig. conectados/min | -0.2 | +0.3 |
| Tentativas/min | -3.1 | +2.7 |
| Precisão | +27% | -27% |
| Quedas/5min | +0.5 | -0.3 |
| Tentativas quedas/5min | +1.3 | 0.0 |
| Precisão quedas | +25% | -29% |
| Controle | +15% | -18% |
| Saldo sig./min | 0.0 | -0.7 |

---

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos (%)

| Alvo | R1 (n=7) | R2 (n=4) | R3 (n=4) |
|------|:--------:|:--------:|:--------:|
| Cabeça | 36% | 47% | 30% |
| Corpo | 21% | 30% | 31% |
| Perna | 42% | 23% | 39% |

#### Posição (%)

| Posição | R1 (n=7) | R2 (n=4) | R3 (n=4) |
|---------|:--------:|:--------:|:--------:|
| Distância | 85% | 61% | 85% |
| Clinch | 6% | 15% | 15% |
| Chão | 9% | 24% | 0% |

---

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Resultado | Método | SLPM | Precisão | TD/5min | Prec. TD | Controle | Saldo sig./min |
|------|---------|-----------|--------|:----:|:--------:|:-------:|:--------:|:--------:|:--------------:|
| 04/06/2022 | Poliana Botelho | **V** | Finalização (R1) | 3.5 | 25% | 1.0 | 100% | 16% | -0.41 |
| 03/06/2023 | Ketlen Souza | **V** | Finalização (R1) | 1.7 | 30% | 2.9 | 100% | 77% | +1.71 |
| 19/08/2023 | Maryna Moroz | **V** | Finalização (R1) | 6.0 | 57% | 1.0 | 100% | 17% | +2.81 |
| 27/04/2024 | Ariane da Silva | **V** | Decisão (R3) | 1.8 | 36% | 1.7 | 83% | 50% | -1.00 |
| 16/11/2024 | Viviane Araujo | **D** | Decisão (R3) | 3.9 | 44% | 0.4 | 14% | 23% | +0.67 |
| 16/08/2025 | Dione Barbosa | **V** | Decisão (R3) | 1.7 | 37% | 0.3 | 33% | 16% | -0.33 |
| 06/12/2025 | Maycee Barber | **D** | Decisão (R3) | 1.4 | 47% | 0.7 | 67% | 23% | -2.27 |

---

### Análise Técnica

- O R2 é o round mais eficiente de Karine em precisão de striking (61%), mas não em resultado: o volume cai demais e o saldo ainda fica negativo. O R3 é o oposto ruim: o volume volta, a precisão cai para 33% e o saldo despenca para -1.2/min.

- O grappling degrada com a duração da luta. A precisão de quedas cai de 83% no R1 para 39% no R3, o controle recua de 30% para 21% e os golpes de solo simplesmente desaparecem no round final.

- As derrotas compartilham um núcleo comum: Karine não sustenta controle nem defesa de queda quando a luta amadurece. As vitórias por decisão vieram por rotas diferentes, mas as derrotas não: ambas pediram mais tempo de luta do que o jogo dela conseguiu administrar.

---

### Brechas e Insights

**1.** O jogo no chão depende de um primeiro takedown limpo. Quando a defesa adversária sobrevive ao R1, o ground-and-pound quase some e Karine passa a viver de um striking que não ganha saldo suficiente.

**2.** O R3 é o round da pior tomada de decisão técnica: mais volume, menos precisão, menos controle. Não parece só fadiga; parece também perda de qualidade de entrada.

**3.** A luta contra Viviane confirma a prioridade tática: vencer o striking não basta se o grappling for perdido. Em Karine, a luta muda de dono quando a queda muda de dono.

---

### Visão de Coach

#### Se eu fosse da equipe adversária:

- Priorizar defesa de takedown no R1. Se a primeira queda não entra, o chão dela perde peso rápido.
- Alongar a luta e aumentar o volume no R2-R3. Quanto mais a luta dura, pior fica o saldo técnico de Karine.
- Negar o clinch limpo e forçar entradas da distância, onde a qualidade das quedas cai.

#### Se eu fosse da equipe da Karine:

- Treinar setup de queda para rounds tardios, não repetição cega de entrada. O R3 pede qualidade, não insistência.
- Preservar o R2 como round de controle e economia, não de urgência. O pior cenário dela nasce quando acelera sem critério.
- Recuperar produção real de solo depois do primeiro round; sem isso, a luta vira disputa em pé onde ela joga em déficit.

---

## Capítulo 8: Análise Round a Round — Jasmine Jasudavicius

> Como Jasmine se comporta em cada round — volume, precisão, knockdowns, grappling.

### Perfil Geral

- **Total de lutas analisadas:** 11
- **Categoria:** Peso Mosca
- **Resultado geral:** 8V–3D (nos dados disponíveis)
- **Vitórias por método:** 5 Decisão, 3 Finalização
- **Derrotas por método:** 2 Decisão, 1 KO/TKO
- **Lutas com dados de R2 e R3:** 9 (todas exceto vs Jessica Andrade — Finalização R1 — e vs Manon Fiorot — KO/TKO R1)

---

### Dados Frios — Médias por Round

| Métrica | R1 (n=11) | R2 (n=9) | R3 (n=9) |
|---------|:---------:|:--------:|:--------:|
| **Striking** | | | |
| Golpes sig. conectados/min | 3.1 | 3.6 | 4.0 |
| Tentativas/min | 7.3 | 6.9 | 9.4 |
| Precisão | 45% | 54% | 44% |
| KD/5min | 0.0 | 0.1 | 0.0 |
| **Grappling** | | | |
| Quedas/5min | 0.8 | 0.9 | 0.8 |
| Precisão de quedas | 63% | 65% | 32% |
| Subm. tentativas/5min | 0.2 | 0.2 | 0.5 |
| **Posicional** | | | |
| Controle (%) | 41% | 58% | 43% |
| **Saldos** | | | |
| Saldo sig./min | -1.0 | +0.3 | 0.0 |
| Saldo quedas/5min | +0.7 | +0.6 | +0.8 |

Amostra pequena — nota de contexto R1: a luta contra Manon Fiorot (derrota por KO no R1, saldo de striking de -11.35/min) está incluída no n=11. Esse dado puxa o saldo médio do R1 para baixo; sem ela, o saldo do R1 seria menos negativo. Use o -1.0/min como sinal direcional, não como padrão consolidado de R1.

---

### Dados Frios — Variações Médias Round a Round

| Métrica | R1→R2 (n=9) | R2→R3 (n=9) |
|---------|:-----------:|:-----------:|
| Vol. sig. conectados/min | +0.5 | +0.4 |
| Tentativas/min | 0.0 | +2.6 |
| Precisão | +8% | -10% |
| Quedas/5min | +0.1 | -0.1 |
| Tentativas quedas/5min | +0.3 | +0.9 |
| Precisão quedas | +10% | -32% |
| Subm. tentativas/5min | +0.2 | +0.2 |
| Controle | +13% | -16% |
| Saldo sig./min | +0.6 | -0.3 |

---

### Dados Frios — Distribuição de Alvos e Posições por Round

#### Alvos (%)

| Alvo | R1 (n=11) | R2 (n=9) | R3 (n=9) |
|------|:---------:|:--------:|:--------:|
| Cabeça | 70% | 61% | 65% |
| Corpo | 18% | 31% | 30% |
| Perna | 13% | 8% | 5% |

#### Posição (%)

| Posição | R1 (n=11) | R2 (n=9) | R3 (n=9) |
|---------|:---------:|:--------:|:--------:|
| Distância | 72% | 62% | 73% |
| Clinch | 10% | 15% | 14% |
| Chão | 19% | 24% | 14% |

---

### Dados Frios — Detalhamento Luta a Luta

| Data | Oponente | Resultado | Método | SLPM | Precisão | TD/5min | Prec. TD | Controle | Saldo sig./min |
|------|---------|-----------|--------|:----:|:--------:|:-------:|:--------:|:--------:|:--------------:|
| 22/01/2022 | Kay Hansen | **V** | Decisão (R3) | 3.33 | 45% | 0.7 | 67% | 40% | +0.40 |
| 18/06/2022 | Natalia Silva | **D** | Decisão (R3) | 2.07 | 31% | 0.0 | 0% | 24% | -4.33 |
| 25/02/2023 | Gabriella Fernandes | **V** | Decisão (R3) | 1.60 | 44% | 1.4 | 50% | 77% | -0.13 |
| 10/06/2023 | Miranda Maverick | **V** | Decisão (R3) | 4.47 | 42% | 0.4 | 100% | 51% | +0.27 |
| 16/09/2023 | Tracy Cortez | **D** | Decisão (R3) | 5.13 | 37% | 0.7 | 20% | 20% | -1.73 |
| 20/01/2024 | Priscila Cachoeira | **V** | Finalização (R3) | 6.48 | 78% | 0.7 | 40% | 80% | +4.81 |
| 13/07/2024 | Fatima Kline | **V** | Decisão (R3) | 2.67 | 45% | 1.4 | 67% | 52% | +0.07 |
| 02/11/2024 | Ariane da Silva | **V** | Finalização (R3) | 2.89 | 43% | 1.2 | 60% | 46% | -0.48 |
| 01/02/2025 | Mayra Bueno Silva | **V** | Decisão (R3) | 3.73 | 53% | 1.0 | 60% | 48% | +1.27 |
| 10/05/2025 | Jessica Andrade | **V** | Finalização (R1) | 4.13 | 61% | 1.9 | 50% | 45% | +2.63 |
| 18/10/2025 | Manon Fiorot | **D** | KO/TKO (R1) | 1.62 | 14% | 0.0 | -- | 0% | -11.35 |

---

### Análise Técnica

- O striking de Jasmine melhora do R1 para o R2 por precisão, não por volume. Ela lê melhor a luta, acerta mais e estabiliza o saldo mesmo sem grande salto de tentativas.

- O grappling atinge o pico no R2 e perde eficiência no R3. A precisão de quedas cai de 65% para 32% justamente quando as tentativas aumentam, sinal de wrestling mais forçado do que limpo no round final.

- Nas decisões, o controle separa quase tudo: controle alto sustenta vitórias apertadas; controle baixo acompanha as derrotas. Quando ela não instala o jogo posicional, o resto da luta fica exposto.

---

### Brechas e Insights

**1.** O R1 ainda é o round mais vulnerável dela em pé. Se o grappling não começa cedo, Jasmine tende a ceder mais do que entrega antes de estabilizar a luta.

**2.** O R3 concentra um risco claro: mais tentativa de queda com menos conversão. Quando a luta aperta, ela aumenta a frequência antes de manter a limpeza.

**3.** As derrotas por decisão reforçam a regra do perfil: sem chão, sem controle, sem placar. O grappling não é complemento; é a estrutura que segura a luta inteira.

---

### Visão de Coach

#### Se eu fosse da equipe adversária:

- Pressionar o striking do R1 e negar a primeira sequência de grappling. Esse é o ponto mais exposto do perfil.
- Defender o takedown desde o início e forçar o R3 em pé, onde ela aumenta a tentativa antes de sustentar a eficiência.
- Não aceitar clinch estável no R2, porque é ali que o controle dela costuma se consolidar.

#### Se eu fosse da equipe da Jasmine:

- Reduzir o déficit de striking do R1 para não depender tanto do grappling como amortecedor.
- Melhorar a qualidade das quedas do R3; o problema ali é menos esforço e mais limpeza de entrada.
- Proteger o controle do R2 como eixo da luta, porque é ali que ela mais consistentemente constrói vitória.

---

## Capítulo 9: Perfil vs Média — Karine Silva

> Karine no contexto do top 15 do Peso Mosca Feminino. Os números dos capítulos anteriores ganham escala aqui.

**Categoria:** Peso Mosca
**Gênero:** Feminino
**Grupo de comparação:** top15 (14 lutadoras)
**Data da análise:** 2026-04-10

---

### Grupo de Comparação

| # | Lutadora |
|---|---------|
| Campeã | Valentina Shevchenko |
| 1 | Natalia Silva |
| 1 | Manon Fiorot |
| 3 | Alexa Grasso |
| 4 | Erin Blanchfield |
| 5 | Maycee Barber |
| 7 | Rose Namajunas |
| 7 | Jasmine Jasudavicius |
| 8 | Tracy Cortez |
| 9 | Karine Silva **(analisada)** |
| 10 | Miranda Maverick |
| 12 | Casey O'Neill |
| 14 | JJ Aldrich |
| 14 | Gabriella Fernandes |

---

### Outliers Positivos — Elite (3 métricas)

| Métrica | Valor | Média | Percentil | n |
|---------|------:|------:|----------:|--:|
| media_finalizacoes_15min | 2.00 | 0.48 | 93% | 14 |
| perc_vitorias_viarapida | 0.89 | 0.42 | 93% | 14 |
| vitorias_1_round | 3 | 0.79 | 93% | 14 |

Três outliers de elite na mesma direção: ela termina lutas antes do tempo. Média de 2 finalizações por 15 minutos — 4x acima dos 0.48 de média do grupo. 89% das vitórias por via rápida (p93). 3 vitórias no primeiro round, contra 0.79 de média. O mecanismo é queda + finalização: 60% das vitórias no UFC por finalização, com média de 23.88 minutos acumulados para fechar — o menor do grupo (grupo em 66.85, n=9). Quando chega ao adversário, a luta tem prazo.

---

### Acima da Média — Destaques (34 métricas)

- **derrotas_ko_tko_ufc**: 0 (p0, média 0.21) *(menor=melhor: p0 = melhor do grupo)*
- **derrotas_finalizacao_ufc**: 0 (p0, média 0.29) *(menor=melhor)*
- **perc_derrotas_ko_tko_ufc**: 0.00 (p0, média 0.05) *(menor=melhor)*
- **perc_derrotas_finalizacao_ufc**: 0.00 (p0, média 0.11) *(menor=melhor)*
- **knockdowns_sofridos_por_5min**: 0.00 (p0, média 0.02) *(menor=melhor)*
- *+29 métricas adicionais (destaques: perc_vitorias_finalizacao_ufc p93, taxa_vitoria_no_r1 p93, tentativas_sub_causadas_por_5min p93, perc_precisao_quedas p86, golpes_pernas_por_min p86)*

Nunca perdeu por KO/TKO ou finalização no UFC, nunca foi nocauteada. O queixo resiste; o problema não é colapso físico. Nos destaques adicionais, o que mais define o perfil ofensivo: 60% precisão de queda (p86, contra 37% de média), 0.40 tentativas de submissão por 5min (p93, 3x a média), 0.84/min de golpes de perna (p86). As pernas são usadas em pé para manter distância e abrir espaço antes de buscar o chão — não é striking puro, é transição.

---

### Outliers Negativos — Pontos Fracos Críticos (4 métricas)

| Métrica | Valor | Média | Percentil | n |
|---------|------:|------:|----------:|--:|
| perc_vitorias_decisao | 0.11 | 0.58 | 0% | 14 |
| perc_defesa_quedas | 0.14 | 0.65 | 0% | 14 |
| golpes_sig_conectados_total | 182 | 548 | 0% | 14 |
| golpes_sig_desferidos_total | 453 | 1191 | 0% | 14 |

Quatro outliers negativos com a mesma leitura: não compete bem em lutas longas. Defesa de queda de 14% (p0), o menor do grupo por larga margem, significa que quando alguém quer ir ao chão com ela, vai. 11% de vitórias por decisão (p0): se a luta chega ao juízo, ela perde. Volume de striking total 67% abaixo da média do grupo — não é estilo, é ausência de instrumento. SLPM de 2.56 (mais detalhes abaixo) confirma: a troca à distância não é o plano.

---

### Abaixo da Média — Pontos de Atenção (46 métricas)

- **sequencia_vitorias_atual**: 0 (p0, média 1.86)
- **vitorias_decisao**: 2 (p0, média 6.43)
- **slpm_conectados_min**: 2.56 (p0, média 4.23)
- **perc_defesa_striking**: 0.49 (p0, média 0.59)
- **resiliencia_nocaute**: 0.78 (p0, média 0.83)
- *+41 métricas adicionais (destaques relevantes: qnt_lutas_ufc p7, taxa_sobrevivencia_derrota p14, perc_precisao_striking p14, saldo_striking_por_min p29)*

Vem de derrota — sequência atual zerada. Só 2 vitórias por decisão em toda a carreira (p0): o perfil é finalizadora ou derrotada. SLPM de 2.56 é o menor do top15 — não conecta volume em pé. Defesa de striking de 49% (p0) é o pior do grupo — absorve quando trocas acontecem. Taxa de sobrevivência em derrota de 50% (p14): quando perde, perde antes do tempo final. Saldo de striking de -0.38/min (grupo em +0.84) fecha o quadro: quanto mais a luta dura em pé, mais o saldo pesa contra ela. Apenas 7 lutas no UFC (p7) — alguns números refletem histórico curto, não tendência consolidada.

---

### Métricas Neutras — Perfil de Estilo (10 métricas)

- **perc_golpes_cabeca**: 0.40 (p0, média 0.66)
- **perc_carreira_no_ufc**: 0.28 (p0, média 0.55)
- **pct_luta_lutada_medio**: 0.68 (p0, média 0.84)
- **perc_golpes_corpo**: 0.24 (p93, média 0.18)
- **perc_golpes_pernas**: 0.36 (p93, média 0.16)
- *+5 métricas adicionais*

Distribuição de golpes inverte o padrão do grupo: só 40% na cabeça (p0, contra 66% de média), 36% nas pernas (p93) e 24% no corpo (p93). Não é boxer — usa golpes para aproximar e abrir o grappling. perc_carreira_no_ufc de 28% (p0) é o menor do top15: a maior parte da carreira foi fora do octógono, o que contextualiza o volume baixo de dados no UFC. pct_luta_lutada_medio de 0.68 (p0) — as lutas dela são curtas por design, não por acidente.

---

### Resumo Quantitativo

| Classificação | Qtd | % |
|---------------|----:|--:|
| Outliers Positivos (Elite) | 3 | 3% |
| Acima da Média | 34 | 34% |
| Abaixo da Média | 46 | 46% |
| Outliers Negativos (Críticos) | 4 | 4% |
| Neutras (Perfil) | 10 | 10% |
| Na Média (suprimido) | 4 | 4% |

**3% de elite. 34% acima da média. 46% abaixo. 4% como pontos críticos.**

Karine Silva é finalizadora de alta eficiência com exposição estrutural em lutas longas. Os 3 outliers de elite estão todos na mesma direção — terminar rápido. Os 4 outliers negativos estão todos na direção oposta — quando não termina. O perfil é binário: ou acaba no chão em pouco tempo, ou os números em pé e ao longo dos rounds trabalham contra ela. Contra Jasmine, a defesa de queda de 14% é o número que mais importa.

---

## Capítulo 10: Perfil vs Média — Jasmine Jasudavicius

> Jasmine no contexto do top 15. O espelho do capítulo anterior — e onde os perfis se encontram.

**Categoria:** Peso Mosca
**Gênero:** Feminino
**Grupo de comparação:** top15 (14 lutadoras)
**Data da análise:** 2026-04-10

---

### Grupo de Comparação

| # | Lutadora |
|---|---------|
| Campeã | Valentina Shevchenko |
| 1 | Natalia Silva |
| 1 | Manon Fiorot |
| 3 | Alexa Grasso |
| 4 | Erin Blanchfield |
| 5 | Maycee Barber |
| 7 | Rose Namajunas |
| 7 | Jasmine Jasudavicius **(analisada)** |
| 8 | Tracy Cortez |
| 9 | Karine Silva |
| 10 | Miranda Maverick |
| 12 | Casey O'Neill |
| 14 | JJ Aldrich |
| 14 | Gabriella Fernandes |

---

### Outliers Positivos — Elite (0 métricas)

Nenhuma métrica no percentil de outlier positivo. O perfil de Jasmine não tem pico isolado de elite — a vantagem é distribuída no grappling, não concentrada em um número único que a separe do grupo.

---

### Acima da Média — Destaques (47 métricas)

- **derrotas_finalizacao**: 0 (p0, média 0.79) *(menor=melhor: p0 = melhor do grupo)*
- **derrotas_finalizacao_ufc**: 0 (p0, média 0.29) *(menor=melhor)*
- **perc_derrotas_finalizacao**: 0.00 (p0, média 0.18) *(menor=melhor)*
- **perc_derrotas_finalizacao_ufc**: 0.00 (p0, média 0.11) *(menor=melhor)*
- **knockdowns_sofridos_por_5min**: 0.00 (p0, média 0.02) *(menor=melhor)*
- *+42 métricas adicionais (destaques: pct_ctrl_medio_lutas p93, golpes_solo_total p93, tentativas_queda_por_5min p86, media_quedas_15min p86)*

Os cinco maiores desvios positivos são todos zeros em métricas de dano recebido — nunca foi finalizada em toda a carreira, nunca levou knockdown. O mecanismo: ela vai ao chão com frequência abaixo da média do grupo (quedas_sofridas_por_5min: 0.15 contra 0.39, p7) e quando vai, não é submetida. Fora das zeros, os números que definem o perfil são controle de luta médio de 44% (p93, quase o dobro dos 24% de média) e 114 golpes do solo (p93, contra 62 de média). A plataforma é wrestle-and-pound: ela chega ao chão, ocupa posição e bate.

---

### Outliers Negativos — Pontos Fracos Críticos (2 métricas)

| Métrica | Valor | Média | Percentil | n |
|---------|------:|------:|----------:|--:|
| perc_derrotas_ko_tko_ufc | 0.33 | 0.05 | 93% | 14 |
| derrotas_ko_tko_ufc | 1 | 0.21 | 79% | 14 |

33% das derrotas no UFC vieram por KO/TKO — a média do grupo é 5%, percentil 93. Quase ninguém no top15 perde tanto por nocaute proporcionalmente. O caminho está claro: saldo de striking negativo (-0.30/min), defesa de striking de 51% (p14), zero KOs aplicados no UFC. Quando a luta permanece em pé por tempo suficiente, o acúmulo de dano abre a derrota por nocaute.

---

### Abaixo da Média — Pontos de Atenção (41 métricas)

- **sequencia_vitorias_atual**: 0 (p0, média 1.86)
- **vitorias_ko_tko**: 0 (p0, média 2.93)
- **perc_vitorias_ko_tko**: 0.00 (p0, média 0.20)
- **vitorias_ko_tko_ufc**: 0 (p0, média 1.29)
- **perc_vitorias_ko_tko_ufc**: 0.00 (p0, média 0.15)
- *+36 métricas adicionais (destaques relevantes: golpes_pernas_por_min p7, perc_defesa_striking p14, saldo_striking_por_min p36)*

Não tem KO/TKO em nenhum momento da carreira — esse caminho de vitória não existe para ela. A sequência atual de 0 vitórias reflete a derrota recente. O que importa para este contexto específico: golpes de perna em 0.29/min (p7, contra 0.58 de média) e defesa de striking de 51% (p14). Ela não usa pernas e não bloqueia bem em pé — duas brechas que se abrem diretamente contra uma adversária com 0.84/min de chutes como Karine.

---

### Métricas Neutras — Perfil de Estilo (10 métricas)

- **perc_golpes_pernas**: 0.09 (p7, média 0.16)
- **perc_golpes_em_pe**: 0.74 (p14, média 0.79)
- **perfil_distancia_luta**: 0.48 (p14, média 0.59)
- **perc_golpes_clinche**: 0.07 (p50, média 0.09)
- **perc_golpes_solo**: 0.19 (p79, média 0.12)
- *+5 métricas adicionais*

74% dos golpes na cabeça (p79 do grupo), 9% de pernas (p7). Perfil de distância de 0.48 contra 0.59 de média — opera mais no clinche e no chão. DNA de estilo equilibrado em 0.39 (p79), acima da média, confirma que mescla grappling com striking mesmo sem usar pernas.

---

### Resumo Quantitativo

| Classificação | Qtd | % |
|---------------|----:|--:|
| Outliers Positivos (Elite) | 0 | 0% |
| Acima da Média | 47 | 46% |
| Abaixo da Média | 41 | 40% |
| Outliers Negativos (Críticos) | 2 | 2% |
| Neutras (Perfil) | 10 | 10% |
| Na Média (suprimido) | 4 | 4% |

**0% de elite. 46% acima da média. 40% abaixo. 2% como pontos críticos.**

Jasmine Jasudavicius é wrestler de pressão sem nenhum outlier de elite — consistência no grappling, sem pico isolado. A vulnerabilidade ao KO define o único caminho de derrota dela: acúmulo de dano em pé. O controle de luta de 44% médio é a resposta para fechar esse caminho — e contra Karine com defesa de queda de 14%, o acesso ao chão não é incerto.

---

## Capítulo 11: Cruzamento de Dados Frios

> Dados brutos lado a lado. O comparativo direto que sustenta toda a análise anterior.

> Nota metodológica: `Ficha Técnica` e `Carreira Geral` usam carreira completa. `Carreira no UFC` e os blocos técnicos abaixo usam o recorte UFC ponderado de 7 lutas da Karine e 11 da Jasmine.

### Ficha Técnica

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| Categoria | Peso Mosca | Peso Mosca | - |
| Postura | Destro | Destro | - |
| Ranking na Categoria | 9 🔴 | 7 🟢 | **Jasmine Jasudavicius** |
| Ranking PFP | Desranqueado | Desranqueado | - |
| Idade (anos) | 32 🟢 | 37 🔴 | **Karine Silva** |
| Altura (cm) | 165 🔴 | 170 🟢 | **Jasmine Jasudavicius** |
| Envergadura (cm) | 170 🔴 | 173 🟢 | **Jasmine Jasudavicius** |
| Alcance Extra (cm) | 5 🟢 | 3 🔴 | **Karine Silva** |

---

### Carreira Geral

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| Total de Lutas | 25 🟢 | 18 🔴 | **Karine Silva** |
| Vitórias | 19 🟢 | 14 🔴 | **Karine Silva** |
| Derrotas | 6 🔴 | 4 🟢 | **Jasmine Jasudavicius** |
| Taxa de Vitória | 76% 🔴 | 78% 🟢 | **Jasmine Jasudavicius** |
| Sequência de Vitórias Atual | 0 | 0 | Empate |
| Vitórias por KO/TKO | 8 | 2 | - |
| Vitórias por Finalização | 9 | 4 | - |
| Vitórias por Decisão | 2 | 8 | - |
| Vitórias no 1º Round | 3 | 3 | Empate |
| % Vitórias Via Rápida | 89% 🟢 | 43% 🔴 | **Karine Silva** |
| % Vitórias por KO/TKO | 42% | 14% | - |
| % Vitórias por Finalização | 47% | 29% | - |
| % Vitórias por Decisão | 11% | 57% | - |
| % Derrotas por KO/TKO | 17% | 25% | - |
| % Derrotas por Finalização | 33% | 0% | - |
| % Derrotas por Decisão | 50% | 75% | - |
| Tempo Médio de Luta | 09:48 | 12:34 | - |

---

### Carreira no UFC

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| Lutas no UFC | 7 🔴 | 11 🟢 | **Jasmine Jasudavicius** |
| Vitórias no UFC | 5 🔴 | 8 🟢 | **Jasmine Jasudavicius** |
| Derrotas no UFC | 2 🟢 | 3 🔴 | **Karine Silva** |
| % Carreira no UFC | 28% 🔴 | 61% 🟢 | **Jasmine Jasudavicius** |
| Tempo Total no UFC (min) | 72 🔴 | 136 🟢 | **Jasmine Jasudavicius** |
| Vitórias UFC por KO/TKO | 0 | 0 | Empate |
| Vitórias UFC por Finalização | 3 | 3 | Empate |
| Vitórias UFC por Decisão | 2 🔴 | 5 🟢 | **Jasmine Jasudavicius** |
| % Vitórias UFC por Finalização | 60% | 38% | - |
| % Vitórias UFC por Decisão | 40% | 62% | - |
| Derrotas UFC por KO/TKO | 0 🟢 | 1 🔴 | **Karine Silva** |
| Derrotas UFC por Finalização | 0 | 0 | Empate |
| Derrotas UFC por Decisão | 2 | 2 | Empate |
| % Derrotas UFC por KO/TKO | 0% 🟢 | 33% 🔴 | **Karine Silva** |
| % Derrotas UFC por Decisão | 100% 🔴 | 67% 🟢 | **Jasmine Jasudavicius** |

---

### Striking

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| Golpes Sig. Conectados/min | 2.56 🔴 | 3.47 🟢 | **Jasmine Jasudavicius** |
| Golpes Sig. Absorvidos/min | 2.94 🟢 | 3.77 🔴 | **Karine Silva** |
| Precisão de Striking | 42% 🔴 | 45% 🟢 | **Jasmine Jasudavicius** |
| Defesa de Striking | 49% 🔴 | 51% 🟢 | **Jasmine Jasudavicius** |
| Saldo de Striking por Minuto | -0.38 🔴 | -0.30 🟢 | **Jasmine Jasudavicius** |
| Knockdowns Causados/5min | 0.05 | 0.05 | Empate |
| Knockdowns Sofridos/5min | 0.0 | 0.0 | Empate |
| Golpes na Cabeça/min | 1.09 🔴 | 2.45 🟢 | **Jasmine Jasudavicius** |
| Golpes no Corpo/min | 0.61 🔴 | 0.85 🟢 | **Jasmine Jasudavicius** |
| Golpes nas Pernas/min | 0.84 🟢 | 0.29 🔴 | **Karine Silva** |
| Golpes em Pé/min | 1.90 🔴 | 2.31 🟢 | **Jasmine Jasudavicius** |
| Golpes no Clinche/min | 0.40 🔴 | 0.44 🟢 | **Jasmine Jasudavicius** |
| Golpes no Solo/min | 0.24 🔴 | 0.84 🟢 | **Jasmine Jasudavicius** |
| Golpes p/ Nocautear | sem dado | sem dado | - |
| Golpes p/ Ser Nocauteada | sem dado | 512 | - |

---

### Perfil de Striking

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| % Golpes na Cabeça | 40% | 74% | - |
| % Golpes no Corpo | 24% | 17% | - |
| % Golpes nas Pernas | 36% | 9% | - |
| % Golpes em Pé | 76% | 74% | - |
| % Golpes no Clinche | 13% | 7% | - |
| % Golpes no Solo | 11% | 19% | - |

---

### Grappling

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| Quedas Aplicadas/5min | 0.85 🟢 | 0.80 🔴 | **Karine Silva** |
| Quedas Sofridas/5min | 0.65 🔴 | 0.15 🟢 | **Jasmine Jasudavicius** |
| Precisão de Quedas | 60% 🟢 | 54% 🔴 | **Karine Silva** |
| Defesa de Quedas | 14% 🔴 | 76% 🟢 | **Jasmine Jasudavicius** |
| Tentativas de Queda/5min | 1.54 🔴 | 1.88 🟢 | **Jasmine Jasudavicius** |
| Tentativas de Finalização Causadas/5min | 0.40 🟢 | 0.20 🔴 | **Karine Silva** |
| Tentativas de Finalização Sofridas/5min | 0.15 🔴 | 0.05 🟢 | **Jasmine Jasudavicius** |

---

### Índices Compostos

| Dado | Karine Silva | Jasmine Jasudavicius | Vantagem |
|------|:------------:|:--------------------:|:--------:|
| Resiliência ao Nocaute | 0.78 🔴 | 0.81 🟢 | **Jasmine Jasudavicius** |
| Taxa de Vitória no 1º Round | 16% 🟢 | 7% 🔴 | **Karine Silva** |
| % Controle Médio por Luta | 32% 🔴 | 44% 🟢 | **Jasmine Jasudavicius** |
| % Luta Lutada Médio | 68% 🔴 | 82% 🟢 | **Jasmine Jasudavicius** |
| DNA Estilo Equilibrado | 0.36 | 0.39 | - |
| Perfil Distância de Luta | 0.52 | 0.48 | - |

---

**Legenda:** 🟢 Vantagem | 🔴 Desvantagem | Empate = valores idênticos | - = sem dado ou sem vantagem direta
