# Medidas DAX e Indicadores de Desempenho

## 1. Contextualização

A linguagem DAX (Data Analysis Expressions) foi utilizada para desenvolver indicadores relacionados ao monitoramento de análises laboratoriais, conformidade, liberação de produtos e acompanhamento de volumes de produção.

As medidas foram organizadas em oito grupos, considerando as particularidades das bases de dados e as regras de negócio de cada processo.

## 2. Organização das medidas

A estrutura foi segmentada em grupos de medidas para facilitar a identificação, manutenção e utilização dos cálculos.

| Grupo | Aplicação |
|---|---|
| Mercado A | Indicadores analíticos, volumétricos e laboratoriais |
| Análises gerais | Indicadores de conformidade e resultados microbiológicos |
| Mercado B | Indicadores de liberação e pendências |
| Mercado C | Indicadores analíticos e acompanhamento de produção |
| Monitoramento normativo | Indicadores de presença, ausência e status |
| Requisitos específicos | Indicadores de conformidade, produção e destinação |
| Mercado D | Indicadores quantitativos e volumétricos |
| Mercado E | Indicadores de liberação, redestinação e volume |

A segmentação das medidas está relacionada à heterogeneidade das fontes de dados e às particularidades dos processos monitorados.

## 3. Indicadores de conformidade

Foram desenvolvidas medidas para acompanhamento dos resultados analíticos:

- Quantidade de resultados conformes.
- Quantidade de resultados não conformes.
- Total de resultados conformes e não conformes.
- Percentual de conformidade.
- Percentual de não conformidade.
- Quantidade de resultados vazios.

Esses indicadores auxiliam na identificação de desvios e no acompanhamento dos padrões de qualidade.

## 4. Indicadores microbiológicos

O modelo contempla medidas específicas para monitoramento de resultados microbiológicos:

- Quantidade de resultados com presença.
- Quantidade de resultados com ausência.
- Percentual de presença.
- Percentual de ausência.
- Percentual de presença de Salmonella.

Os indicadores são segmentados conforme as bases e os processos analíticos correspondentes.

## 5. Indicadores de liberação

Foram desenvolvidas medidas para acompanhamento das diferentes condições de liberação e destinação:

- Quantidade de amostras liberadas.
- Quantidade de amostras pendentes.
- Quantidade de amostras redestinadas.
- Quantidade de registros em análise.
- Percentual de amostras liberadas.
- Percentual de amostras pendentes.
- Percentual de amostras redestinadas.
- Percentual de pendências por análise.

Essas medidas possibilitam acompanhar a situação dos registros e identificar pendências nos processos de liberação.

## 6. Indicadores volumétricos e de produção

Além do acompanhamento quantitativo das análises, foram desenvolvidas medidas relacionadas aos volumes de produção.

| Indicador | Finalidade |
|---|---|
| Volume total | Acompanhamento do volume registrado |
| Produção total | Consolidação da produção |
| Volume liberado | Acompanhamento dos volumes liberados |
| Volume pendente | Identificação dos volumes com pendências |
| Volume redestinado | Acompanhamento das alterações de destinação |
| Volume por status | Distribuição dos volumes conforme classificação |
| Percentual de produção liberada | Acompanhamento proporcional das liberações |
| Percentual de produção pendente | Acompanhamento proporcional das pendências |
| Percentual de produção redestinada | Acompanhamento proporcional das redestinações |
| Percentual de produção em análise | Monitoramento proporcional da produção em análise |

A separação entre indicadores quantitativos e volumétricos permite avaliar tanto a quantidade de registros quanto os volumes associados aos processos monitorados.

## 7. Indicadores temporais

O modelo contempla medidas e colunas calculadas relacionadas ao acompanhamento da permanência em laboratório.

- Média de dias no laboratório.
- Dias no laboratório.
- Faixas de permanência.

Esses recursos auxiliam no acompanhamento temporal dos processos e na identificação de períodos prolongados de permanência.

## 8. Medidas auxiliares de visualização

Também foram desenvolvidas medidas destinadas ao suporte das visualizações:

- Medidas de apresentação de volumes em formato textual.
- Medidas específicas para cartões de indicadores.
- Medidas auxiliares de exibição de registros.

Esses recursos complementam os indicadores principais e atendem às necessidades de apresentação dos dashboards.

## 9. Classificação por status

O modelo utiliza dimensões de status compartilhadas e específicas para atender às particularidades dos processos.

Entre as condições monitoradas estão:

- Liberado.
- Pendente.
- Redestinado.
- Em análise.
- Conforme.
- Não conforme.
- Presença.
- Ausência.

As classificações possuem aplicações distintas, podendo representar resultados analíticos, situações de liberação ou condições de destinação.

## 10. Integração com o modelo relacional

As medidas utilizam a estrutura relacional desenvolvida no projeto, considerando as dimensões disponíveis para cada processo.

Entre os principais contextos de análise estão:

- Período.
- Produto.
- Tipo de análise.
- Mercado de destino.
- Status.
- Resultado analítico.

A documentação dos relacionamentos está disponível em [Modelagem e Arquitetura de Dados](modelagem.md).

## 11. Decisões técnicas

A utilização de grupos específicos de medidas está relacionada às diferenças estruturais entre as fontes de dados.

Embora determinados indicadores possuam finalidades semelhantes, suas implementações precisam considerar as tabelas, identificadores e classificações disponíveis em cada processo.

A estrutura atual permite preservar essas particularidades, mas também apresenta oportunidades de reutilização e padronização dos cálculos.

## 12. Oportunidades de melhoria

- Avaliação da possibilidade de consolidação de medidas semelhantes.
- Padronização das nomenclaturas.
- Organização das medidas em pastas de exibição.
- Documentação das dependências entre cálculos.
- Revisão dos critérios utilizados nos denominadores dos indicadores percentuais.
- Validação do comportamento dos cálculos em diferentes contextos de filtro.
- Avaliação da utilização de grupos de cálculo, quando aplicável.

## 13. Competências técnicas aplicadas

- Desenvolvimento de indicadores utilizando DAX.
- Criação de medidas quantitativas e percentuais.
- Desenvolvimento de indicadores volumétricos.
- Monitoramento de resultados microbiológicos.
- Análise de conformidade.
- Classificação de informações.
- Desenvolvimento de indicadores temporais.
- Organização de medidas por processo.
- Integração de indicadores com modelos relacionais.

## 14. Confidencialidade

A documentação apresenta a estrutura conceitual dos indicadores desenvolvidos, utilizando nomenclaturas generalizadas para preservar informações corporativas.

---

**Autora:** Anne Caroline Marquez Bragante

**Área:** Business Intelligence, Data Analytics e Gestão da Qualidade
