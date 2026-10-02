---
impacto: capacidade_nova
secao: alterado
titulo: A tela "Uso de IA" passa a contar o período inteiro e separa chamadas de turnos do agente
---
Em instalações com mais de mil chamadas à IA no período, a tela "Uso de IA" somava só as primeiras mil e deixava de fora justamente os dias mais recentes: o custo, os tokens e o tempo apareciam menores do que eram. A taxa de conversas passadas para uma pessoa também era calculada sobre um recorte. Agora a conta é feita inteira no banco, para o período todo.

Os cartões também passaram a dizer o que medem. "Atendimentos com IA" virou "Chamadas de IA", porque contava cada chamada ao modelo, e uma resposta do agente costuma fazer várias. Há um cartão novo, "Turnos do agente", com o custo médio de cada resposta. Ele conta só os turnos que a fila de tarefas ainda guarda, por padrão os últimos 90 dias. Outro cartão novo, "Taxa de cache", mostra quanto do texto enviado à IA veio do cache, que custa bem menos. "Tempo de resposta" virou "Tempo de uma chamada à IA": é o tempo de uma chamada ao modelo, não o tempo que o cliente esperou pela resposta inteira.

O cartão de orçamento do mês não mudou e continua usando a mesma conta que decide o limite de gasto. A atualização traz uma função nova no banco (migration 0523), aplicada pelo `update.sh` de sempre. Não é preciso fazer nada na instalação.
