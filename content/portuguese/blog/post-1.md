---
title: "O Problema do Caixeiro-Viajante: De Gregor Samsa à Max Verstappen e a Busca Incessante pelo Caminho Perfeito."
meta_title: ""
description: "this is meta description"
date: 2025-05-29T05:00:00Z
image: "/images/gallery/post01/cover.png"
categories: ["Ciência da Computação", "Algoritmos", "Analogias"]
author: "Pedro Fernandes"
tags: ["algoritmos", "formula 1"]
draft: false
---

Um caixeiro-viajante é uma pessoa que viaja constantemente para diferentes cidades e regiões a fim de vender produtos em nome de uma empresa. Talvez você se lembre (ou não) mas um exemplo famoso de caixeiro-viajante é o personagem Gregor Samsa, de A Metamorfose. Gregor trabalhava arduamente como caixeiro-viajante para sustentar sua família e pagar uma dívida de seus pais, possuindo uma rotina exaustiva e com diversas pressões no trabalho.

Como um caixeiro-viajante é um vendedor que precisa passar por diversos locais, há a necessidade de escolher a melhor rota para economizar tempo. Para isso, existem dois fatores básicos que precisam ser considerados: distância entre as cidades e a ordem em que elas são visitadas. Além disso, precisamos pensar também que o viajante não deve passar em um mesmo local duas vezes.

Em uma pequena escala, é possível solucionar esse problema facilmente. Observando a imagem ilustrativa abaixo, podemos observar que alguns locais possuem saídas para duas outras cidades enquanto existem alguns que possuem saída para apenas uma cidade. Algo relativamente comum, de acordo com a realidade.

{{< image src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9vw7vft4qzvf1d3qj1ww.png" caption="" alt="alter-text" height="" width="" position="center" command="fill" option="q100" class="img-fluid" title="image title"  webp="false" >}}

Imagine que o primeiro caminho seja:

**Rio de Janeiro, London, Cape Town, Moscow → Distância Resultante: 70 km**

Agora se percorrermos:

**Cape Town, Moscow, London, Rio de Janeiro → Distância Resultante: 90 km**

Ambos os caminhos atendem aos requisitos propostos porém o segundo caminho é mais longo, custoso e cansativo para o caixeiro-viajante. Podemos descobrir isso de forma simples, testando todas as possibilidades e combinações possíveis, algo plausível de se fazer em pequenas situações. Porém apesar de parecer um problema simples, a medida que a quantidade de locais a serem visitados aumenta, mais difícil se torna encontrar boas soluções. E isso se mostrou um verdadeiro pesadelo para muitos matemáticos e cientistas da computação.

Mas ok, agora você pode estar se perguntando o que o Max Verstappen 🦁tem a ver com o caixeiro-viajante. Bom, ambos desgostam de viajar longas distâncias sem necessidade.

> “Eu sempre disse que temos muitas corridas no calendário. Mas acho que o problema maior é viajar pelos diferentes fusos, entre Las Vegas e Catar. Estamos voando para o outro lado do mundo de novo e acho que podemos fazer um trabalho um pouco melhor nas pernas triplas, que estejam um pouco mais próximas. Para mim, isso faria um pouco mais de sentido, então provavelmente é algo que precisamos analisar” — Max Verstappen

Para quem não sabe, Max Verstappen é tetracampeão de Fórmula 1 e no ano de 2025, o campeonato de F1 possui 24 etapas, ou seja, realiza corrida em 24 cidades diferentes, passando por 21 países e 5 continentes.

Com a crescente conscientização da sociedade a respeito do desenvolvimento sustentável, dos impactos ambientais causados pela indústria, do efeito estufa, da pegada zero de Carbono e etc. uma das maiores dificuldades da Fórmula 1 tem sido encontrar a melhor e mais eficiente organização das corridas ao longo do ano pois apesar do que muitos acreditam, o maior impacto ambiental causado pela organização é proveniente de viagens (seja por via marítima, aérea ou terrestre) enquanto a emissão dos carros de corrida consiste em apenas 0.7%.

Voltando à temática computacional, nessa larga escala e com grandes distâncias, tentar encontrar a melhor solução calculando e testando todas as possibilidades seria extremamente exaustivo. Observando a tabela abaixo, apenas com 24 cidades a quantidade de possibilidades se torna impossível de ser calculada à mão e extremamente longa para um computador simples.



| Cidades      | Possíveis Combinações |
|-------------|-----------------------|
|      1      | 1           | 
|      2      | 2           |
|      3      | 6           |
|      4      | 24          |
|      5      | 120         |
|      6      | 720         |
|      7      | 5040        |
|      8      | 40320       |
|      9      | 362880      |
|      10     | 3628800     |
|      11     | 39916800    |
|      12     | 479001600   |
|      24     | 620448401733239439360000   |

E mesmo que, na década de 1980, os pesquisadores Grötschel, Padberg, Rinaldi tenham conseguido resolver o problema com até 2392, o Problema do Caixeiro Viajante continua mais relevante do que nunca. Há quem argumente que a evolução do hardware é a principal solução para os problemas computacionais atuais, a ponto de não precisarmos mais nos preocupar tanto com otimização de algoritmos porém podemos refletir e observar com a história que problemas como o caixeiro viajante e sua discussão ao longo dos anos trouxeram soluções que foram aplicadas em nas mais diferentes áreas. Portanto, mesmo que a evolução do hardware seja um grande avanço, a construção de soluções inteligentes para problemas são igualmente importantes.

A cada nova temporada da F1, com seu calendário global, ou a cada desafio logístico que surge, a necessidade de encontrar a rota mais inteligente persiste, com pesquisadores constantemente desenvolvendo métodos para lidar com a crescente complexidade do mundo real.

Afinal, quem sabe daqui um tempo não precisaremos encontrar as melhores rotas para entre galáxias, estrelas e planetas? 🚀
