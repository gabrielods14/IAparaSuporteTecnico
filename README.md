# Projeto de Sistema de Suporte com serviços de IA

Este projeto visa desenvolver um sistema integrado de suporte técnico para uma empresa de médio porte. O objetivo é substituir o atual processo de recebimento de chamados por e-mail, permitindo o registro centralizado das solicitações. A inteligência artificial (IA) será usada para sugerir soluções de forma automática ou encaminhar os chamados ao técnico adequado, com base nas intruções fornecidas pelo time de desenvolvimento.

## Objetivo Geral

Melhorar os erros cometidos por equipes de suporte 100% humanizadas e automatizar processos de trabalhos com mais eficiencia


## Requisitos Funcionais (RF


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


## Sprint Backlog

A sprint backlog foi feita levanto os seguintes requisitos em consideração, MVP e prioridade. Usamos a metodologia de MVP para listar os requisitos minimos para ter um produto funcionando. Basedado nisso também levamos em consideração a importancia de cada requisito, dado como alta: Prioridade máxima. Média: Muito importante, porém menos urgente. Bixa: Requisito que pode ser feito mais para o final, levando em consideração funções que podem ser fetias após o sistema pronto. Abaixo terá um link para um arquivo PNG, onde tem uma tabela feita em Execel ilustrando está descrição.

- [Tabela sprint Backlog](https://github.com/gabrielods14/IAparaSuporteTecnico/blob/main/Sprint%20Backlog/sprintbacklog.jpg)


## Aqui está as sprints dos requisitos do sistema:

A formatação feita para o Github perdeu as datas. As sprints foram usados duas semanas para cada uma. A sprint 1 foi usado do dia 8 de abril até dia 15 de abril. A sprint 2 do dia 15 até dia 29. E a sprint 3 ainda está em desenvolvimento, começou no dia 30 e vai até dia 13.

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


## o arquivo astah com os diagramas está neste link:

- [Arquivo Astah](https://github.com/gabrielods14/IAparaSuporteTecnico/tree/main/Pasta%20diagramas%20do%20sistema)

## Planilha de teste unitário

Esta planilha reúne os principais testes unitários do sistema Help IA. Cada linha descreve uma funcionalidade testada, incluindo pré-condições, dados de entrada, resultado esperado, critério de aceitação e prioridade.

O objetivo é garantir que cada função do sistema funcione corretamente de forma isolada, contribuindo para a estabilidade e qualidade do projeto. 

| **ID** | **Função**                  | **Descrição do Caso de Teste**                           | **Pré-condição**                               | **Dados de Entrada**                  | **Resultado Esperado**                                        | **Critério de Aceitação**                                                   | **Prioridade** |
| ------ | --------------------------- | -------------------------------------------------------- | ---------------------------------------------- | ------------------------------------- | ------------------------------------------------------------- | --------------------------------------------------------------------------- | -------------- |
| TC001  | Login_admin()                 | Verificar login com credenciais válidas                  | Admin já cadastrado                            | Usuário: admin<br>Senha: admin        | Acesso ao sistema com permissões de admin                     | Sistema deve permitir acesso e redirecionar para dashboard do admin         | Alta           |
| TC002  | Cadastro_de_usuário()         | Criar um novo usuário com perfil comum                   | Admin logado                                   | Nome, Email, Senha, Papel = "usuário" | Usuário criado e salvo no banco                               | Exibir mensagem de sucesso e listar novo usuário no painel                  | Alta           |
| TC003  | Cadastro_de_empresa()         | Cadastrar uma nova empresa                               | Admin logado                                   | Nome da empresa, CNPJ, Email, etc.    | Empresa salva no banco e listada na tela de empresas          | Exibir confirmação de cadastro e listar empresa em tela                     | Alta           |
| TC004  | Cadastro_de_instrução_da_IA() | Criar nova instrução para resposta automática da IA      | Admin e funcionsario logado e empresa selecionada             | Palavra-chave, resposta, contexto     | Instrução salva com sucesso                                   | IA passa a responder e-mail relacionado ao tema usando essa instrução       | Média          |
| TC005  | Classificação_de_e-mails()    | IA deve classificar e-mails recebidos                    | IA ativa e empresa com instruções cadastradas  | E-mail com palavras-chave             | IA classifica corretamente com base nas instruções existentes | Classificação condizente com conteúdo da mensagem recebida                  | Média          |
| TC006  | Resposta_automática()         | IA deve responder automaticamente com base em instrução  | E-mail classificado e instrução correspondente | E-mail com problema comum             | E-mail respondido com texto da instrução                      | Cliente recebe resposta automaticamente no e-mail                           | Alta           |
| TC007  | Encaminhamento_ao_suporte()   | IA não entende o e-mail e encaminha ao suporte humano    | E-mail sem correspondência nas instruções      | E-mail com conteúdo novo              | E-mail redirecionado à equipe de suporte                      | Mensagem não respondida automaticamente deve ser visível ao time de suporte | Baixa          |
| TC008  | Histórico_de_conversa()       | Verificar se o sistema salva todas as mensagens tratadas | IA ou suporte responde e-mails                 | Nenhum (é automático)                 | Histórico salvo no banco e acessível                          | Admin pode visualizar histórico completo das interações com clientes        | Baixa          |


## Tecnologias Utilizadas

- *Linguagem*: C#
- *Framework*: .NET
- *Banco de Dados*: SQLServer
- *Ferramentas*: GitHub, Trello, Figma


## Integrantes

- [Lucas de Oliveira Silva](https://github.com/Kript0-Web) (Scrum Master)
- [Samuel Jhonata de Lima](https://github.com/SamuJL) (PO)
- [Gabriel Oliveira dos Santos](https://github.com/gabrielods14) (Dev)
- [João Gabriel Goulart Silva](https://github.com/Goulart06) (Dev)
- [Thiago Almeida Ribeiro](https://github.com/Thiagoalmeida74) (Dev)
- [Richard Willian Barreto](https://github.com/RichardZl123) (Dev)
