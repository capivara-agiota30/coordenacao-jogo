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
- Estado: livre
- Tarefa: nenhuma; T-DISPUTA-20261028-01 concluída e registrada em alteracoes.md
- Recursos reservados: nenhum; reserva lógica do teste liberada após confirmar histórico e remoção da pendência
- Última atualização: 2026-10-28 13:59 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: aguardar tarefa do usuário; adquirir nova reserva condicional ao SHA antes de editar
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: nenhum; jogo não alterado durante os testes
- Studio / experiência: PlaceId 128162258382604; GameId 10773516313; confirmado pelo usuário
- Decisões e testes feitos / pendentes: teste de aceitação T-DISPUTA-20261028-01 concluído: reserva condicional por Chatgpt-arthur; [ANTIGRAVITY] detectou a reserva ativa, não assumiu, aguardou e preservou a entrada alheia; Chatgpt-arthur preservou a entrada de [ANTIGRAVITY]. Controle de SHA antigo rejeitado com HTTP 409; simulação concorrente documentada pela outra IA em T-TESTE-DISPUTA-ANTIGRAVITY-20261028. Histórico e retirada da pendência confirmados antes desta liberação. Nenhum desenvolvimento iniciado.

## [ANTIGRAVITY]
- Nome fixo: [ANTIGRAVITY]
- Estado: aguardando
- Tarefa: nenhuma (avaliou T-DISPUTA-20261028-01 e NÃO pode assumi-la devido à reserva ativa de Chatgpt-arthur)
- Recursos reservados: nenhum
- Última atualização: 2026-10-28 13:58 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: aguardando conclusão ou liberação por Chatgpt-arthur de T-DISPUTA-20261028-01; reserva alheia ativa detectada e respeitada; nenhum trabalho ou alteração iniciado
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: somente leitura e inspeção do Studio; nenhuma alteração efetuada
- Studio / experiência: projeto cyberpunk (placeId: 128162258382604); id: 66546857-569b-4503-aca6-6a489a4a072c
- Decisões e testes feitos / pendentes: T-DISPUTA-20261028-01 lida em alteracoes-pendentes.md e estado-das-ias.md; detectada reserva ativa de Chatgpt-arthur no recurso coordenacao/testes/T-DISPUTA-20261028-01; em conformidade com as regras de AGENTS.md, [ANTIGRAVITY] NÃO assumiu a tarefa, manteve recursos_reservados=nenhum, mudou estado para 'aguardando' e preservou integralmente a entrada de Chatgpt-arthur. Teste de disputa entre IAs validado em comportamento.
