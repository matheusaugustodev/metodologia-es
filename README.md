# Tema: Explicabilidade e Transparência em Agentes Baseados em LLM ao Longo do Ciclo de Vida de Desenvolvimento de Software (SDLC): Um Mapeamento Sistemática da Literatura

## Estudantes

- DAVI DUARTE NECO (Matrícula: 202302601)
- JORDANE GABRIELLA SOARES DE OLIVEIRA PIRES (Matrícula: 201711014)
- MATHEUS AUGUSTO FERREIRA MEDEIROS (Matrícula: 202305532)
- MATHEUS VIEIRA MENDES PACHECO (Matrícula: 202302623)

## Documento de Trabalho

A estruturação do artigo está sendo feita no Google Docs: [Documento do artigo](https://docs.google.com/document/d/1wim1Iciu9yBbUmtnl1ZOr3PVLI1eRTKtHvNAkMdhMS4/edit?tab=t.0)

## Escopo do Estudo

Mapeamento e consolidação sistemática das técnicas de Inteligência Artificial Explicável (XAI) e mecanismos de transparência (ex.: *chain-of-thought rationale*, grafos de raciocínio, atribuição de atenção, rastreamento de proveniência de contexto e inspecção de estados internos) aplicados a agentes autônomos e semi-autônomos baseados em LLMs.

O estudo investiga como a explicabilidade é implementada e adaptada nas diferentes etapas da Engenharia de Software (Engenharia de Requisitos, Arquitetura, Codificação, Testes, DevOps e Manutenção), avaliando o impacto da transparência na confiança dos engenheiros, na facilidade de auditoria e na detecção de erros de raciocínio (*hallucinations*).

## Perguntas de Pesquisa (RQs)

### RQ1: Taxonomia e Técnicas de XAI

Quais são as técnicas de explicabilidade (ex.: raciocínio verbalizado/CoT, *provenance* de RAG, árvores de decisão de agentes, saliência de código/tokens) mais utilizadas para tornar transparente as decisões de agentes LLM?

### RQ2: Mapeamento ao Longo do SDLC

Como as abordagens de explicabilidade variam entre as diferentes fases do ciclo de vida do software (e.g., explicação de escolha de arquitetura vs. justificativa para geração de casos de teste ou correções de código)?

### RQ3: Eficácia e Confiança do Desenvolvedor

Qual é o impacto documentado da explicabilidade dos agentes na tomada de decisão humana, na facilidade de *debugging* e na mitigação do excesso de confiança (*over-reliance*) do engenheiro no código gerado?

### RQ4: Métricas e Métodos de Avaliação de XAI

Como os estudos da literatura avaliam empiricamente a qualidade, fidelidade e utilidade das explicações fornecidas pelos agentes aos engenheiros de software (ex.: métricas automáticas, testes de uso com programadores, auditoria humana)?
