# Projeto de Sistema de Suporte com serviços de IA

Este projeto visa desenvolver um sistema integrado de suporte técnico para uma empresa de médio porte. O objetivo é substituir o atual processo de recebimento de chamados por e-mail, permitindo o registro centralizado das solicitações. A inteligência artificial (IA) será usada para sugerir soluções de forma automática ou encaminhar os chamados ao técnico adequado, com base nas intruções fornecidas pelo time de desenvolvimento.

## Objetivo Geral

Melhorar os erros cometidos por equipes de suporte 100% humanizadas e automatizar processos de trabalhos com mais eficiencia


## Requisitos Funcionais (RF)


1. Login do usuário 
2. cria histórico de problemas 
3. da soluções para o cliente 
4. deixa criar introduções 
5. entende o problema por palavras chaves 
6. cria histórico 
7. manda feedback pro suporte 
8. pede feedback para o cliente sobre o problema se foi resolvido 
9. responde por e-mail 
10. prioriza os chamados por complexidade do problemas 

## Requisitos Não Funcionais (RNF)

1. Desempenho e Eficiência
2. Segurança e Privacidade
3. Manutenção e evolução
4. Usabilidade e Acessibilidade

## Diagramas do sistema 

Os diagramas do sistema estão disponíveis em pastas no repositório. Acesse-os abaixo:

## Aqui está as sprints dos requisitos do sistema:

| Sprint | Objetivo | Principais Tarefas | Entrega Esperada |
|-----------|------------|------------------|----------------|
| Sprint 1 | Configuração do sistema e integração com e-mail | - Modelagem do banco de dados<br>- Implementar API backend em C#<br>- Criar painel administrativo básico<br>- Configurar integração com e-mail (MailKit)<br>- Documentação inicial | O sistema recebe e-mails e os armazena no banco de dados |
| Sprint 2 | Implementação da IA para classificar e responder e-mails | - Configurar OpenAI/Dialogflow<br>- Criar regras de categorização de mensagens<br>- Implementar respostas automáticas da IA<br>- Melhorar o painel administrativo<br>- Criar logs de interações | Sistema classifica e responde automaticamente via e-mail |
| Sprint 3 | Encaminhamento para atendentes e melhorias no atendimento | - Implementar encaminhamento para atendente humano<br>- Criar notificações de novos tickets<br>- Melhorar monitoramento no painel administrativo<br>- Refinar IA para respostas mais humanizadas<br>- Testes de desempenho | Sistema identifica problemas simples e complexos, enviando os difíceis para atendentes |
| Sprint 4 | Ajustes finais e refinamento para entrega | - Otimizar integração com e-mail<br>- Melhorar interface do painel administrativo<br>- Criar relatórios de desempenho da IA<br>- Ajustar IA com base nos testes finais<br>- Correção de bugs e documentação final | Sistema totalmente funcional e pronto para apresentação |


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
