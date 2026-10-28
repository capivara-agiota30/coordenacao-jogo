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
