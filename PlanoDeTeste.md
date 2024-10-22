# Plano de Testes da Situação de Aprendizagem - 4° Semestre
### Gabriel Abel da Silva, Bruno Silva, Leonardo da Rosa e Nicolas.


# 1. Identificador do Plano de Teste

### Identificador: [TPT-2024-002]
1. Identificador do Plano de Teste

Identificador: [TPT-2024-002]

TPT: Plano de Teste

2024: Ano atual

### 002: Número sequencial do plano

002: Número sequencial do plano

Versão: [1.2]

1: Versão principal

2: Revisão menor

# 3. Introdução

#### 3.1 Objetivo do Documento

Este documento tem como objetivo definir a estratégia, os procedimentos e os critérios para a execução dos testes do sistema de gestão de EPIs.
O plano detalha os testes a serem realizados para garantir que o sistema atenda aos requisitos funcionais e não-funcionais estabelecidos,
assegurando sua qualidade e confiabilidade antes de sua implantação.

#### 3.2 Escopo do Projeto

O sistema de gestão de EPIs tem como propósito centralizar o controle e o acompanhamento de todos os equipamentos de proteção individual utilizados pela empresa.
O sistema abrangerá as seguintes funcionalidades:

* **Cadastro de EPIs:** Registro detalhado de cada tipo de EPI, incluindo suas características técnicas, fornecedor, data de validade, etc.
* **Gerenciamento de Estoque:** Controle dos níveis de estoque de cada EPI, incluindo entradas, saídas e movimentações internas.
* **Atribuição de EPIs:** Vinculação de EPIs aos colaboradores, considerando suas funções e riscos associados.
* **Geração de Relatórios:** Criação de relatórios personalizados para acompanhar o uso, a manutenção e a necessidade de reposição dos EPIs.
* **Notificações:** Emissão de alertas para datas de validade próximas, necessidade de manutenção ou falta de estoque de determinados EPIs.

#### 3.3 Público-Alvo

Este documento é direcionado aos seguintes públicos:

* **Equipe de Desenvolvimento:** Para que compreendam os critérios de aceitação e as atividades de teste a serem realizadas.
* **Equipe de Qualidade:** Para que planejem e executem os testes de acordo com as especificações.
* **Gerenciamento do Projeto:** Para acompanhar o progresso dos testes e tomar decisões baseadas nos resultados.
* **Usuários Finais:** Para que tenham conhecimento das funcionalidades do sistema e de seus níveis de qualidade.

#### 3.4 Convenções do Documento

Este documento segue algumas convenções de formatação e nomenclatura para garantir clareza, consistência e fácil compreensão. A seguir estão as principais convenções adotadas:

* Estrutura de Títulos e Subtítulos:
Os títulos de seções e subseções seguem uma numeração hierárquica, com títulos de seção numerados como "3", "3.1", "3.2", etc. Eles são formatados em negrito para destacá-los.

* Negrito:
É utilizado para destacar termos importantes, como nomes de funcionalidades ou títulos de seções. Exemplo: Cadastro de EPIs, Gerenciamento de Estoque.

* Itálico:
Utilizado para destacar termos técnicos, siglas, ou componentes específicos do sistema, como EPI (Equipamento de Proteção Individual) ou SGE (Sistema de Gestão de EPIs).

* Listas Numeradas e com Marcadores:

Listas numeradas são usadas quando a ordem de execução ou priorização dos itens é relevante. Exemplo:
Cadastro de EPIs
Atribuição de EPIs
Listas com marcadores são usadas para descrever funcionalidades ou itens sem uma ordem específica. Exemplo:
Geração de Relatórios
Notificações de validade
Abreviações e Siglas:
As siglas e abreviações são descritas por extenso na primeira vez que aparecem no documento, seguidas pela sigla entre parênteses. Exemplo: Equipamento de Proteção Individual (EPI).

* Cores e Destaques Visuais:
Caso haja a necessidade de destacar algum texto de maneira visual, serão utilizados elementos como caixas de alerta, ícones de nota ou cor de fundo para enfatizar informações adicionais ou críticas.

* Referências a Documentos Externos:
Quando houver menções a outros documentos ou normas, será usado o formato de citação direta, entre colchetes. Exemplo: [ISO 45001] ou [Manual de Procedimentos Internos].

