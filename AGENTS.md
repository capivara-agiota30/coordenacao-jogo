# Instruções compartilhadas para as IAs

## Contexto do projeto
Estamos desenvolvendo em equipe um jogo no Roblox com temática cyberpunk, combinando trabalho manual dos desenvolvedores e ajuda de múltiplas IAs. O código, mapa e demais elementos do jogo são editados no Roblox Studio, com colaboração pelo Team Create. Este repositório serve para coordenação entre os participantes.

A temática cyberpunk é uma direção geral. Mecânicas, história, referências visuais e sistemas específicos ainda não estão definidos neste documento; não invente requisitos nem presuma que o jogo adapta uma franquia existente. Consulte as decisões registradas e as instruções dos desenvolvedores.

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

## Substituição de IAs e continuidade
Qualquer IA pode ser substituída por outra ferramenta, modelo ou conversa, inclusive por esgotamento do plano. Não dependa de memória da conversa: registre progresso nos marcos relevantes enquanto trabalha, pois uma interrupção pode impedir uma mensagem final.

Antes de uma troca planejada, registre em estado-das-ias.md: ID da tarefa, trabalho parcial aplicado no Studio, caminhos afetados, decisões, testes feitos e pendentes, bloqueios e próximo passo. Mantenha a tarefa em andamento; não registre como concluído o que está incompleto.

A IA substituta usa o nome informado pelo usuário no prompt, registra quem está substituindo, lê os três documentos atuais e confere no Studio o estado real dos recursos envolvidos. Se a IA anterior parou sem registrar progresso, reconstrua o contexto a partir do Studio e explicite as incertezas.

A transferência exige instrução do usuário e confirmação de que a instância anterior não continuará editando. Após essa confirmação, transfira a reserva da IA anterior para a substituta numa única atualização de estado-das-ias.md condicionada à versão lida, preservando o ID da tarefa e as reservas alheias; depois atualize o responsável nas pendências. Nunca deixe as duas como donas ativas dos mesmos recursos. Registre a anterior como substituída e a nova como responsável. Inatividade ou limite de plano presumido não transferem reservas automaticamente.

Se a IA anterior voltar, deve reler o estado e não retomar recursos já transferidos. Os registros concluídos preservam os autores originais; a substituta não assume autoria do trabalho anterior. Uma substituição não cancela tarefas nem inicia uma IA automaticamente.
