# Protocolo do Mapeamento Sistemático

**Tema:** Explicabilidade e Transparência em Agentes Baseados em LLM ao Longo do Ciclo de Vida de Desenvolvimento de Software (SDLC).

Este protocolo consolida o que está descrito na [versão preliminar do artigo](../artigo/explicabilidade-llm-sdlc-msl-preliminar.pdf) (Seção 3). O estudo segue as diretrizes de Petersen et al. (2015) para mapeamentos sistemáticos, complementadas por Kitchenham e Charters (2007) para a definição do protocolo.

## 1. Objetivo

Mapear sistematicamente as abordagens de explicabilidade e transparência aplicadas a agentes baseados em LLMs no contexto da Engenharia de Software, identificando as técnicas utilizadas, sua aplicação nas diferentes fases do SDLC e os métodos empregados para avaliar sua eficácia e utilidade para desenvolvedores.

## 2. Questões de pesquisa

- **RQ1 (Taxonomia e técnicas de XAI):** Quais são as técnicas de explicabilidade (ex.: raciocínio verbalizado/CoT, proveniência de RAG, árvores de decisão de agentes, saliência de código/tokens) mais utilizadas para tornar transparentes as decisões de agentes LLM?
- **RQ2 (Mapeamento ao longo do SDLC):** Como as abordagens de explicabilidade variam entre as diferentes fases do ciclo de vida do software (ex.: explicação da escolha de arquitetura vs. justificativa para a geração de casos de teste ou correções de código)?
- **RQ3 (Eficácia e confiança do desenvolvedor):** Qual é o impacto documentado da explicabilidade dos agentes na tomada de decisão humana, na facilidade de depuração e na mitigação do excesso de confiança (*over-reliance*) do engenheiro no código gerado?
- **RQ4 (Métricas e métodos de avaliação de XAI):** Como os estudos da literatura avaliam empiricamente a qualidade, a fidelidade e a utilidade das explicações fornecidas pelos agentes aos engenheiros de software (ex.: métricas automáticas, testes de uso com programadores, auditoria humana)?

## 3. Estratégia de busca

A string combina três grupos de termos derivados das questões de pesquisa: a tecnologia (LLMs e agentes de LLM), o atributo de interesse (explicabilidade, transparência e interpretabilidade) e o domínio (Engenharia e desenvolvimento de software). Sinônimos são unidos por `OR` e grupos, por `AND`:

```text
("large language model" OR "LLM agent" OR "LLM agents")
AND (explainability OR transparency OR interpretability)
AND ("software engineering" OR "software development")
```

A string foi aplicada a todos os campos disponíveis, sem restrição de período. Termos de técnicas específicas (ex.: *chain-of-thought*) foram omitidos para não enviesar a busca. A busca automática foi complementada por *snowballing* para trás e para frente (Wohlin, 2014) a partir dos estudos incluídos.

## 4. Fontes de busca

- IEEE Xplore
- ACM Digital Library
- Google Scholar

As duas primeiras indexam os principais veículos de Engenharia de Software; o Google Scholar abrange também preprints.

### Registro das buscas

