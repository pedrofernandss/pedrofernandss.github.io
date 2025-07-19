---
title: "Uma Reflexão Sobre a Representatividade de Dados em Datasets Globais"
# meta_title: ""
# description: ""
date: 2025-07-19T05:17:00Z
image: "/images/gallery/post02/cover.jpg"
categories: ["Inteligência Artificial","Dados","Pesquisas","Projetos"]
author: "Pedro Fernandes"
tags: ["dados","pesquisa","projetos","reflexões"]
draft: false
---

Talvez o maior diferença entre estudar e trabalhar com Inteligência Artificial está na nos dados. Nos cursos e nos pequenos projetos, os dataset são perfeitos. No máximo precisamos fazer uma análise exploratória, converter strings para floats e limpar valores faltantes e outliers. Na vida real, a história é tem se mostrado à mim ser completamente diferente.

Desenvolver um modelo que performe bem e seja de fato útil para a sociedade quando se possui poucos dados ou dados com baixa qualidade é extremamente complicado.

Por meio do IEEE Computational Intelligence Society Student Chapter UnB, atualmente estou trabalhando na construção de uma inteligência artificial que facilite o reencontro de cachorros perdidos com seus tutores. Os algoritmos utilizados para isso, pode ficar para um outro post, agora eu gostaria de falar da base de tudo: os dados!

Quando se fala em qualidade dos dados, deve-se pensar em algumas dimensões como: (1) completeness: todos os dados necessários devem estar presentes, (2) consistency: os dados precisam ser consistentes e uniformes entre datasets diferentes, (3) timeliness: os dados devem estar atualizados e relevantes no tempo de acordo com as necessidades, (4) relevance: os dados devem representar a realidade do contexto em que será utilizado.

No que diz respeito a dimensão de relevance, a algum tempo eu encontrei um artigo chamado ["Does Object Recognition Work for Everyone?"](https://arxiv.org/pdf/1906.02659) escrito pelo Facebook e que se tornou um embasamento teórico muito precioso para o projeto que estou desenvolvendo. Este artigo realiza um comparativo de acurácias alcançadas entre cinco sistemas de reconhecimento de objetos em bases que contenham dados geograficamente diversos. Base de dados com fotos com o mesmo tema porém em fotografadas em regiões diferentes do mundo. Uma situação exemplo seria: dado uma foto de uma prateleira de temperos de cozinha do Estados Unidos, como sistemas de reconhecimento da Google, Azure, Amazon à classificaria? Em seguida dado agora uma outra foto com este mesmo tema, prateleira de temperos de cozinha, porém da Filipinas, como estes sistemas à classificariam?

A pesquisa demonstra que houve uma diferença entre as acurácias atingidas pelos modelos em cenários diferentes. O reconhecimento de itens domésticos de locais com renda familiar média de menos de US$50/mês tinha uma acurácia 10% quando se comparada com as acurácias obtidas no reconhecimento de itens domésticos de locais com renda familiar acima de US$3500/mês. As análises desses resultados indicam que essa queda de performance é primeiramente devido a distinção de aparências entre objetos de uma mesma classe e pelo aparecimento de itens em diferentes contextos e cenários como escovas de dentes aparecendo fora do banheiro.

{{< figure src="/images/gallery/post02/first_image.png" alt="Prateleira de temperos de cozinha" >}}

A conclusão do estudo é dita como: _**"The results of our study suggest that further work is needed to make object-recognition systems work equally well for people across different countries and income levels."**_

Além disso, uma análise dos metadados das imagens presentes no ImageNet - base de dados utilizada para treinar modelos importantes como ResNet50, MobileNet, Inception e YOLO 8 - revela que os dados possuem origem principalmente de países da Europa Ocidental, Estados Unidos e Canadá. Ao pensarmos a situação de maneira mais crítica, percebemos que estas bases de dados, que são utilizadas para o desenvolvimento de modelos state-of-the-art não tem sido diversas o suficiente para se mostrarem representativas em escala global.

{{< figure src="/images/gallery/post02/second_image.png" alt="Infográfico de Dispersão de Fonte de Dados" >}}

Neste contexto, em que as grande base de dados são compostas majoritariamente por informações contextualizadas à realidade norte americana e europeia, surge o questionamento de quando devemos começar a construir nossas próprias base de dados para que sejam representativas à nossa realidade? No projeto "Onde Está Meu Caramelo?" percebemos que no Brasil, há uma quantidade imensa de cachorros SRD (Sem raça definida) conhecidos também como cachorros caramelos e fiapos de manga e bem inferior de, por exemplo Husky's.

Qual o impacto que o uso solo dos dataset's disponíveis on-line teriam na performance do modelo? Considerando que em produção, o modelo irá se deparar com imagens que representem o cotidiano e costumes brasileiros como fazer tranças nos pelos dos cachorros e colocar estrelinha após o pet-shop

💡 Se não existe nada tão representativo assim, talvez caiba a nós mesmos criarmos. 

Dessa forma, estamos construindo uma base de dados de imagens com o apoio da população brasileira para que seja possível realizar o treinamento de modelos (ou pelo menos um fine-tunning) que performem com excelência ao se depararem com dados brasileiros.