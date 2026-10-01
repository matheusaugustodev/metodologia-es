# Estudos de Mapeamento Sistemático em Engenharia de Software

> Tradução para o português do artigo *Systematic Mapping Studies in Software Engineering*, de Kai Petersen, Robert Feldt, Shahid Mujtaba e Michael Mattsson. O original em inglês está em [`Guia-Systematic Mapping Studies in Software Engineering.pdf`](Guia-Systematic%20Mapping%20Studies%20in%20Software%20Engineering.pdf). Tradução feita para fins de estudo; em caso de dúvida, prevalece o texto original. As referências bibliográficas foram mantidas no idioma original.

**Kai Petersen**<sup>1,2</sup>, **Robert Feldt**<sup>1</sup>, **Shahid Mujtaba**<sup>1,2</sup>, **Michael Mattsson**<sup>1</sup>

<sup>1</sup> School of Engineering, Blekinge Institute of Technology, Box 520, SE-372 25 Ronneby — (kai.petersen | robert.feldt | shahid.mujtaba | michael.mattsson)@bth.se
<sup>2</sup> Ericsson AB, Box 518, SE-371 23 Karlskrona — (kai.petersen | shahid.mujtaba)@ericsson.com

## Resumo

**CONTEXTO:** Um mapa sistemático em engenharia de software é um método definido para construir um esquema de classificação e estruturar um campo de interesse da engenharia de software. A análise dos resultados concentra-se nas frequências de publicações para as categorias do esquema. Assim, é possível determinar a cobertura do campo de pesquisa. Diferentes facetas do esquema também podem ser combinadas para responder a perguntas de pesquisa mais específicas.

**OBJETIVO:** Descrevemos como conduzir um estudo de mapeamento sistemático em engenharia de software e fornecemos diretrizes. Também comparamos mapas sistemáticos e revisões sistemáticas para esclarecer como escolher entre eles. Essa comparação leva a um conjunto de diretrizes para mapas sistemáticos.

**MÉTODO:** Definimos um processo de mapeamento sistemático e o aplicamos para concluir um estudo de mapeamento sistemático. Além disso, comparamos mapas sistemáticos com revisões sistemáticas, analisando sistematicamente revisões sistemáticas existentes.

**RESULTADOS:** Descrevemos um processo para estudos de mapeamento sistemático em engenharia de software e o comparamos com revisões sistemáticas. Com base nisso, definimos diretrizes para a condução de mapas sistemáticos.

**CONCLUSÕES:** Mapas e revisões sistemáticas diferem em termos de objetivos, abrangência, questões de validade e implicações. Assim, devem ser usados de forma complementar e exigem métodos diferentes (por exemplo, para a análise).

**Palavras-chave:** Estudos de Mapeamento Sistemático, Revisões Sistemáticas, Engenharia de Software Baseada em Evidências

## 1. Introdução

À medida que uma área de pesquisa amadurece, frequentemente há um aumento acentuado no número de relatos e resultados disponíveis, e torna-se importante resumi-los e fornecer uma visão geral. Muitos campos de pesquisa têm metodologias específicas para esses estudos secundários, amplamente utilizadas, por exemplo, na medicina baseada em evidências. Até recentemente, esse não era o caso na Engenharia de Software (ES). No entanto, uma tendência geral em direção a uma engenharia de software mais baseada em evidências (Kitchenham et al. 2004) levou a um foco maior em métodos de pesquisa novos, empíricos e sistemáticos. Também houve propostas de relato mais estruturado dos resultados, usando, por exemplo, resumos estruturados (Budgen et al. 2007).

A revisão sistemática da literatura é um método de estudo secundário que recebeu muita atenção recentemente em ES (Kitchenham & Charters 2007, Dybå et al. 2006, Hannay et al. 2007, Kampenes et al. 2007) e é inspirado na pesquisa médica. Em resumo, uma revisão sistemática (RS) percorre os relatos primários existentes, revisa-os em profundidade e descreve sua metodologia e resultados. Em comparação com as revisões de literatura comuns em qualquer projeto de pesquisa, uma RS tem vários benefícios: uma metodologia bem definida reduz o viés, uma gama mais ampla de situações e contextos pode permitir conclusões mais gerais, e o uso de meta-análise estatística pode detectar mais do que estudos individuais isoladamente (Kitchenham & Charters 2007). Entretanto, as RSs também têm várias desvantagens, sendo a principal o esforço considerável exigido. Em engenharia de software, as revisões sistemáticas têm se concentrado em estudos quantitativos e empíricos, mas existe um grande conjunto de métodos para sintetizar resultados de pesquisa qualitativa (Dixon-Woods et al. 2005).

O mapeamento sistemático é uma metodologia frequentemente usada na pesquisa médica, mas que tem sido amplamente negligenciada em ES. Até onde sabemos, há apenas um exemplo claro de estudo de mapeamento sistemático em ES (Bailey et al. 2007). Isso pode se dever ao fato de os mapas sistemáticos ainda não terem sido descobertos como método para agregar a pesquisa em engenharia de software.

Um estudo de mapeamento sistemático fornece uma estrutura do tipo de relatos e resultados de pesquisa publicados, categorizando-os. Frequentemente, oferece um resumo visual de seus resultados: o mapa. Exige menos esforço, ao mesmo tempo em que fornece uma visão geral de granularidade mais grossa. Anteriormente, estudos de mapeamento sistemático em engenharia de software eram recomendados principalmente para áreas de pesquisa com falta de estudos primários relevantes e de alta qualidade (Kitchenham & Charters 2007).

