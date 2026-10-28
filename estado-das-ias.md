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
- Tarefa: T-DISPUTA-20261028-01 — teste de exclusividade de reserva em andamento
- Recursos reservados: coordenacao/testes/T-DISPUTA-20261028-01 (recurso lógico de teste, sem objeto no Studio); reserva ATIVA enquanto aguarda a outra IA
- Última atualização: 2026-10-28 13:55 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: outra IA deve tentar assumir a mesma tarefa, detectar esta reserva e aguardar sem transferi-la ou iniciar trabalho; registrar o resultado na própria entrada preservando as demais; aguardar validação do usuário antes de encerrar o teste
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: nenhum; este teste não autoriza alterações ou testes de execução no jogo
- Studio / experiência: PlaceId 128162258382604; GameId 10773516313; confirmado pelo usuário
- Decisões e testes feitos / pendentes: reserva original preservada após atualizações de [ANTIGRAVITY]. Relato de simulação concorrente por duas requisições registrado em T-TESTE-DISPUTA-ANTIGRAVITY-20261028 (1 sucesso e 1 HTTP 409); controle de SHA já testado diretamente por Chatgpt-arthur. Falta evidência de que a segunda IA tentou assumir T-DISPUTA-20261028-01, detectou a reserva ativa e aguardou sem reassumi-la. Simulação da API não comprova sozinha essa decisão da IA. Manter teste em andamento e reserva ativa; nenhum desenvolvimento autorizado.

## [ANTIGRAVITY]
- Nome fixo: [ANTIGRAVITY]
- Estado: livre
- Tarefa: nenhuma
- Recursos reservados: nenhum
- Última atualização: 2026-10-28 13:53 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: aguardar tarefa do usuário; teste de concorrência/disputa realizado com sucesso (mecanismo condicional por SHA funcional)
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: somente leitura e inspeção do Studio; nenhuma alteração efetuada
- Studio / experiência: projeto cyberpunk (placeId: 128162258382604); id: 66546857-569b-4503-aca6-6a489a4a072c
- Decisões e testes feitos / pendentes: TESTE-CONEXAO-ANTIGRAVITY-20261028 concluído; TESTE-DISPUTA-ANTIGRAVITY-20261028 concluído com sucesso: duas requisições concorrentes disparadas simultaneamente para a mesma versão base resultaram em 1 gravação bem-sucedida e 1 rejeição com HTTP 409 Conflict, comprovando proteção atômica contra condições de corrida