* Notas e Observações:
Notas ou observações relevantes serão destacadas com um ícone de alerta ou símbolo de nota, geralmente em uma caixa de texto em itálico, para indicar informações adicionais, advertências ou recomendações.


# 6. Funcionalidades a Serem Testadas

 ### F001: Cadastro de Colaboradores

6. Funcionalidades a Serem Testadas

F001: Cadastro de Colaboradores

Descrição: Funcionalidade para registro de novos colaboradores.

Prioridade: Alta

F002: Devolução de EPIs

Descrição: Funcionalidade que registra a devolução dos EPIs pelos colaboradores.

Prioridade: Alta


### 7. Funcionalidades que Não Serão Testadas

7. Funcionalidades que Não Serão Testadas

   NF001: Funcionalidade de Exportação de Dados

   Motivo: Não é parte do escopo inicial.



# 9. Critérios de Aprovação/Reprovação de Item
## 9.1 Critérios de Aprovação
Para que um item de teste seja aprovado, ele deve atender a todos os seguintes critérios:

Cumprimento dos Requisitos: O item deve satisfazer todos os requisitos funcionais e não funcionais definidos na especificação de requisitos. Ausência de Defeitos Críticos: O item deve estar livre de defeitos críticos que impeçam a sua funcionalidade principal. Resultados dos Testes: O item deve passar com sucesso em todos os casos de teste relevantes, sem apresentar falhas em funcionalidades essenciais. Performance e Confiabilidade: O desempenho do item deve estar dentro dos limites aceitáveis e ele deve demonstrar confiabilidade em cenários de uso prolongado. Conformidade com Padrões: O item deve estar em conformidade com as normas e padrões de qualidade definidos, como segurança, acessibilidade, e desempenho.

## 9.2 Critérios de Reprovação
Um item de teste será reprovado se qualquer um dos seguintes cenários ocorrer:

Falha nos Testes: O item não passou em um ou mais casos de teste importantes, especialmente aqueles relacionados à sua funcionalidade crítica. Defeitos Críticos ou Bloqueadores: A presença de defeitos que comprometem o funcionamento do sistema de forma crítica ou bloqueiam o uso da funcionalidade. Desempenho Insatisfatório: O item apresenta desempenho fora dos padrões estabelecidos ou falha em atender aos requisitos de tempo de resposta e estabilidade. Inconsistências com os Requisitos: O item não cumpre os requisitos especificados, incluindo funcionalidades principais e requisitos de segurança ou de usabilidade. Não-Conformidade com Padrões: O item não está em conformidade com as normas e padrões de qualidade exigidos para o projeto.

# 11. Entregáveis de Teste
    Os entregáveis de teste são documentos e relatórios que fornecem evidências das atividades de teste realizadas durante o ciclo de desenvolvimento. Eles são fundamentais para assegurar que os requisitos e objetivos dos testes foram cumpridos.

## 11.1 Plano de Teste
Documento que descreve detalhadamente o escopo, a abordagem, os recursos e o cronograma das atividades de teste. O Plano de Teste também inclui critérios de entrada e saída, além dos riscos identificados e estratégias de mitigação.

## 11.2 Especificações de Caso de Teste
Esses documentos contêm as descrições dos casos de teste que serão executados. Cada especificação de caso de teste inclui as condições iniciais, os passos de execução, os resultados esperados e os critérios de aceitação.

## 11.3 Conjuntos de Dados de Teste
Os dados de teste são conjuntos de informações ou parâmetros que serão usados durante a execução dos casos de teste. Esses conjuntos são preparados para garantir que os testes sejam representativos das condições reais de uso do sistema.

## 11.4 Relatórios de Execução de Teste
Esses relatórios documentam os resultados de cada execução de teste, destacando os casos que foram bem-sucedidos, os que falharam e quaisquer anomalias encontradas. Eles incluem informações como o número de casos de teste executados, status dos testes (aprovados/reprovados) e métricas de desempenho.

## 11.5 Relatórios de Incidentes
Relatórios de incidentes detalham as falhas ou defeitos encontrados durante os testes. Cada relatório contém uma descrição do incidente, o impacto no sistema, a probabilidade de ocorrência e as recomendações para correção.

## 11.6 Relatório de Resumo de Teste
Este documento resume as atividades de teste realizadas e os principais resultados obtidos. Ele fornece uma visão geral de todo o processo de teste, incluindo métricas de sucesso e falha, uma análise dos riscos mitigados e recomendações para melhorias futuras.