Neste artigo, analisamos as diferenças entre revisão sistemática e estudos de mapeamento sistemático e defendemos um conjunto mais amplo de situações em que este último é apropriado. Na Seção 2, descrevemos um processo detalhado para mapas sistemáticos. A Seção 3 resume as revisões sistemáticas existentes em ES e as contrasta com mapas sistemáticos. A Seção 4 discute diretrizes adicionais para mapas sistemáticos, antes de concluirmos na Seção 5.

## 2. O Processo de Mapeamento Sistemático

Adaptamos e aplicamos o mapeamento sistemático à engenharia de software em um estudo focado na variabilidade em linhas de produto de software (Mujtaba et al. 2008). A seguir, detalhamos o processo que utilizamos. Também discutimos algumas das escolhas feitas no mapa sistemático de (Bailey et al. 2007).

**Figura 1: O Processo de Mapeamento Sistemático**

| Etapa do processo | Resultado |
| --- | --- |
| Definição das perguntas de pesquisa | Escopo da revisão |
| Condução da busca | Todos os artigos |
| Triagem dos artigos | Artigos relevantes |
| Atribuição de palavras-chave usando os resumos | Esquema de classificação |
| Extração de dados e processo de mapeamento | Mapa sistemático |

As etapas essenciais do processo do nosso estudo de mapeamento sistemático são: definição das perguntas de pesquisa, condução da busca por artigos relevantes, triagem dos artigos, atribuição de palavras-chave aos resumos e extração de dados e mapeamento (ver Figura 1). Cada etapa do processo tem um resultado, sendo o resultado final do processo o mapa sistemático.

### 2.1. Definição das Perguntas de Pesquisa (Escopo da Pesquisa)

O objetivo principal de um estudo de mapeamento sistemático é fornecer uma visão geral de uma área de pesquisa e identificar a quantidade e o tipo de pesquisa e de resultados disponíveis nela. Frequentemente, deseja-se mapear as frequências de publicação ao longo do tempo para observar tendências. Um objetivo secundário pode ser identificar os fóruns em que a pesquisa na área foi publicada. Esses objetivos se refletem nas perguntas de pesquisa (RQs) de ambos os artigos, que são semelhantes, conforme mostrado na Tabela 1.

**Tabela 1: Perguntas de Pesquisa para Mapas Sistemáticos**

| Mapa de Projeto Orientado a Objetos (Bailey et al. 2007) | Mapa de Variabilidade em Linhas de Produto de Software (Mujtaba et al. 2008) |
| --- | --- |
| **RQ1:** Quais periódicos incluem artigos sobre projeto de software? | **RQ1:** Quais áreas da variabilidade em linhas de produto de software são abordadas e quantos artigos cobrem as diferentes áreas? |
| **RQ2:** Quais são os tópicos de projeto orientado a objetos mais investigados e como eles mudaram ao longo do tempo? | **RQ2:** Que tipos de artigos são publicados na área e, em particular, que tipo de avaliação e de novidade eles constituem? |
| **RQ3:** Quais são os métodos de pesquisa aplicados com mais frequência, e em que contexto de estudo? | |

### 2.2. Condução da Busca por Estudos Primários (Todos os Artigos)

Os estudos primários são identificados usando strings de busca em bases de dados científicas ou navegando manualmente pelos anais de conferências ou publicações de periódicos relevantes. Uma boa forma de criar a string de busca é estruturá-la em termos de população, intervenção, comparação e resultado (*population, intervention, comparison, outcome*) (Kitchenham & Charters 2007). A estrutura deve, naturalmente, ser guiada pelas perguntas de pesquisa. As palavras-chave da string de busca podem ser extraídas de cada aspecto da estrutura. Por exemplo, o resultado de um estudo (p. ex., a acurácia de um método de estimativa) pode levar a palavras-chave como "estudo de caso" ou "experimento", que são abordagens de pesquisa para determinar essa acurácia.

A principal diferença entre os estudos é que não consideramos resultados específicos nem desenhos experimentais em nosso estudo (Mujtaba et al. 2008). Evitamos essa restrição porque queríamos uma visão geral ampla da área de pesquisa como um todo. Se tivéssemos considerado apenas certos tipos de estudos, a visão geral poderia ter sido enviesada e o mapa, incompleto. Alguns subtópicos poderiam estar super ou sub-representados para certos métodos de estudo. Essa diferença também se reflete nas strings de busca:

- **Mapa de Projeto Orientado a Objetos:** `("object oriented" AND "design" AND "empirical evidence") OR ("OO" AND "empirical" AND "design") OR ("software design" AND "OO" AND "experimental")`
- **Mapa de Variabilidade em Linhas de Produto de Software:** `"software" AND ("product line" OR "product family" OR "system family") AND ("variability" OR "variation")`

A escolha das bases de dados também foi diferente. Para o mapa de projeto orientado a objetos, foram considerados todos os resultados das bases de dados relevantes para ciência da computação e engenharia de software. Já nós consideramos apenas os principais fóruns de pesquisa em linhas de produto de software, a saber, a Software Product Line Conference (SPLC)<sup>1</sup> e o Workshop on Product Family Engineering (PFE). Além disso, consideramos também artigos de periódicos. Como a SPLC é o principal fórum de publicação de pesquisa em linhas de produto, ela é um bom ponto de partida para determinar o esquema de classificação e a distribuição dos artigos entre as categorias identificadas.

### 2.3. Triagem dos Artigos para Inclusão e Exclusão (Artigos Relevantes)

Critérios de inclusão e exclusão são usados para excluir estudos que não são relevantes para responder às perguntas de pesquisa. Os critérios da Tabela 2 mostram que as perguntas de pesquisa influenciaram os critérios de inclusão e exclusão; assim, a parte empírica é considerada apenas no mapa de projeto orientado a objetos. Achamos útil excluir artigos que apenas mencionavam nosso foco principal, a variabilidade, em frases introdutórias do resumo. Isso foi necessário porque ela é um conceito central na área e, portanto, é frequentemente usada em resumos sem que os artigos realmente a abordem com mais profundidade. Prototipamos essa técnica e não encontramos nenhuma classificação incorreta decorrente dela.