Busca original registrada na planilha [Registro de buscas](https://docs.google.com/spreadsheets/d/1yOv2-kCNidnmWYq14np6j1VPp75qHHXb_LebeTwxjzI/edit?gid=0#gid=0):

| Data | Base | Resultados | Observações |
| --- | --- | --- | --- |
| 01/10/2026 | Google Scholar | ~17.500 | Busca exploratória; retorno muito amplo |
| 01/10/2026 | ACM Digital Library | 3.176 | Retorno amplo |
| 01/10/2026 | IEEE Xplore | 58 | Retorno mais restrito |

Como os resultados são ordenados por relevância e o volume é elevado, a triagem considerou os 8 primeiros resultados na IEEE Xplore, os 9 primeiros na ACM Digital Library e os 8 primeiros no Google Scholar (25 no total).

A coleta dos dados bibliográficos está descrita em [`estudos-primarios-coletados/`](../estudos-primarios-coletados/README.md).

## 5. Critérios de inclusão e exclusão

São incluídos os estudos que atendem a todos os critérios de inclusão e a nenhum dos critérios de exclusão.

**Critérios de inclusão**

- **CI1:** O estudo aborda LLMs ou agentes de LLMs.
- **CI2:** O LLM/agente é aplicado a uma atividade de Engenharia de Software ou etapa do SDLC, como requisitos, testes, arquitetura, codificação, DevOps ou manutenção.
- **CI3:** O estudo aborda algum mecanismo de explicabilidade, transparência, interpretabilidade, rastreabilidade ou proveniência relacionado ao comportamento/resultado do LLM ou agente.
- **CI4:** O estudo apresenta informação suficiente para responder a pelo menos uma das RQs do mapeamento.
- **CI5:** O texto completo está disponível para análise.
- **CI6:** O estudo está escrito em inglês ou português.

**Critérios de exclusão**

- **CE1:** Estudo duplicado entre as bases.
- **CE2:** Utiliza LLM, mas fora do contexto de Engenharia de Software.
- **CE3:** Trata de Engenharia de Software e LLM, mas não aborda explicabilidade/transparência.
- **CE4:** Trata de XAI/explicabilidade, mas não envolve LLMs ou agentes baseados em LLMs.
- **CE5:** O LLM é usado apenas como instrumento auxiliar da pesquisa, sem que sua explicabilidade/transparência seja objeto do estudo.
- **CE6:** Discute requisitos de explicabilidade de outros sistemas de IA, sem investigar a explicabilidade/transparência do LLM/agente atuando no SDLC.
- **CE7:** Não possui texto completo acessível ou não apresenta informações suficientes para análise.

## 6. Processo de seleção

1. Reunião dos resultados e remoção de duplicados (CE1).
2. Aplicação dos critérios a título, resumo e palavras-chave; casos duvidosos seguem para a etapa seguinte.
3. Leitura completa e reaplicação dos critérios, com atenção a CE5 e CE6, que distinguem os estudos em que a explicabilidade do LLM é objeto de investigação daqueles em que o LLM é apenas instrumento.
4. *Snowballing* a partir dos estudos incluídos.

Divergências entre os pesquisadores são discutidas até o consenso. Os estudos levantados e classificados estão na planilha [Estudos - Mapeamento Sistemático](https://docs.google.com/spreadsheets/d/1H6Rxr1Q_WzX-FOXynGSWa4hc7c1hJ9rNmwAt9qBS99Q/edit?gid=0#gid=0).

## 7. Extração e classificação dos dados

O formulário de extração registra, para cada estudo:

- identificação (autores, ano, veículo);
- nível de autonomia (assistente ou agente);
- técnica de explicabilidade (RQ1);
- fase do SDLC (RQ2);
- efeitos sobre confiança, decisão, depuração e excesso de confiança (RQ3);
- método de avaliação, com métricas e número de participantes (RQ4).

As técnicas foram classificadas por codificação aberta seguida de agrupamento, partindo dos exemplos citados na RQ1, em cinco categorias (cada estudo é associado à técnica predominante):

| Código | Categoria |
| --- | --- |
| T1 | Justificativa em linguagem natural (raciocínio verbalizado, CoT ou explicação textual da saída) |
| T2 | Atribuição pós-hoc (importância de *tokens*, trechos ou características da entrada) |
| T3 | Sinalização de incerteza e confiança |
| T4 | Rastreamento de trajetórias do agente |
| T5 | Elicitação de necessidades de explicação |

As fases do SDLC seguem Hou et al. (2024), acrescidas de revisão de código e operação.

## 8. Referências do protocolo

- Hou, X. et al. (2024). Large language models for software engineering: A systematic literature review. *ACM TOSEM*, 33(8).
- Kitchenham, B. e Charters, S. (2007). *Guidelines for performing systematic literature reviews in software engineering*. EBSE-2007-01.
- Petersen, K., Vakkalanka, S. e Kuzniarz, L. (2015). Guidelines for conducting systematic mapping studies in software engineering: An update. *Information and Software Technology*, 64:1–18.
- Wohlin, C. (2014). Guidelines for snowballing in systematic literature studies and a replication in software engineering. *EASE*. ACM.
