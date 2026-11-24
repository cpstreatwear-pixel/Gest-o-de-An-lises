# Regras de Negócio — Gestão de Análises e Liberações

## 1. Objetivo

O projeto foi desenvolvido para centralizar o acompanhamento das análises laboratoriais, dos resultados analíticos e das condições de liberação dos produtos, relacionando informações de qualidade aos volumes de produção.

## 2. Segmentação dos processos

O monitoramento considera diferentes mercados de destino, requisitos específicos e processos analíticos.

Cada processo possui particularidades relacionadas a:

- Identificação dos produtos.
- Tipos de análises.
- Classificação dos resultados.
- Critérios de liberação.
- Condições de destinação.
- Estrutura das informações.

Essas diferenças são consideradas individualmente na modelagem e no desenvolvimento dos indicadores.

## 3. Classificação dos resultados analíticos

| Classificação | Descrição |
|---|---|
| Conforme | Resultado classificado como atendendo aos critérios aplicáveis |
| Não conforme | Resultado classificado como não atendendo aos critérios aplicáveis |
| Presença | Identificação de presença no resultado microbiológico |
| Ausência | Identificação de ausência no resultado microbiológico |
| Vazio | Registro sem resultado preenchido |

As classificações são utilizadas conforme o tipo de análise e as regras aplicáveis a cada processo.

Resultados ausentes não devem ser interpretados automaticamente como conformes.

## 4. Status de liberação e destinação

| Status | Descrição |
|---|---|
| Liberado | Produto ou registro classificado como liberado |
| Pendente | Produto ou registro com pendências no processo |
| Redestinado | Produto direcionado para outra destinação |
| Em análise | Registro classificado como estando em processo de análise |

O modelo utiliza dimensões específicas de status para preservar as particularidades de cada processo.

## 5. Monitoramento quantitativo e volumétrico

O projeto contempla duas perspectivas complementares:

### Monitoramento quantitativo

- Quantidade de amostras.
- Quantidade de resultados analíticos.
- Quantidade de conformidades e não conformidades.
- Quantidade de liberações e pendências.
- Quantidade de redestinações.

### Monitoramento volumétrico

- Volume total de produção.
- Volume liberado.
- Volume pendente.
- Volume redestinado.
- Distribuição percentual dos volumes por status.

A separação dessas perspectivas permite acompanhar tanto a quantidade de ocorrências quanto o impacto associado aos volumes de produção.

## 6. Monitoramento temporal

O acompanhamento temporal considera as datas disponíveis em cada processo, incluindo datas de produção, coleta e recebimento.

O modelo também contempla indicadores relacionados à permanência em laboratório, permitindo analisar:

- Dias de permanência.
- Média de dias no laboratório.
- Faixas de permanência.
- Evolução histórica dos indicadores.

## 7. Integridade das informações

A confiabilidade dos indicadores depende da manutenção das bases de dados e dos cadastros utilizados no modelo.

São considerados pontos críticos:

- Preenchimento correto das informações.
- Atualização dos cadastros de produtos.
- Consistência dos códigos de identificação.
- Padronização dos resultados analíticos.
- Classificação adequada dos status.
- Integridade dos campos de data.
- Atualização recorrente das fontes.

## 8. Aplicação gerencial

Os indicadores desenvolvidos permitem apoiar:

- Acompanhamento das condições de liberação.
- Identificação de pendências laboratoriais.
- Monitoramento de não conformidades.
- Avaliação dos volumes associados aos diferentes status.
- Análise histórica dos processos.
- Identificação de oportunidades de melhoria.

O dashboard constitui uma ferramenta de acompanhamento e suporte à tomada de decisão, não substituindo os procedimentos oficiais de avaliação e liberação de produtos.

## 9. Confidencialidade

As regras apresentadas representam conceitualmente os processos monitorados pelo projeto.

Critérios internos de liberação, limites analíticos, requisitos comerciais e procedimentos corporativos específicos não são disponibilizados nesta documentação.

---

**Autora:** Anne Caroline Marquez Bragante

**Área:** Business Intelligence, Data Analytics e Gestão da Qualidade  