**Tabela 2: Critérios de Inclusão e Exclusão**

| | Mapa de Projeto Orientado a Objetos (Bailey et al. 2007) | Mapa de Variabilidade em Linhas de Produto de Software (Mujtaba et al. 2008) |
| --- | --- | --- |
| **Inclusão** | Livros, artigos, relatórios técnicos e literatura cinzenta que descrevam estudos empíricos sobre projeto de software orientado a objetos. Quando vários artigos relatavam o mesmo estudo, apenas o mais recente foi incluído. Quando vários estudos eram relatados no mesmo artigo, cada estudo relevante foi tratado separadamente. | O resumo menciona explicitamente variabilidade ou variação no contexto da engenharia de linhas de produto de software. A partir do resumo, o pesquisador consegue deduzir que o foco do artigo contribui para a pesquisa em variabilidade de linhas de produto. |
| **Exclusão** | Estudos que não relataram resultados empíricos ou literatura disponível apenas na forma de resumos ou apresentações de PowerPoint. | O artigo está fora do domínio da engenharia de software. Variabilidade e variação não fazem parte das contribuições do artigo; os termos são mencionados apenas nas frases introdutórias gerais do resumo. |

### 2.4. Atribuição de Palavras-chave aos Resumos (Esquema de Classificação)

Em (Bailey et al. 2007), o processo de criação do esquema de classificação não foi descrito com clareza. Em nosso estudo, seguimos um processo sistemático, mostrado na Figura 2. Aqui, a atribuição de palavras-chave (*keywording*) é uma forma de reduzir o tempo necessário para desenvolver o esquema de classificação e de garantir que o esquema leve em conta os estudos existentes. A atribuição de palavras-chave é feita em duas etapas. Primeiro, os revisores leem os resumos e procuram palavras-chave e conceitos que reflitam a contribuição do artigo. Ao fazer isso, o revisor também identifica o contexto da pesquisa. Em seguida, os conjuntos de palavras-chave dos diferentes artigos são combinados para desenvolver uma compreensão de alto nível sobre a natureza e a contribuição da pesquisa. Isso ajuda os revisores a definir um conjunto de categorias representativo da população subjacente. Quando os resumos têm qualidade baixa demais para permitir a escolha de palavras-chave significativas, os revisores podem optar por estudar também as seções de introdução ou conclusão do artigo. Quando um conjunto final de palavras-chave é escolhido, elas podem ser agrupadas e usadas para formar as categorias do mapa.

**Figura 2: Construção do Esquema de Classificação**

```
Artigos ──► Resumos ──► Atribuição de palavras-chave ──► Esquema de classificação
                                                                │
                                                                ▼
                     Mapa sistemático ◄── Classificar os artigos no esquema
                                                   │        ▲
                                                   ▼        │
                                              Atualizar o esquema
```

Em nosso estudo, foram criadas três facetas principais. Uma faceta estruturou o tópico (isto é, variabilidade em linhas de produto de software), por exemplo, em termos de variabilidade de arquitetura, variabilidade de requisitos, variabilidade de implementação, gerenciamento de variabilidade e assim por diante. Além disso, foi considerado o tipo de contribuição, que poderia ser, por exemplo, um processo, método, ferramenta etc. Essas categorias foram derivadas das palavras-chave. Já a faceta de pesquisa, que reflete a abordagem de pesquisa usada nos artigos, é geral e independente de uma área de foco específica. Escolhemos uma classificação existente de abordagens de pesquisa, de Wieringa et al. (Wieringa et al. 2006), resumida na Tabela 3.

**Tabela 3: Faceta de Tipo de Pesquisa**

| Categoria | Descrição |
| --- | --- |
| **Pesquisa de Validação** (*Validation Research*) | As técnicas investigadas são novas e ainda não foram implementadas na prática. As técnicas usadas são, por exemplo, experimentos, isto é, trabalho realizado em laboratório. |
| **Pesquisa de Avaliação** (*Evaluation Research*) | As técnicas são implementadas na prática e é conduzida uma avaliação da técnica. Isso significa que se mostra como a técnica é implementada na prática (implementação da solução) e quais são as consequências da implementação em termos de benefícios e desvantagens (avaliação da implementação). Isso também inclui identificar problemas na indústria. |
| **Proposta de Solução** (*Solution Proposal*) | É proposta uma solução para um problema; a solução pode ser nova ou uma extensão significativa de uma técnica existente. Os potenciais benefícios e a aplicabilidade da solução são mostrados por um pequeno exemplo ou por uma boa linha de argumentação. |
| **Artigos Filosóficos** (*Philosophical Papers*) | Esses artigos esboçam uma nova forma de olhar para coisas existentes, estruturando o campo na forma de uma taxonomia ou arcabouço conceitual. |
| **Artigos de Opinião** (*Opinion Papers*) | Esses artigos expressam a opinião pessoal de alguém sobre se determinada técnica é boa ou ruim, ou sobre como as coisas deveriam ser feitas. Não se apoiam em trabalhos relacionados nem em metodologias de pesquisa. |
| **Artigos de Experiência** (*Experience Papers*) | Artigos de experiência explicam o que foi feito na prática e como. Deve tratar-se da experiência pessoal do autor. |

