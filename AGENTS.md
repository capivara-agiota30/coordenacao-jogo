# Instruções compartilhadas para as IAs

## Configuração a preencher
- Repositório e branch compartilhada: https://github.com/capivara-agiota30/coordenacao-jogo — main
- Nome fixo desta IA: <nome>
- Experiência / Studio alvo: <identificação>
- Sistemas desta IA: <responsabilidades>

## Função do GitHub
O GitHub armazena os três documentos de coordenação. O jogo é editado no Roblox Studio, compartilhado pelo Team Create. Não copie scripts para o repositório nem configure Script Sync para este fluxo.

## Antes de trabalhar
1. Leia os três documentos na versão atual. Para economizar contexto em tarefas futuras, consulte registros posteriores ao último ID conhecido; em uma nova conversa, leia o contexto necessário. Nunca suponha memória compartilhada entre IAs.
2. Confirme qual Studio e experiência está acessando. Consulte o trecho atual do jogo que pretende alterar.
3. Escolha tarefa pendente com dependências satisfeitas. Verifique se há outra IA trabalhando no recurso ou em um recurso ancestral/descendente. Não amplie o escopo sem obter nova reserva.
4. Reserve primeiro em estado-das-ias.md, usando comparação com a versão lida. Se outra IA atualizou o documento, releia e reavalie o conflito antes de tentar novamente. Só depois da gravação confirmada marque a pendência em andamento. A reserva no documento de estados é a autoridade caso os documentos discordem.
5. Se a integração não oferece gravação condicionada à versão atual (por exemplo SHA do arquivo na API GitHub), não simule exclusividade: use divisão fixa de sistemas e peça coordenação humana para transferências. Não prometa reserva automática sem implementar e testar esse mecanismo.

## Durante a tarefa
- Edite apenas os recursos reservados, respeitando alterações manuais dos usuários.
- Antes de editar outro sistema, releia estados e atualize a reserva com controle de versão.
- Registre pedidos a outra IA nas pendências. Registrar um pedido não inicia execução nem autoriza enviar mensagens a outro chat.
- Atualize o estado nas transições importantes. Sem agendador, não há vigilância contínua nem atualização enquanto a IA está inativa.
- Coordene testes que afetem outros participantes e registre limitações.

## Ao concluir
1. Teste o resultado e registre o que realmente foi verificado.
2. Adicione a entrada em alteracoes.md preservando o ID, remova a pendência e libere a reserva. Prefira um único commit com os três arquivos, condicionado à revisão atual da branch.
3. Se a ferramenta só permite escrever arquivo por arquivo, mantenha a reserva até confirmar histórico e remoção da pendência. Libere a reserva por último; em falha, registre a situação e reconcilie pelo ID antes de continuar.
4. Nunca sobrescreva documento inteiro a partir de cópia desatualizada. Em conflito, releia e preserve as entradas das outras IAs.

## Interrupções e trabalho manual
Uma reserva antiga não é livre automaticamente. A pessoa responsável confirma se há edição em curso. Mudanças manuais relevantes devem ser registradas antes de a IA depender desses recursos.

## Instalação destas instruções
No Codex, coloque estas instruções em AGENTS.md na pasta do projeto aberta no aplicativo. Em outra IA, use o mecanismo de instruções persistentes suportado por ela, ou forneça o texto ao iniciar cada conversa. Manter este arquivo no GitHub, sozinho, não garante que a IA o leia.

## Teste de aceitação
Antes de trabalhar simultaneamente, tente reservar a mesma tarefa com as duas IAs. Apenas uma deve começar; a outra deve detectar o conflito e aguardar. Confirme também que ambas preservam entradas alheias ao atualizar documentos. Se isso não for demonstrado, use divisão fixa de sistemas.
