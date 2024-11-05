# Plano de Testes da Situação de Aprendizagem - 4° Semestre
### Gabriel Abel da Silva, Bruno Silva, Leonardo da Rosa e Nicolas.

## 1. Identificador do Plano de Teste
- **Identificador**: TPT-2024-001
    - **TPT**: Template de Plano de Teste
    - **2024**: Ano atual
    - **001**: Número sequencial do plano

## 2. Referências
|Documento                       |Versão|Descrição                                                 |Localização                                                                 |
|:-------------------------------|:----:|----------------------------------------------------------|---------------------------------------------------------------------------:|
|Especificação de Requisitos     |1.2   |Documento com todos os requisitos funcionais e não funcionais|/documentos/requisitos_v1_2.pdf                                           |
|IEEE 829 Standard for Software Test Documentation |2008 |Padrão IEEE 829 para documentação de testes de software|[Link para IEEE 829](https://standards.ieee.org/standard/829-2008.html) |


## 3. Introdução
### 3.1 Objetivo do Documento
Este documento define o plano de testes para o sistema de gerenciamento de EPIs, assegurando a conformidade com as normas de segurança e usabilidade, conforme o padrão IEEE 829.

### 3.2 Escopo do Projeto
O projeto abrange as funcionalidades de cadastro, empréstimo, devolução e controle de estoque de EPIs, visando garantir segurança no ambiente de trabalho e facilidade de uso.

### 3.3 Público-Alvo
Este documento destina-se à equipe de desenvolvimento, analistas de QA, gerentes de projeto e stakeholders.

### 3.4 Convenções do Documento
- Identificadores específicos para cada caso de teste.
- Formato de versão X.Y para controle de revisões.
- Documentação de incidentes e relatórios em conformidade com a estrutura IEEE 829.

## 4. Itens de Teste (Funções)
|ID     |Item de Teste                     |Descrição                                |Versão|
|:------|:----------------------------------|-----------------------------------------|-----:|
|IT001  |Cadastro de Usuários               |Permite o cadastro, consulta e exclusão de usuários do sistema |1.0   |
|IT002  |Empréstimo de EPI                  |Registro de empréstimos com controle de estoque|1.0   |
|IT003  |Devolução de EPI                   |Permite a devolução e ajuste de estoque de equipamentos |1.0   |
|IT004  |Relatórios de Uso                  |Geração de relatórios sobre uso e movimentação de EPIs |1.1   |

## 5. Questões de Risco de Software
### 5.1 Riscos Identificados
|ID     |Risco                                |Probabilidade|Impacto|Mitigação                       |
|:------|:------------------------------------|:----------:|------:|--------------------------------|
|R001   |Falha no controle de estoque         |Alta        |Alto   |Revisão periódica de estoque e auditorias|
|R002   |Inconsistência de dados no empréstimo|Média       |Alto   |Validação adicional nos registros|
|R003   |Desempenho insuficiente              |Baixa       |Médio  |Otimização do banco de dados e código|

### 5.2 Áreas de Preocupação Especial
- Controle de estoque de equipamentos.
- Registro e rastreamento de devoluções.
- Auditoria e geração de relatórios de segurança.

## 6. Funcionalidades a Serem Testadas
|ID     |Funcionalidade                   |Descrição                                       |Prioridade|
|:------|:--------------------------------|------------------------------------------------|---------:|
|F001   |Autenticação                     |Controle de acesso ao sistema                    |Alta      |
|F002   |Cadastro de Colaboradores        |Registro e consulta de colaboradores            |Alta      |
|F003   |Controle de Estoque              |Gerenciamento de estoque dos EPIs               |Média     |
|F004   |Relatórios de Segurança          |Relatórios sobre utilização e estoque de EPIs   |Baixa     |

### 6.2 Matriz de Rastreabilidade
|ID Funcionalidade|ID Requisito|ID Caso de Teste         |
|:----------------|:----------:|-------------------------:|
|F001            |REQ001      |CT001, CT002              |
|F002            |REQ002      |CT003, CT004              |
|F003            |REQ003      |CT005, CT006              |

## 7. Funcionalidades que Não Serão Testadas
|ID     |Funcionalidade                     |Motivo para Não Testar      |
|:------|:----------------------------------|----------------------------|
|NF001  |Consulta de Histórico              |Funcionalidade não prioritária no escopo atual|
|NF002  |Exportação de Dados para Excel     |Não essencial na versão inicial|

## 8. Abordagem (Estratégia)
### 8.1 Tipos de Teste
- Teste Unitário: Validação de funções individuais.
- Teste de Integração: Validação da interação entre diferentes módulos.
- Teste de Sistema: Avaliação do sistema como um todo.
- Teste de Aceitação do Usuário (UAT): Teste realizado pelos usuários finais.
- Teste de Desempenho: Teste de carga e estresse para avaliar o sistema sob uso intenso.

### 8.2 Ferramentas de Teste
|Ferramenta               |Versão|Propósito                           |
|:-------------------------|:----:|-----------------------------------:|
|Selenium                  |4.0   |Automatizar testes de interface web|
|JMeter                    |5.4   |Teste de carga e estresse          |
|Postman                   |9.1   |Teste de API                       |

### 8.3 Critérios de Entrada e Saída
- **Critérios de Entrada**: Conclusão do desenvolvimento de todas as funcionalidades, ambiente de teste configurado.
- **Critérios de Saída**: Todos os casos de teste críticos aprovados, incidentes registrados e resolvidos.

## 9. Critérios de Aprovação/Reprovação de Item
### 9.1 Critérios de Aprovação
- O item deve satisfazer todos os requisitos críticos e de segurança.
- Passar em todos os casos de teste aplicáveis sem falhas.

### 9.2 Critérios de Reprovação
- O item falha em qualquer caso de teste crítico ou requisito de segurança.
- Inconsistência ou perda de dados durante a execução do teste.

## 10. Critérios de Suspensão e Requisitos de Retomada
### 10.1 Critérios de Suspensão
|ID     |Critério                               |Descrição                                            |
|:------|:--------------------------------------|-----------------------------------------------------|
|S001   |Falha Crítica                          |Suspensão do teste até a resolução da falha crítica  |
|S002   |Falta de Recursos                      |Interrupção dos testes por falta de ambiente ou dados|

### 10.2 Requisitos de Retomada
|ID     |Requisito                              |Descrição                                            |
|:------|:--------------------------------------|-----------------------------------------------------|
|R001   |Teste Reexecutado                      |Reiniciar os testes após a resolução da falha        |
|R002   |Disponibilidade de Recursos            |Disponibilizar recursos e ambiente para retomar teste|

## 11. Entregáveis de Teste
|Entregável                        |Descrição                                             |
|:---------------------------------|------------------------------------------------------|
|Plano de Teste                    |Documento com escopo e estratégia de teste           |
|Especificações de Caso de Teste   |Documentos com casos de teste detalhados             |
|Conjuntos de Dados de Teste       |Dados para simular condições de uso real             |
|Relatórios de Execução de Teste   |Resultados dos testes realizados                     |
|Relatórios de Incidentes          |Detalhes de falhas e problemas encontrados           |
|Relatório de Resumo de Teste      |Sumário das atividades de teste realizadas           |

## 12. Tarefas de Teste Restantes
|ID     |Tarefa                           |Responsável          |Status          |Data Prevista |
|:------|:--------------------------------|:--------------------:|:--------------:|-------------:|
|T001   |Desenvolver Casos de Teste       |Ana Silva            |Em andamento    |15/10/2024    |
|T002   |Executar Testes Unitários        |Carlos Andrade       |Não Iniciado    |20/10/2024    |
|T003   |Executar Testes de Integração    |Mariana Costa        |Não Iniciado    |25/10/2024    |

## 13. Necessidades Ambientais
### 13.1 Hardware
|Item                       |Especificação        |Quantidade|Propósito                            |
|:--------------------------|:-------------------:|:--------:|------------------------------------:|
|Servidor                   |Intel Xeon           |2         |Execução de testes de carga          |
|Estação de Trabalho        |Intel i7             |5         |Execução de testes de interface      |

### 13.2 Software
|Software                   |Versão|Licença Necessária|Propósito                           |
|:--------------------------|:----:|:----------------:|-----------------------------------:|
|Windows Server             |2019  |Sim               |Servidor para ambiente de teste     |
|MySQL                      |8.0   |Não               |Banco de dados do sistema           |
|Docker                     |20.10 |Não               |Configuração de ambientes isolados  |

## 14. Necessidades de Pessoal e Treinamento
### 14.1 Pessoal
|Função                     |Habilidades Necessárias           |Número de Pessoas |
|:--------------------------|:---------------------------------|-----------------:|
|Analista de Teste          |Automação de Testes               |2                 |
|Engenheiro de QA           |Conhecimento em testes de carga   |1                 |
|Administrador de Sistemas  |Configuração de ambientes         |1                 |

### 14.2 Treinamento
|Treinamento                |Público-Alvo          |Duração          |Data Prevista |
|:--------------------------|:---------------------|:---------------:|-------------:|
|Curso de Ferramentas de Teste |Equipe de QA       |4 horas         |10/10/2024    |
|Workshop de Automação      |Analistas de Teste    |6 horas         |15/10/2024    |

## 15. Responsabilidades
|Função                     |Responsável          |Responsabilidades                                                               |
|:--------------------------|:-------------------:|-------------------------------------------------------------------------------:|
|Gerente de Teste           |Roberto Fernandes    |Planejamento e supervisão de todas as atividades de teste                      |
|Analista de Teste          |Ana Silva            |Execução e automação de casos de teste                                         |
|Engenheiro de QA           |Carlos Andrade       |Análise de desempenho e qualidade do sistema                                  |

## 16. Cronograma
|Fase                       |Data de Início       |Data de Término  |Duração          |
|:--------------------------|:-------------------:|:---------------:|----------------:|
|Planejamento               |01/10/2024           |03/10/2024       |2 dias          |
|Preparação                 |04/10/2024           |07/10/2024       |3 dias          |
|Execução                   |08/10/2024           |20/10/2024       |12 dias         |
|Avaliação                  |21/10/2024           |22/10/2024       |1 dia           |

## 17. Riscos de Planejamento e Contingências
|Risco                      |Probabilidade        |Impacto          |Estratégia de Mitigação                  |
|:--------------------------|:-------------------:|----------------:|----------------------------------------:|
|Atraso na Disponibilidade  |Alta                 |Alto             |Planejamento de recursos de backup       |
|Incompatibilidade de Ferramentas |Média         |Médio            |Teste preliminar de ferramentas          |

## 18. Aprovações
|Função                     |Nome                |Assinatura       |Data              |
|:--------------------------|:------------------:|:---------------:|------------------:|
|Gerente de Projeto         |Patrícia Sousa      |_________________|01/10/2024        |
|Gerente de QA              |João Oliveira       |_________________|02/10/2024        |
|Cliente/Stakeholder        |Eduardo Martins     |_________________|03/10/2024        |

## 19. Glossário
|Termo                      |Definição                                                             |
|:--------------------------|---------------------------------------------------------------------:|
|EPI                        |Equipamento de Proteção Individual.                                  |
|QA                         |Quality Assurance, processo de garantia de qualidade.                |
|UAT                        |User Acceptance Testing, teste de aceitação pelo usuário final.      |