Achamos essas categorias fáceis de interpretar e de usar na classificação sem avaliar cada artigo em detalhe (como é feito em uma revisão sistemática). Por exemplo, a pesquisa de avaliação pode ser descartada se nenhuma cooperação com a indústria ou projeto real for mencionado. Além disso, a pesquisa de validação é fácil de identificar, verificando se o artigo declara hipóteses, usa estatísticas descritivas (p. ex., figuras como diagramas de dispersão ou histogramas) e descreve os principais componentes de um arranjo experimental. O esquema também permite classificar pesquisas não empíricas nas categorias proposta de solução, artigos filosóficos, artigos de opinião e artigos de experiência. Em nossa revisão, a maioria dos artigos estava relacionada à categoria não empírica. Outras classificações de tipo de pesquisa foram propostas, e elas são discutidas na Seção 4.

### 2.5. Extração de Dados e Mapeamento dos Estudos (Mapa Sistemático)

Com o esquema de classificação pronto, os artigos relevantes são classificados no esquema, isto é, ocorre a extração de dados propriamente dita. Como mostrado na Figura 2, o esquema de classificação evolui durante a extração de dados, por exemplo, com a adição de novas categorias ou com a fusão e a divisão de categorias existentes. Nesta etapa, usamos uma planilha do Excel para documentar o processo de extração de dados. A planilha continha cada categoria do esquema de classificação. Ao inserir os dados de um artigo no esquema, os revisores forneciam uma breve justificativa de por que o artigo deveria estar em determinada categoria (por exemplo, por que o artigo aplicou pesquisa de avaliação). A partir da planilha final, é possível calcular as frequências de publicações em cada categoria.

A análise dos resultados concentra-se em apresentar as frequências de publicações para cada categoria. Isso permite ver quais categorias foram enfatizadas na pesquisa anterior e, assim, identificar lacunas e possibilidades para pesquisas futuras. Os dois mapas usaram formas diferentes de apresentar e analisar os resultados.

O mapa de projeto orientado a objetos é ilustrado com estatísticas descritivas na forma de tabelas, mostrando as frequências de publicações em cada categoria. No mapa de projeto orientado a objetos, o tipo de intervenção foi usado para estruturar o tópico, contando-se o número de artigos para cada tipo de intervenção. Em nosso estudo, usamos um gráfico de bolhas (*bubble plot*) para relatar as frequências, mostrado na Figura 3. Ele consiste basicamente em dois gráficos de dispersão x-y com bolhas nas interseções das categorias. O tamanho de cada bolha é proporcional ao número de artigos que pertencem ao par de categorias correspondente às coordenadas da bolha. A mesma ideia é usada duas vezes, em quadrantes diferentes do mesmo diagrama, para mostrar a interseção com a terceira faceta. Se um mapa sistemático tiver mais de três facetas, gráficos de bolhas adicionais podem ser acrescentados, seja no mesmo diagrama, seja em vários diagramas para diferentes combinações de facetas. Acreditamos que o gráfico de bolhas apoia a análise melhor do que as tabelas de frequência. É mais fácil considerar diferentes facetas simultaneamente, e estatísticas descritivas ainda podem ser adicionadas para as facetas individualmente. Ele também é mais eficaz em fornecer uma visão geral rápida de um campo e, portanto, em fornecer um mapa. Outras alternativas de visualização podem ser encontradas nos campos de estatística, interação humano-computador (IHC) e visualização de informação.

**Figura 3: Visualização de um Mapa Sistemático na Forma de Gráfico de Bolhas**

> **Nota da tradução:** a figura original é um gráfico de bolhas (ver página 5 do PDF). Ela cruza a **faceta de contexto de variabilidade** (eixo central) com a **faceta de contribuição** (quadrante esquerdo, 118 artigos) e com a **faceta de pesquisa** (quadrante direito, 128 artigos). Abaixo, os números de artigos de cada bolha foram transcritos em tabelas; os percentuais exibidos ao lado das bolhas foram omitidos.

*Contexto de variabilidade × tipo de contribuição*

| Contexto de variabilidade | Métrica | Ferramenta | Modelo | Método | Processo |
| --- | ---: | ---: | ---: | ---: | ---: |
| Variabilidade de requisitos | 3 | 6 | 15 | 17 | 4 |
| Variabilidade de arquitetura | | 1 | 11 | 15 | 8 |
| Variabilidade de implementação | | | 8 | 4 | 1 |
| Verificação e validação | 1 | 2 | 2 | 7 | |
| Gerenciamento de variabilidade | | 1 | 4 | 3 | 3 |
| Variabilidade ortogonal | | | 2 | 1 | |
| **Total (118 = 100%)** | **4 (3,39%)** | **10 (8,48%)** | **42 (35,59%)** | **46 (38,98%)** | **16 (13,56%)** |

*Contexto de variabilidade × tipo de pesquisa*

| Contexto de variabilidade | Pesquisa de avaliação | Pesquisa de validação | Proposta de solução | Artigo filosófico | Relato de experiência | Artigo de opinião |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Variabilidade de requisitos | 13 | | 21 | 2 | | |
| Variabilidade de arquitetura | 17 | | 19 | 5 | 3 | |
| Variabilidade de implementação | 9 | | 3 | 4 | 1 | |
| Verificação e validação | 6 | | 4 | | | |
| Gerenciamento de variabilidade | 3 | | 7 | 2 | 4 | |
| Variabilidade ortogonal | 2 | | 2 | 1 | | |
| **Total (128 = 100%)** | **50 (39,06%)** | **0 (0%)** | **56 (43,75%)** | **14 (10,95%)** | **8 (6,25%)** | **0 (0%)** |

> Na figura original, as bolhas da coluna "Método" somam 47, embora o total indicado seja 46; os valores foram mantidos como no original.

## 3. Análise Comparativa e Discussão

