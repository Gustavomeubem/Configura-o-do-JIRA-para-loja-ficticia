# Configura-o-do-JIRA-para-loja-ficticia

📋 Visão Geral do Projeto
Este projeto estabelece a configuração completa do JIRA para gerenciar o desenvolvimento da loja virtual ficticia utilizando metodologia Scrum. Inclui todos os componentes necessários para um fluxo de trabalho ágil eficiente.

🎯 Estrutura do Repositório
text
swaglabs-jira-setup/
│
├── docs/
│   ├── jira-configuration.md
│   ├── scrum-workflow.md
│   └── confluence-templates.md
│
├── scripts/
│   ├── jira-automation-rules.json
│   └── custom-fields-setup.py
│
├── templates/
│   ├── user-stories-template.json
│   ├── sprint-planning-template.md
│   └── retrospective-template.md
│
├── screenshots/
│   └── workflow-visualization.png
│
└── README.md
📖 Documentação Completa
Configuração do JIRA para loja ficticia
1. Visão Geral do Projeto loja ficticia
loja ficticia é uma loja virtual de e-commerce que será desenvolvida utilizando metodologias ágeis com foco em entrega contínua de valor.

2. Metodologia Scrum Implementada
2.1. Roles Definidas
Product Owner: Responsável pelo backlog e priorização

Scrum Master: Facilita processos ágeis

Development Team: Equipe de desenvolvimento (5-8 pessoas)

2.2. Artefatos do Scrum
Product Backlog

Sprint Backlog

Incremento

2.3. Eventos do Scrum
Sprint Planning (2 horas/semana)

Daily Stand-up (15 minutos/dia)

Sprint Review (1 hora/sprint)

Sprint Retrospective (45 minutos/sprint)

3. Configuração do JIRA
3.1. Esquema de Projeto
Tipo de projeto: Scrum

Nome do projeto: loja ficticia

Chave do projeto: SLS

Lead do projeto: Product Owner

3.2. Configuração de Workflow
Workflow Personalizado:
text
[Backlog] → [Selected for Development] → [In Progress] → [Code Review] → [Testing] → [Done]
Regras de Transição:
Apenas desenvolvedores podem mover para "In Progress"

Apenas QA pode mover para "Testing"

Product Owner deve aprovar mudança para "Done"

3.3. Tipos de Issue Configurados
Epic: Funcionalidades grandes (ex: "Sistema de Pagamento")

Story: Funcionalidades do usuário (ex: "Usuário pode adicionar item ao carrinho")

Task: Tarefas técnicas (ex: "Configurar ambiente de desenvolvimento")

Bug: Problemas identificados

Sub-task: Divisões de stories/tasks

3.4. Campos Personalizados
Business Value (1-10): Valor de negócio da issue

Story Points: Estimativa de esforço (Fibonacci)

Time Tracking: Controle de horas gastas

Release Version: Versão de lançamento

3.5. Screens Configurados
Default Screen: Para a maioria das issues

Bug Screen: Campos específicos para bugs

Epic Screen: Campos específicos para epics

3.6. Permissões e Acessos
Development Team: Pode editar issues, log work, etc.

Stakeholders: Acesso apenas de leitura

Product Owner: Permissões completas de edição

4. Estrutura do Backlog
4.1. Épicos Principais
Autenticação e Perfil de Usuário

Catálogo de Produtos

Carrinho de Compras

Processo de Checkout

Sistema de Pagamento

Gestão de Pedidos

Sistema de Recomendações

4.2. Sprint 1 - Configuração Inicial
Configurar ambiente de desenvolvimento

Configurar repositório Git

Configurar integração contínua

Definir padrões de código

5. Configuração de Boards
5.1. Scrum Board
Filtro: project = SLS

Colunas: Backlog, Selected, In Progress, Review, Testing, Done

Swimlanes: Por épicos

5.2. Kanban Board (para bugs)
Filtro: project = SLS AND issuetype = Bug

Colunas: Backlog, In Progress, Testing, Done

6. Automações Configuradas
6.1. Regras de Automação
Atribuir automaticamente bugs ao QA team

Notificar quando issues ficam paradas > 2 dias

Atualizar status baseado em commits no Git

Criar sub-tasks automaticamente para épicos

6.2. Integrações
GitHub: Link entre commits e issues

Confluence: Documentação vinculada

Slack: Notificações de status

7. Relatórios e Métricas
7.1. Relatórios Principais
Velocity Chart: Velocidade da equipe

Burndown Chart: Progresso do sprint

Cumulative Flow Diagram: Fluxo de trabalho

Control Chart: Tempo de ciclo

Version Report: Progresso da versão

7.2. Métricas de acompanhamento
Velocity médio: 25 story points/sprint

Capacidade da equipe: 120 horas/sprint

Meta de lead time: < 3 dias para stories

8. Configuração do Confluence
8.1. Espaços Criados
SLS Documentation: Documentação técnica

SLS Product: Requisitos e visão do produto

SLS Meetings: Atas de reuniões

8.2. Modelos de Página
Template de Sprint Planning

Template de Retrospectiva

Template de Revisão de Sprint

Template de Documentação de Feature
