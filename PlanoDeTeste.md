# Plano de Testes da Situação de Aprendizagem - 4° Semestre
### Gabriel Abel da Silva, Bruno Silva, Leonardo da Rosa e Nicolas.

# 1. Identificador do Plano de Teste

### Identificador: [TPT-2024-002]

TPT: Plano de Teste

2024: Ano atual

### 002: Número sequencial do plano

Versão: [1.2]

1: Versão principal

2: Revisão menor

# 3. Introdução

### 3.1 Objetivo do Documento
Este plano de testes visa garantir que o sistema de gerenciamento de Equipamentos de Proteção Individual (EPIs) atenda aos requisitos funcionais e de segurança exigidos pela empresa. Seguindo o padrão IEEE 829, documentaremos todos os procedimentos de teste para assegurar que os colaboradores utilizem os EPIs conforme as normas, promovendo um ambiente de trabalho seguro.

### 3.2 Escopo do Projeto
O escopo abrange o sistema de controle de EPIs, incluindo cadastro, empréstimo, devolução e gerenciamento de estoque. Testes de interface e funcionalidade são aplicados para validar operações críticas, como autenticação, controle de estoque e rastreamento de devoluções.

### 3.3 Público-Alvo
Este documento destina-se à equipe de desenvolvimento, testadores e stakeholders, com foco em garantir que todos compreendam os objetivos e métodos de teste utilizados para validar o sistema de controle de EPIs.

### 3.4 Convenções do Documento

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

Descrição: Funcionalidade para registro de novos colaboradores.

Prioridade: Alta

F002: Devolução de EPIs

Descrição: Funcionalidade que registra a devolução dos EPIs pelos colaboradores.

Prioridade: Alta

# 7. Funcionalidades que Não Serão Testadas

   NF001: Funcionalidade de Exportação de Dados

   Motivo: Não é parte do escopo inicial.

#  8. Abordagem (Estratégia)
### 8.1 Tipos de Teste
Teste Unitário
Teste de Integração
Teste de Sistema
Teste de Aceitação do Usuário (UAT)
### 8.2 Ferramentas de Teste
Ferramenta	Versão	Propósito
JUnit	5.8	Testes unitários
Selenium	4.0	Testes de integração
### 8.3 Critérios de Entrada e Saída

### Critérios de Entrada:
Todos os requisitos devem estar documentados e aprovados.

### Critérios de Saída:
Todos os testes devem ser executados e documentados com resultados satisfatórios.

# 9. Critérios de Aprovação/Reprovação de Item
### 9.1 Critérios de Aprovação
Para aprovação, o item de teste deve:

Atender aos requisitos funcionais e de segurança de EPI.
Passar em testes de autenticação e verificação de estoque sem erros.
Ter seu desempenho avaliado e aprovado em situações reais de uso.
Conformidade com normas de segurança e confiabilidade no controle de EPIs.
### 9.2 Critérios de Reprovação
Um item será reprovado se:

Falhar nos testes de funcionalidade crítica (ex. controle de estoque).
Apresentar defeitos que comprometam a segurança ou rastreamento de EPIs.
Não atender às normas de controle de EPI e segurança estabelecidas.
Apresentar inconsistências de desempenho ou falha no controle de acesso.

# 11. Entregáveis de Teste
    Os entregáveis de teste são documentos e relatórios que fornecem evidências das atividades de teste realizadas durante o ciclo de desenvolvimento. Eles são fundamentais para assegurar que os requisitos e objetivos dos testes foram cumpridos.

### 11.1 Plano de Teste
Documento com o planejamento detalhado para teste de todas as funcionalidades do sistema de gerenciamento de EPIs.

### 11.2 Especificações de Caso de Teste
Descreve os passos e resultados esperados para cada caso de teste específico, garantindo a validação de funcionalidades críticas, como controle de estoque e cadastro de equipamentos.

### 11.3 Conjuntos de Dados de Teste
Dados específicos para simular condições reais de uso, como diferentes estados de estoque e combinações de equipamentos e colaboradores.

### 11.4 Relatórios de Execução de Teste
Relatórios que documentam os resultados de cada execução, com detalhes sobre casos aprovados e reprovados.

### 11.5 Relatórios de Incidentes
Relatórios sobre falhas identificadas, incluindo descrição, impacto e solução proposta.

### 11.6 Relatório de Resumo de Teste
Sumário final de todos os testes executados, destacando métricas de sucesso e falha e recomendações.

# 15. Responsabilidades

|Função|Responsável|Responsabilidades|
|:---|:---:|---:|
|Gerente de Teste|Nome do Gerente|Planejamento e coordenação das atividades de teste, supervisão da equipe, conformidade com o plano e aprovação final.|
|Testadores|Nome dos Testadores|Execução dos casos de teste, identificação de incidentes, verificação de funcionalidades e validação de segurança.|
|Analistas de Qualidade|Nome dos Analistas|Revisão dos entregáveis, validação de requisitos de segurança e funcionalidade, e garantia de conformidade.|

# 16. Cronograma

|Fase         |Data de Início|Data de Término|Duração|
|:------------|:------------:|:-------------:|------:|
|Planejamento |DD/MM/AAAA    |DD/MM/AAAA     |X dias |
|Preparação   |DD/MM/AAAA    |DD/MM/AAAA     |X dias |
|Execução     |DD/MM/AAAA    |DD/MM/AAAA     |X dias |
|Avaliação    |DD/MM/AAAA    |DD/MM/AAAA     |X dias |

# 18. Aprovações

|Função                |Nome              |Assinatura          |Data       |
|:---------------------|:----------------:|:-------------------:|----------:|
|Gerente de Projeto    |Nome do Gerente   |____________________|DD/MM/AAAA |
|Gerente de QA         |Nome do Gerente QA|____________________|DD/MM/AAAA |
|Cliente/Stakeholder   |Nome do Cliente   |____________________|DD/MM/AAAA |