Estudamos as revisões sistemáticas existentes em engenharia de software e as caracterizamos. Isso serve de insumo para a comparação e a discussão desta seção. Os estudos de revisão sistemática foram identificados usando a seguinte string de busca: `"systematic review" AND "software engineering"`, pesquisando nas bases Inspec & Compendex, IEEExplore e ACM Digital Library. A busca resultou em um total de 21 artigos. Excluímos os artigos que não eram da área de engenharia de software, que não se baseavam em (Kitchenham & Charters 2007) ou que não declaravam explicitamente, no título ou no resumo, que eram revisões sistemáticas. Isso resultou na inclusão de oito revisões sistemáticas. Incluímos também duas outras revisões sistemáticas identificadas em (Kitchenham 2007), pois também atendem aos nossos critérios de inclusão. As referências estão resumidas na tabela a seguir.

**Tabela 4: Revisões Sistemáticas Incluídas**

| ID | Referência | ID | Referência |
| --- | --- | --- | --- |
| 1 | (Dybå et al. 2006) | 6 | (Mendes 2005) |
| 2 | (Grimstad et al. 2006) | 7 | (Sjøberg et al. 2005) |
| 3 | (Hannay et al. 2007) | 8 | (Jørgensen & Shepperd 2007) |
| 4 | (Kampenes et al. 2007) | 9 | (MacDonell & Shepperd 2007) |
| 5 | (Kitchenham et al. 2007) | 10 | (Davis et al. 2006) |

### 3.1. Caracterização das Revisões Sistemáticas Existentes

Caracterizamos cada uma das dez revisões sistemáticas de ES incluídas com base em seus objetivos de pesquisa, critérios de inclusão e exclusão, número de inclusões e exclusões, esquema de classificação e meios de análise:

- **Objetivos de pesquisa:** um estudo que visa "Identificar Práticas Melhores e Típicas" analisa um conjunto de estudos empíricos para determinar quais técnicas são usadas e funcionam na prática. Em "Classificação e Taxonomia", o estudo cria um arcabouço ou classifica a pesquisa existente. "Ênfase em Categorias de Tópicos" significa que o estudo identifica quanta pesquisa é publicada em diferentes subtópicos do campo de interesse. Por fim, um estudo que visa "Identificar Fóruns de Publicação" identifica os periódicos, conferências e workshops relevantes na área de foco.
- **Requisitos de inclusão:** foram encontrados dois requisitos principais de inclusão: "A pesquisa está dentro da área de foco" e "Métodos empíricos utilizados". Nesta última categoria, os artigos incluídos usaram métodos empíricos.
- **Número de artigos incluídos:** nesta categoria, identificamos o número de "estudos potencialmente relevantes" (isto é, encontrados na busca) e o número de "artigos incluídos" (após a aplicação dos critérios de inclusão e exclusão, bem como das verificações de qualidade).
- **Meios de análise:** são usados quatro tipos de estudo. "Meta-estudos" integram vários estudos por meio de análises estatísticas dos dados quantitativos desses estudos. A "análise comparativa" usa simplificação lógica e teorias de avaliação de confiança. A "análise temática" conta os artigos relacionados a temas ou categorias específicos. Os "resumos narrativos" concentram-se na revisão qualitativa e em explicações narrativas. Outros meios de análise são descritos em (Dixon-Woods et al. 2005), mas não encontramos evidências de seu uso em revisões sistemáticas de engenharia de software.

O resumo da nossa caracterização é mostrado na Tabela 5; os IDs das referências remetem aos estudos da Tabela 4. Ela mostra que a maioria das revisões visa identificar melhores práticas em engenharia de software (estudos 2, 5, 6, 8, 9 e 10). A maioria delas se concentra no uso de métodos empíricos (ver requisitos de inclusão). Os estudos restantes (1, 3, 4 e 7) impõem requisitos à parte empírica, pois estudam métodos empíricos em ES. Além disso, todas as revisões sistemáticas avaliam se os artigos estão relacionados à área de foco. Apenas duas revisões (7 e 8: Sjøberg et al. 2005, Jørgensen & Shepperd 2007) se concentraram principalmente em classificações e taxonomias e apresentaram frequências de artigos nas categorias identificadas por meio de análise temática. Esses dois estudos também visaram identificar os fóruns de publicação relevantes. O que os distingue dos mapas sistemáticos é sua análise aprofundada, na forma de um resumo narrativo detalhado.

Na tabela, podemos ver que o número de estudos potencialmente relevantes é grande em comparação com o número de estudos incluídos na análise. Vale notar que três das revisões encontradas (Dybå et al. 2006, Hannay et al. 2007, Kampenes et al. 2007) se baseiam nos 103 artigos identificados em um único dos outros estudos (Sjøberg et al. 2005). Como meio de análise, todos os estudos usaram alguma forma de resumo narrativo. Dois estudos usaram análise temática, dois aplicaram meta-análise e um usou análise comparativa.

**Tabela 5: Características das Revisões Sistemáticas**

| ID da referência | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ***Objetivos de pesquisa*** | | | | | | | | | | |
| Identificar práticas melhores e típicas | x | x | x | x | x | x | | | x | x |
| Classificação e taxonomia | | | x | | | | x | x | | |
| Ênfase em categorias de tópicos | | | | | | | x | x | | |
| Identificar fóruns de publicação | | | | | | | x | x | | |
| ***Requisitos de inclusão*** | | | | | | | | | | |
| A pesquisa está dentro da área de foco | x | x | x | x | x | x | x | x | x | x |
| Métodos empíricos utilizados | x | x | x | x | x | | x | | x | x |
| ***Número de artigos incluídos*** | | | | | | | | | | |
| Estudos potencialmente relevantes | 5453 | 963 | 5453 | 5453 | 1344 | 353 | 5453 | n.d. | 185 | 564 |
| Estudos relevantes (incluídos) | 78 | 24 | 24 | 78 | 10 | 173 | 103 | 304 | 10 | 26 |
| ***Meios de análise*** | | | | | | | | | | |
| Meta-estudo | x | | x | | | | | | | |
| Análise comparativa | | | | | | | | | | x |
| Análise temática | | | | | | | x | x | | |
| Resumo narrativo | x | x | x | x | x | x | x | x | x | x |

