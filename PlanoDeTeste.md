# Plano de Testes da Situação de Aprendizagem - 4° Semestre
### Gabriel Abel da Silva, Bruno Silva, Leonardo da Rosa e Nicolas.

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


# 6. Funcionalidades a Serem Testadas

 ### F001: Cadastro de Colaboradores

Descrição: Funcionalidade para registro de novos colaboradores.

Prioridade: Alta

F002: Devolução de EPIs

Descrição: Funcionalidade que registra a devolução dos EPIs pelos colaboradores.

Prioridade: Alta

### 7. Funcionalidades que Não Serão Testadas

   NF001: Funcionalidade de Exportação de Dados

   Motivo: Não é parte do escopo inicial.


# 9. Critérios de Aprovação/Reprovação de Item
## 9.1 Critérios de Aprovação
Para que um item de teste seja aprovado, ele deve atender a todos os seguintes critérios:

Cumprimento dos Requisitos: O item deve satisfazer todos os requisitos funcionais e não funcionais definidos na especificação de requisitos. Ausência de Defeitos Críticos: O item deve estar livre de defeitos críticos que impeçam a sua funcionalidade principal. Resultados dos Testes: O item deve passar com sucesso em todos os casos de teste relevantes, sem apresentar falhas em funcionalidades essenciais. Performance e Confiabilidade: O desempenho do item deve estar dentro dos limites aceitáveis e ele deve demonstrar confiabilidade em cenários de uso prolongado. Conformidade com Padrões: O item deve estar em conformidade com as normas e padrões de qualidade definidos, como segurança, acessibilidade, e desempenho.

## 9.2 Critérios de Reprovação
Um item de teste será reprovado se qualquer um dos seguintes cenários ocorrer:

Falha nos Testes: O item não passou em um ou mais casos de teste importantes, especialmente aqueles relacionados à sua funcionalidade crítica. Defeitos Críticos ou Bloqueadores: A presença de defeitos que comprometem o funcionamento do sistema de forma crítica ou bloqueiam o uso da funcionalidade. Desempenho Insatisfatório: O item apresenta desempenho fora dos padrões estabelecidos ou falha em atender aos requisitos de tempo de resposta e estabilidade. Inconsistências com os Requisitos: O item não cumpre os requisitos especificados, incluindo funcionalidades principais e requisitos de segurança ou de usabilidade. Não-Conformidade com Padrões: O item não está em conformidade com as normas e padrões de qualidade exigidos para o projeto.