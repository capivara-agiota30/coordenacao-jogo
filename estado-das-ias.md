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
- Estado: livre
- Tarefa: nenhuma; T-DASH-KEY-Q-20261028-01 concluída
- Recursos reservados: nenhum; reserva liberada após confirmação de alteracoes.md e remoção da pendência
- Última atualização: 2026-10-28 15:32 -03:00 (America/Sao_Paulo)
- Próximo passo / bloqueio: aguardar nova tarefa do usuário
- Substitui / substituída por: nenhum
- Progresso parcial no Studio: Dash ativado na tecla Q com animacao nativa do modelo R6 Dash Anim
- Studio / experiência: projeto cyberpunk (placeId: 128162258382604); id: 66546857-569b-4503-aca6-6a489a4a072c
- Decisões e testes feitos / pendentes: T-DASH-KEY-Q-20261028-01 concluída com sucesso; animacao oficial Dash do modelo R6 Dash Anim integrada na tecla Q; histórico registrado em alteracoes.md e pendência removida antes da liberação da reserva.


## [OPENCODE]
- Nome fixo: [OPENCODE]
- Estado: livre
- Tarefa: nenhuma; T-PUNCH-REFINE-20261029-01 concluida
- Recursos reservados: nenhum
- Ultima atualizacao: 2026-10-29 23:20 -03:00 (America/Sao_Paulo)
- Proximo passo / bloqueio: aguardar tarefa do usuario
- Substitui / substituida por: nenhum
- Progresso parcial no Studio: nenhum; soco refinado (crossfade, mao alternada, som)
- Studio / experiencia: projeto cyberpunk (placeId: 128162258382604); id: 35403bfd-be8e-48df-af28-27e0ec991899
- Decisoes e testes feitos / pendentes: T-PUNCH-REFINE-20261029-01 concluida; crossfade simetrico evita quebrar animacao em cliques rapidos; alternancia R->L validada; som 114843195133055 confirmado no personagem; play-test sem erros (rajada 8x). Pendente so confirmacao visual da troca de mao pelo usuario.