> **Nota da tradução:** a tabela segue o PDF original. Ela não coincide totalmente com o texto da Seção 3.1, que cita os estudos 2, 5, 6, 8, 9 e 10 como focados em melhores práticas; essa divergência já existe no artigo original.

### 3.2. Comparação

Uma comparação entre mapas e revisões sistemáticas já foi apresentada em (Kitchenham & Charters 2007), concentrando-se principalmente nas diferenças de abrangência e profundidade. Ampliamos essa comparação com base na visão geral das revisões sistemáticas e na experiência com a condução de mapas sistemáticos.

**Diferença nos objetivos:** ao comparar revisões e mapas sistemáticos, fica claro que seus objetivos podem ser diferentes. Como apontado em (Kitchenham & Charters 2007), uma revisão sistemática visa estabelecer o estado da evidência, embora outros objetivos, como a classificação, sejam mencionados. No entanto, as revisões sistemáticas que encontramos se concentram em identificar melhores práticas com base em evidências empíricas (é o caso da maioria das revisões sistemáticas; ver Tabela 5). Esse não é um objetivo dos mapas sistemáticos, nem pode ser, já que eles não estudam os artigos com detalhe suficiente. Em vez disso, o foco principal aqui é a classificação, a condução de análise temática e a identificação de fóruns de publicação. Ambos os tipos de estudo compartilham o objetivo de identificar lacunas de pesquisa. Em nosso mapa de variabilidade em linhas de produto, identificamos lacunas por meio de gráficos, mostrando em quais áreas de tópicos e para quais tipos de pesquisa há escassez de publicações. As revisões sistemáticas mostram onde determinada evidência está ausente ou é relatada de forma insuficiente nos estudos existentes. Isso não é possível com mapas sistemáticos.

**Diferença no processo:** vemos duas diferenças principais no processo. Nos mapas, os artigos não são avaliados quanto à sua qualidade, pois o objetivo principal não é estabelecer o estado da evidência. Em segundo lugar, os métodos de extração de dados diferem. Para o estudo de mapeamento sistemático, a análise temática é um método de análise interessante, pois ajuda a ver quais categorias estão bem cobertas em termos de número de publicações. Nas revisões sistemáticas, o método de meta-análise exige outro nível de extração de dados para trabalhar com os dados quantitativos coletados nos estudos primários (Kitchenham & Charters 2007). No entanto, não vemos razão para que vários métodos de análise diferentes não possam ser aplicados no mesmo estudo. Um resumo temático que leve a um mapa pode ser o primeiro passo de uma revisão sistemática mais detalhada. É exatamente o que estamos fazendo com base em (Mujtaba et al. 2008).

**Diferença em abrangência e profundidade:** em um estudo de mapeamento sistemático, mais artigos podem ser considerados, pois não precisam ser avaliados com tanto detalhe. Portanto, um campo maior pode ser estruturado (p. ex., toda a área de linhas de produto de software). Isso também se reflete na string de busca e nos critérios de inclusão que usamos no mapa de variabilidade em linhas de produto. Ou seja, consideramos apenas população e intervenção, introduzindo menos limitações e, potencialmente, obtendo mais resultados na busca. Por outro lado, a revisão sistemática de Kitchenham et al. (Kitchenham et al. 2007) declara o resultado e a avaliação de qualidade dos artigos como foco principal, o que aumenta a profundidade e, portanto, o esforço necessário. Isso pode exigir um foco mais específico do estudo e, consequentemente, a inclusão de menos estudos. Essa diferença também foi reconhecida em (Kitchenham & Charters 2007).

**Classificação da área de tópicos:** muitas revisões mencionaram a falta de rigor metodológico nos estudos primários; por exemplo, em (Mendes 2005), "apenas 5% dos estudos são considerados pesquisas metodologicamente rigorosas". Se restringirmos nossa amostra de artigos a uma parcela tão pequena dos artigos disponíveis, há o risco de que nossa visão geral da área de tópicos fique incompleta. É provável também que seja relativamente mais fácil fazer pesquisa empírica em algumas subáreas do que em outras. Assim, uma revisão sistemática focada em artigos que usam algum método específico pode introduzir um viés ao apresentar a área de pesquisa como um todo. Isso também é corroborado pelo fato de apenas um pequeno número de artigos potencialmente relevantes ser incluído nas revisões sistemáticas que encontramos acima.

**Classificação da abordagem de pesquisa:** em nosso mapa sistemático sobre variabilidade em linhas de produto de software, usamos categorias de nível muito alto para avaliar o tipo de artigo em termos de novidade e avaliação. Pelo argumento anterior, isso é válido, pois nenhuma avaliação detalhada dos artigos pode ser feita ao estruturar uma área grande; consequentemente, a classificação precisa ser de alto nível. Por outro lado, um esquema de classificação diferente deve ser usado em revisões sistemáticas, já que a abordagem de pesquisa empírica é avaliada com muito mais detalhe. Por isso, um estudo de revisão (Sjøberg et al. 2005) aplicou o esquema de classificação proposto por Glass et al. (Glass et al. 2002). O esquema tem um nível bastante detalhado, pois distingue mais de 22 métodos de pesquisa (como pesquisa-ação, análise conceitual, etnografia, estudo de campo etc.) e 13 abordagens de pesquisa (por exemplo, sistema descritivo, avaliativo-dedutiva, avaliativo-crítica etc.). Julgar um artigo em relação a essas categorias exige uma análise muito mais aprofundada do artigo. O grande número de categorias das revisões sistemáticas e seu nível de detalhe são particularmente visíveis nas revisões (Hannay et al. 2007, Sjøberg et al. 2005).

