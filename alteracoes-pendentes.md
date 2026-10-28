# Alterações pendentes

Estados: pendente ou em andamento. Uma tarefa impedida mantém seu estado e informa o bloqueio. Exemplos e modelos não são tarefas reservadas.

## Modelo de tarefa
- ID: T-<identificador único>
- Pedido: <objetivo>
- Critério de conclusão: <resultado verificável>
- Estado: pendente
- Responsável: nenhum
- Escopo previsto: <caminhos dos scripts e objetos>
- Dependências: <IDs ou nenhuma>
- Bloqueio: nenhum
- Última atualização: <data e hora com fuso>


## T-DISPUTA-20261028-01
- ID: T-DISPUTA-20261028-01
- Pedido: testar exclusividade de reserva entre Chatgpt-arthur e outra IA, sem alterar o jogo
- Critério de conclusão: apenas uma IA mantém a reserva; a outra detecta o conflito e aguarda; ambas preservam as entradas alheias; evidências registradas antes de encerrar
- Estado: em andamento
- Responsável: Chatgpt-arthur
- Escopo previsto: recurso lógico coordenacao/testes/T-DISPUTA-20261028-01; nenhum script ou objeto do Studio
- Dependências: nenhuma
- Bloqueio: aguardando tentativa da segunda IA e registro do resultado na própria entrada de estado-das-ias.md; reserva de Chatgpt-arthur permanece ativa
- Última atualização: 2026-10-28 13:51 -03:00 (America/Sao_Paulo)
- Evidência inicial: reserva condicional ao SHA confirmada no commit d4ba4d341b8c38e3050b90362c48e5c205f1992a e relida; teste completo ainda pendente
