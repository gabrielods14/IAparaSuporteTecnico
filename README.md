# Projeto de Sistema de Suporte com serviços de IA

Este projeto visa desenvolver um sistema integrado de suporte técnico para uma empresa de médio porte. O objetivo é substituir o atual processo de recebimento de chamados por e-mail, permitindo o registro centralizado das solicitações. A inteligência artificial (IA) será usada para sugerir soluções de forma automática ou encaminhar os chamados ao técnico adequado, com base nas intruções fornecidas pelo time de desenvolvimento.

## Objetivo Geral

Melhorar os erros cometidos por equipes de suporte 100% humanizadas e automatizar processos de trabalhos com mais eficiencia


## Requisitos Funcionais (RF)


1. Vincular o email que ser usado para responder
2. Ter um acesso admin
3. ter um um visualizador de empresas cadastradas e poder selecionar a empresa que vai mexer
4. cadastrar usuario (com niveis de acesso)
5. O sistema deve permitir o cadastro de clientes pela equipe de suporte.
6. A equipe de suporte deve conseguir configurar as instruções da IA.
7. O sistema deve receber mensagens via e-mail e WhatsApp (futuro).
8. A IA deve classificar automaticamente as mensagens recebidas.
9. A IA deve responder automaticamente quando possível.
10. Caso a IA não consiga responder, a mensagem deve ser encaminhada a um atendente humano.
11. O sistema deve armazenar todo o histórico de interações no banco de dados.

    
## Requisitos Não Funcionais (RNF)

1. Desempenho e Eficiência
2. Segurança e Privacidade
3. Manutenção e evolução
4. Usabilidade e Acessibilidade

## Diagramas do sistema 

Os diagramas do sistema estão disponíveis em pastas no repositório. Acesse-os abaixo:

## Aqui está as sprints dos requisitos do sistema:

| **REQUISITO**                                         | **TAREFA**                                                       | **SPRINT** | **PRIORIDADE** |
| ----------------------------------------------------- | ---------------------------------------------------------------- | ---------- | -------------- |
| Ter acesso admin                                      | Criar modelo de usuário com papel/admin                          | Sprint 1   | Alta           |
|                                                       | Implementar autenticação e login                                 | Sprint 1   | Alta           |
|                                                       | Criar verificação de acesso somente para admins                  | Sprint 1   | Alta           |
|                                                       | Criar interface de login                                         | Sprint 1   | Alta           |
| Cadastrar usuário                                     | Criar tela de cadastro de usuário                                | Sprint 1   | Alta           |
|                                                       | Validar dados e salvar no banco                                  | Sprint 1   | Alta           |
|                                                       | Testar criação e listagem de usuários                            | Sprint 1   | Alta           |
| Cadastrar empresas                                    | Criar modelo de empresa e relacionar com usuário                 | Sprint 1   | Alta           |
|                                                       | Criar tela e API de cadastro de empresa                          | Sprint 1   | Alta           |
| Visualizar empresas                                   | Criar tela de listagem de empresas                               | Sprint 1   | Alta           |
|                                                       | Implementar filtros e seleção                                    | Sprint 1   | Alta           |
| Cadastrar instruções                                  | Criar tela de cadastro de instruções                             | Sprint 2   | Média          |
|                                                       | Validar e salvar instruções por empresa                          | Sprint 2   | Média          |
| Vincular o e-mail que será usado                      | Criar campo de e-mail de resposta por empresa                    | Sprint 2   | Média          |
|                                                       | Configurar e testar integração com MailKit (envio e recebimento) | Sprint 2   | Média          |
| IA deve responder automaticamente                     | Criar serviço da IA que processa e envia resposta                | Sprint 2   | Média          |
|                                                       | Integrar IA com sistema de e-mail (ex: MailKit)                  | Sprint 2   | Média          |
| IA deve classificar mensagens automaticamente         | Criar serviço/classificador por palavra-chave ou NLP             | Sprint 2   | Média          |
|                                                       | Relacionar categorias com instruções salvas                      | Sprint 2   | Média          |
| Caso a IA não responda, mandar para equipe de suporte | Detectar falha na IA e encaminhar mensagem para suporte humano   | Sprint 3   | Baixa          |
|                                                       | Notificar ou registrar esse redirecionamento                     | Sprint 3   | Baixa          |
| Histórico de conversa                                 | Criar tabela de logs de mensagens                                | Sprint 3   | Baixa          |
|                                                       | Criar tela de histórico com filtros e paginação                  | Sprint 3   | Baixa          |



## Tecnologias Utilizadas

- *Linguagem*: C#
- *Framework*: .NET
- *Banco de Dados*: SQLServer
- *Ferramentas*: GitHub, Trello 


## Integrantes

- [Lucas de Oliveira Silva](https://github.com/Kript0-Web) (Scrum Master)
- [Samuel Jhonata de Lima](https://github.com/SamuJL) (PO)
- [Gabriel Oliveira dos Santos](https://github.com/gabrielods14) (Dev)
- [João Gabriel Goulart Silva](https://github.com/Goulart06) (Dev)
- [Thiago Almeida](https://github.com/Thiagoalmeida74) (Dev)
- [Richard Willian Barreto](https://github.com/RichardZl123) (Dev