**Considerações de validade:** como apontado em (Mendes 2005), 73% dos artigos foram designados incorretamente, isto é, por exemplo, prometiam um experimento que não era um experimento. O mesmo problema foi relatado por (Jørgensen & Shepperd 2007), que constataram que o termo "experimento" nem sempre era usado de acordo com a definição de experimentos controlados. Consequentemente, como os artigos não são avaliados com tanto detalhe nos mapas sistemáticos, pode haver erros de julgamento ao classificá-los em categorias detalhadas. Essa ameaça é minimizada nas revisões sistemáticas, pois nelas é feita uma avaliação detalhada da metodologia de pesquisa, incluindo a extração de dados sobre a metodologia (p. ex., procedimentos de coleta de dados). Esse efeito pode ser um pouco atenuado pelo fato de os mapas sistemáticos poderem considerar mais artigos do que uma revisão (ver acima).

**Acessibilidade e relevância para a indústria:** em nossos contatos com engenheiros de software da indústria, eles frequentemente pedem artigos que ofereçam uma boa introdução a uma área específica da engenharia de software. Revisões sistemáticas poderiam ser bons artigos para recomendar a eles. Quando fizemos isso, eles muitas vezes acharam os estudos detalhados demais e de difícil acesso. Ao apresentar o mapa sistemático, foi mais fácil despertar o interesse. Acreditamos que o apelo visual dos mapas sistemáticos pode resumir os resultados e ajudar a transferi-los para os profissionais. No entanto, o foco na profundidade e nos resultados validados empiricamente que as revisões sistemáticas revelam deveria ser de maior importância para os profissionais. Assim, os autores de revisões sistemáticas deveriam pensar em formas de apresentar e estruturar seus resultados de maneira mais acessível.

## 4. Diretrizes para Mapas e Revisões Sistemáticas em Engenharia de Software

Com base na comparação acima e em nossa experiência com revisões e mapas sistemáticos, propomos as seguintes extensões às diretrizes para esses tipos de estudo.

**Use os métodos de forma complementar:** vimos que os dois métodos têm objetivos diferentes, que também podem se contradizer em parte. Por exemplo, uma boa estruturação da área de tópicos é prejudicada pela exclusão da maioria dos artigos por falta de evidência empírica. Portanto, é preciso aplicar estratégias de busca e critérios de inclusão e exclusão diferentes (como discutido anteriormente). Um mapa sistemático deve ser usado como primeiro passo em direção a uma revisão sistemática, isto é, primeiro a área de tópicos é estruturada e, em seguida, uma área de foco específica é investigada com uma revisão sistemática. No entanto, nesse contexto, é importante mencionar que um mapa sistemático sem uma revisão sistemática subsequente tem valor por si só. Ele ajuda a identificar lacunas de pesquisa em uma área de tópicos e fornece indícios da falta de pesquisa de avaliação ou de validação em certas áreas, com pouco esforço.

**Profundidade de leitura adaptativa para a classificação:** uma visão comum é que os estudos de mapeamento são frequentemente conduzidos com base apenas nos resumos. No entanto, notamos que os resumos muitas vezes são enganosos e carecem de informações importantes. Como mostrado no estudo de (Budgen et al. 2007), resumos estruturados melhoram consideravelmente a compreensibilidade; por isso, incentivamos que sejam propostos e exigidos mais amplamente na engenharia de software. Quando não estiverem disponíveis, propomos uma estratégia adaptativa para a escolha do nível de detalhe: não especifique de antemão que apenas certas partes de um artigo podem ser lidas. Em vez disso, permita um estudo mais detalhado dos artigos cuja classificação não esteja clara. Quanto mais partes de um artigo forem consideradas, maior o esforço necessário. Contudo, a validade dos resultados também aumenta. Um estudo de mapeamento que se aprofunda nos artigos pode se tornar mais parecido com uma revisão sistemática. Os dois tipos de estudo podem ser considerados pontos diferentes de um contínuo. Independentemente de em que ponto desse contínuo o estudo seja projetado, acreditamos que a abordagem mais quantitativa, comum nos estudos de mapeamento, pode complementar também as revisões sistemáticas.

**Classifique os artigos com base em evidência e novidade:** mesmo sem avaliar os métodos de pesquisa em detalhe, esquemas de classificação de alto nível ainda podem ser usados para classificar os artigos. O esquema de classificação também deve oferecer categorias para pesquisas não empíricas. Esses requisitos são bem atendidos pelo esquema de classificação apresentado por (Wieringa et al. 2006), que recomendamos para futuros mapas sistemáticos. Um refinamento futuro poderia ser dividi-lo em classes diferentes, por exemplo, com base no nível de evidência e no tipo de novidade.

**Visualize seus dados:** ao contar as frequências de publicações em categorias específicas, é possível determinar quão bem a categoria está coberta. Essas informações geralmente são resumidas em tabelas ou visualizadas com gráficos de barras. No entanto, como achamos interessante combinar diferentes categorias (p. ex., cruzar métodos de pesquisa com categorias de tópicos), o gráfico de bolhas do mapa sistemático é mais útil. Os gráficos de bolhas permitem combinar categorias entre si, de modo que a ênfase relativa da pesquisa nas categorias fica visível no próprio gráfico. Portanto, recomendamos que os pesquisadores que fazem mapas e revisões sistemáticas investiguem e utilizem formas alternativas de apresentar e visualizar seus resultados. Por exemplo, o Visualization Toolkit do Google, baseado no GapMinder<sup>2</sup>, poderia ser usado para criar gráficos de bolhas que variam ao longo do tempo, mostrando melhor as tendências de pesquisa.

