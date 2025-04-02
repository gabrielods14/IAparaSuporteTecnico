# Projeto de Sistema de Suporte com serviços de IA

Este projeto visa desenvolver um sistema integrado de suporte técnico para uma empresa de médio porte. O objetivo é substituir o atual processo de recebimento de chamados por e-mail, permitindo o registro centralizado das solicitações. A inteligência artificial (IA) será usada para sugerir soluções de forma automática ou encaminhar os chamados ao técnico adequado, com base nas intruções fornecidas pelo time de desenvolvimento.

## Objetivo Geral

Melhorar os erros cometidos por equipes de suporte 100% humanizadas e automatizar processos de trabalhos com mais eficiencia.


## Requisitos Funcionais (RF)


1. O sistema deve permitir o cadastro de clientes pela equipe de suporte.
2. A equipe de suporte deve conseguir configurar as instruções da IA.
3. O sistema deve receber mensagens via e-mail e WhatsApp (futuro).
4. A IA deve classificar automaticamente as mensagens recebidas.
5. A IA deve responder automaticamente quando possível.
6. Caso a IA não consiga responder, a mensagem deve ser encaminhada a um atendente humano.
7. O sistema deve armazenar todo o histórico de interações no banco de dados.
   

## Requisitos Não Funcionais (RNF)


1. O sistema deve ser desenvolvido em C# e utilizar SQLServer como banco de dados.
2. A IA deve utilizar serviços como OpenAI ou Dialogflow para NLP.
3. O sistema deve garantir segurança e privacidade dos dados dos clientes.
4. O tempo de resposta da IA pode ser escolhida para deixar mais humanizada
5. O sistema deve ser escalável para suportar múltiplos clientes simultaneamente.
   

## Diagramas do sistema 

Os diagramas do sistema estão disponíveis em pastas no repositório. Acesse-os abaixo:

- [Diagramas de caso de uso](https://github.com/gabrielods14/IAparaSuporteTecnico/tree/main/Diagramas%20de%20Caso%20de%20Uso)


## Sprints

As sprints foram dividias em 4 etapas para serem feitas em 1 semana cada, sendo elas:

Aqui está o quadro com a divisão das sprints:  

| **Sprint** | **Objetivo** | **Principais Tarefas** | **Entrega Esperada** |  
|-----------|------------|------------------|----------------|  
| **Sprint 1** | Configuração do sistema e integração com e-mail | - Modelagem do banco de dados<br>- Implementar API backend em C#<br>- Criar painel administrativo básico<br>- Configurar integração com e-mail (MailKit)<br>- Documentação inicial | O sistema recebe e-mails e os armazena no banco de dados |  
| **Sprint 2** | Implementação da IA para classificar e responder e-mails | - Configurar OpenAI/Dialogflow<br>- Criar regras de categorização de mensagens<br>- Implementar respostas automáticas da IA<br>- Melhorar o painel administrativo<br>- Criar logs de interações | Sistema classifica e responde automaticamente via e-mail |  
| **Sprint 3** | Encaminhamento para atendentes e melhorias no atendimento | - Implementar encaminhamento para atendente humano<br>- Criar notificações de novos tickets<br>- Melhorar monitoramento no painel administrativo<br>- Refinar IA para respostas mais humanizadas<br>- Testes de desempenho | Sistema identifica problemas simples e complexos, enviando os difíceis para atendentes |  
| **Sprint 4** | Ajustes finais e refinamento para entrega | - Otimizar integração com e-mail<br>- Melhorar interface do painel administrativo<br>- Criar relatórios de desempenho da IA<br>- Ajustar IA com base nos testes finais<br>- Correção de bugs e documentação final | Sistema totalmente funcional e pronto para apresentação |  


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
- [Richard Willian Barreto](https://github.com/RichardZl123) (Dev)
