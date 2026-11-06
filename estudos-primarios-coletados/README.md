# Estudos primários coletados

Dados bibliográficos, em formato BibTeX, de **todos os estudos retornados** pela string de busca em cada base, e não apenas dos estudos selecionados na etapa final. O protocolo está em [`protocolo/`](../protocolo/protocolo-mapeamento-sistematico.md).

```text
("large language model" OR "LLM agent" OR "LLM agents")
AND (explainability OR transparency OR interpretability)
AND ("software engineering" OR "software development")
```

## Situação da coleta

> [!WARNING]
> **Coleta incompleta.** Apenas a IEEE Xplore está completa.

| Base | Arquivo | Busca original (01/10/2026) | Retorno em 05/11/2026 | Registros no arquivo | Situação |
| --- | --- | --- | --- | --- | --- |
| IEEE Xplore | [`ieee-xplore.bib`](ieee-xplore.bib) | 58 | 64 | 64 | Completa |
| ACM Digital Library | [`acm-digital-library-PARCIAL.bib`](acm-digital-library-PARCIAL.bib) | 3.176 | 3.509 | 3.173 | **Parcial** |
| Google Scholar | — | ~17.500 | não reexecutada | 0 | **Pendente** |

## Observações metodológicas

- **Data da coleta:** os arquivos `.bib` não são da busca original de 01/10/2026, cujos resultados não foram exportados na época. A string foi reexecutada em 05/11/2026, por isso as contagens são maiores que as registradas.
- **Campos e período:** todos os campos, sem filtro de período, como definido no protocolo.
- **IEEE Xplore:** BibTeX exportado pela própria base, com resumos.
- **ACM Digital Library:** para contornar o limite de navegação por busca, os resultados foram percorridos por ano de publicação (a soma dos anos confere com os 3.509). A base devolveu os metadados em CSL-JSON, convertidos para BibTeX.
- **Duplicatas:** nenhuma deduplicação foi aplicada dentro de cada arquivo ou entre as bases, pois ela faz parte da etapa de seleção (CE1).

### O que falta na ACM

A coleta foi interrompida duas vezes por uma verificação de segurança da base (HTTP 403); a segunda interrupção encerrou a coleta em 2026, na página 28.

| Ano de publicação | Retornados | Percorridos |
| --- | --- | --- |
| até 2022 | 19 | 19 |
| 2023 | 195 | 195 |
| 2024 | 740 | 740 |
| 2025 | 857 | 857 |
| 2026 | 1.698 | 1.400 |
| **Total** | **3.509** | **3.211** |

Falta percorrer 298 resultados de 2026. Os 3.211 resultados percorridos geraram 3.173 registros únicos: 38 DOIs reapareceram em páginas diferentes, então o total de registros pode continuar abaixo de 3.509 mesmo após percorrer o restante. O ano do filtro é o da publicação eletrônica e pode diferir do ano no campo `year`. Dos 3.173 registros, 586 vieram sem resumo.