## 5. Conclusão

Neste artigo, ilustramos o processo de mapeamento sistemático e o comparamos com as revisões sistemáticas. Para isso, caracterizamos e resumimos dez revisões sistemáticas existentes em engenharia de software. Nossas constatações são que os métodos de estudo diferem em termos de objetivos, abrangência e profundidade. Além disso, o uso dos métodos tem implicações diferentes para a classificação da área de tópicos e da abordagem de pesquisa. Consequentemente, ambos os métodos devem e podem ser usados de forma complementar. Um mapa sistemático pode ser conduzido primeiro, para obter uma visão geral da área de tópicos. Em seguida, o estado da evidência em tópicos específicos pode ser investigado por meio de uma revisão sistemática. Além disso, com base na comparação e em nossa experiência com mapas sistemáticos, fornecemos um conjunto de extensões às diretrizes para mapas sistemáticos. Elas enfatizam especificamente a importância de visualizar os resultados, uma técnica que deveria ser mais amplamente usada também em revisões sistemáticas.

Em trabalhos futuros, mais mapas sistemáticos devem ser conduzidos para ganhar mais experiência com o processo de mapeamento e as diretrizes que propusemos.

---

<sup>1</sup> www.splc.net
<sup>2</sup> Exemplos de como o GapMinder funciona podem ser encontrados em http://www.gapminder.com

## Referências

- Bailey, J., Budgen, D., Turner, M., Kitchenham, B., Brereton, P. & Linkman, S. (2007), Evidence relating to object-oriented software design: A survey, in 'Proc. of the 1st Int. Symp. on Empirical Software Engineering and Measurement (ESEM 2007)', pp. 482–484.
- Budgen, D., Kitchenham, B., Charters, S., Turner, M., Brereton, P. & Linjkman, S. (2007), Preliminary results of a study of the completeness and clarity of structured abstracts, in 'Proc. of the 11th Int. Conf. on Evaluation and Assessment in Software Engineering 2007', pp. 64–72.
- Davis, A. M., Tubío, Ó. D., Hickey, A. M., Juzgado, N. J. & Moreno, A. M. (2006), Effectiveness of requirements elicitation techniques: Empirical results derived from a systematic review, in 'Proc. of the 15th Int. Conf. on Requirements Engineering (RE 2006)', pp. 176–185.
- Dixon-Woods, M., Agarwal, S., Jones, D., Young, B. & Sutton, A. (2005), 'Synthesising qualitative and quantitative evidence: a review of possible methods.', Journal of Health Services Research and Policy 10(1), 45–53.
- Dybå, T., Kampenes, V. B. & Sjøberg, D. I. K. (2006), 'A systematic review of statistical power in software engineering experiments', Information & Software Technology 48(8), 745–755.
- Glass, R. L., Vessey, I. & Ramesh, V. (2002), 'Research in software engineering: an analysis of the literature', Information & Software Technology 44(8), 491–506.
- Grimstad, S., Jørgensen, M. & Moløkken-Østvold, K. (2006), 'Software effort estimation terminology: The tower of babel', Information & Software Technology 48(4), 302–310.
- Hannay, J. E., Sjøberg, D. I. K. & Dybå, T. (2007), 'A systematic review of theory use in software engineering experiments', IEEE Trans. Software Eng. 33(2), 87–107.
- Jørgensen, M. & Shepperd, M. J. (2007), 'A systematic review of software development cost estimation studies', IEEE Trans. Software Eng. 33(1), 33–53.
- Kampenes, V. B., Dybå, T., Hannay, J. E. & Sjøberg, D. I. K. (2007), 'Systematic review: A systematic review of effect size in software engineering experiments', Information & Software Technology 49(11-12), 1073–1086.
- Kitchenham, B. (2007), 'The current state of evidence-based software engineering. keynote int. conf. on evaluation and assessment in software engineering (2007)'.
- Kitchenham, B. A., Dyba, T. & Jorgensen, M. (2004), Evidence-based software engineering, in 'Proc. of the 26th Int. Conf. on Software Engineering (ICSE 2006)', IEEE Computer Society, pp. 273–281.
- Kitchenham, B. A., Mendes, E. & Travassos, G. H. (2007), 'Cross versus within-company cost estimation studies: A systematic review', IEEE Trans. Software Eng. 33(5), 316–329.
- Kitchenham, B. & Charters, S. (2007), Guidelines for performing systematic literature reviews in software engineering, Technical Report EBSE-2007-01, School of Computer Science and Mathematics, Keele University.
- MacDonell, S. G. & Shepperd, M. J. (2007), Comparing local and global software effort estimation models - reflections on a systematic review, in 'Proc. of the 1st Int. Symp. on Empirical Software Engineering and Measurement (ESEM 2007)', pp. 401–409.
- Mendes, E. (2005), A systematic review of web engineering research, in 'Proc. of the Int. Symp. on Empirical Software Engineering (ISESE 2005)', pp. 498–507.
- Mujtaba, S., Petersen, K., Feldt, R. & Mattsson, M. (2008), Software product line variability: A systematic mapping study, in 'submission'.
- Sjøberg, D. I. K., Hannay, J. E., Hansen, O., Kampenes, V. B., Karahasanovic, A., Liborg, N.-K. & Rekdal, A. C. (2005), 'A survey of controlled experiments in software engineering', IEEE Trans. Software Eng. 31(9), 733–753.
- Wieringa, R., Maiden, N. A. M., Mead, N. R. & Rolland, C. (2006), 'Requirements engineering paper classification and evaluation criteria: a proposal and a discussion', Requir. Eng. 11(1), 102–107.
