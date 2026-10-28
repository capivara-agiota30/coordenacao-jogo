# Estado das IAs

Este documento é a referência para reservas. A reserva só existe após uma gravação com controle de concorrência bem-sucedida. Não trate uma leitura como reserva. Estados possíveis: livre, trabalhando, aguardando, interrompida ou substituída.

## Modelo de agente
- Nome fixo: <por exemplo ChatGPT-Arthur>
- Estado: livre
- Tarefa: nenhuma
- Recursos reservados: nenhum
- Última atualização: <data e hora com fuso>
- Próximo passo / bloqueio: nenhum
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: nenhum
- Decisões e testes feitos / pendentes: nenhum

Uma reserva inclui o recurso indicado e seus descendentes no Explorer. Reservar uma pasta conflita com reservas dos scripts dentro dela. Reserve também ações de teste compartilhadas quando puderem afetar os demais.

Uma atualização antiga não libera uma reserva automaticamente. Confirme a situação com a pessoa responsável antes de reassumir.


## Transferência de responsabilidade
Siga AGENTS.md. Após instrução do usuário e confirmação de que a IA anterior parou, transfira a reserva numa atualização condicionada à versão atual deste documento. A substituta mantém o ID da tarefa e confere as alterações parciais no Studio. Não libere reservas por tempo decorrido. A IA anterior deve consultar este documento antes de voltar a editar.

## Chatgpt-arthur
- Nome fixo: Chatgpt-arthur
- Estado: aguardando
- Tarefa: nenhuma; configuração concluída (T-CONEXAO-Chatgpt-arthur-20261028)
- Recursos reservados: nenhum
- Última atualização: 2026-10-28 13:32 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: aguardar tarefa do usuário; antes de edição simultânea, realizar teste de disputa entre duas IAs ou usar divisão fixa de sistemas
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: somente leitura dos identificadores; nenhuma alteração
- Studio / experiência: Local de Capivara_agiota30: 10282026_1; PlaceId 128162258382604; GameId 10773516313; confirmado pelo usuário
- Decisões e testes feitos / pendentes: TESTE-CONEXAO-Chatgpt-arthur-20261028: leitura e escrita autenticadas confirmadas em main; registro inicial por SHA confirmado e relido; tentativa com SHA antigo rejeitada com HTTP 409 CONFLICT; instruções locais em C:/Users/Arthur/Documents/ChatGPT/cybepunk v2 roblox/AGENTS.md; histórico registrado em alteracoes.md; teste de disputa entre duas IAs ainda não realizado, usar divisão fixa de sistemas até validação

## [ANTIGRAVITY]
- Nome fixo: [ANTIGRAVITY]
- Estado: livre
- Tarefa: nenhuma
- Recursos reservados: nenhum
- Última atualização: 2026-10-28 13:50 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: aguardar tarefa do usuário; antes de edição simultânea, realizar teste de disputa entre duas IAs ou usar divisão fixa de sistemas
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: somente leitura e inspeção do Studio; nenhuma alteração efetuada
- Studio / experiência: projeto cyberpunk (placeId: 128162258382604); id: 66546857-569b-4503-aca6-6a489a4a072c
- Decisões e testes feitos / pendentes: TESTE-CONEXAO-ANTIGRAVITY-20261028: leitura e escrita autenticadas via GitHub CLI; MCP nativo Roblox Studio verificado via tool list_roblox_studios; teste condicional com SHA realizado; instruções locais persistentes em AGENTS.md
