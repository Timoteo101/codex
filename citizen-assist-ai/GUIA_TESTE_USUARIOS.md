# Guia para testar com pessoas reais

O enunciado pede **pelo menos três pessoas de fora da equipe e dez atendimentos ou mais no total, antes da gravação**. Os testes ainda precisam ser feitos: verificação automática e perguntas feitas durante o desenvolvimento não substituem essas pessoas.

## Como organizar

1. Use uma cópia limpa do projeto com `data/historico.json` e `data/avaliacoes.json` contendo `[]`. Não apague dados de um teste já realizado sem ter uma cópia deles.
2. Convide pelo menos três pessoas externas. Explique somente que o assistente ajuda com dúvidas de documentação, trânsito e transporte. Peça para elas mesmas usarem o terminal, sem orientar qual resposta escolher.
3. Some pelo menos dez atendimentos concluídos. As pessoas podem fazer quantidades diferentes; por exemplo, 4 + 3 + 3. O programa registra cada consulta concluída. Perguntas rejeitadas por dados pessoais e saídas com `0` não contam como atendimento.
4. Peça que não digitem nomes, CPF, telefone, e-mail ou qualquer outro dado pessoal. Não registre nomes nem dados dos participantes. O filtro automático não identifica todos esses dados.
5. Depois de cada orientação, a pessoa responde `s` ou `n` para dizer se ajudou. Ao fim da sessão de cada pessoa, escolha `0` no menu e informe uma nota de facilidade de 1 a 5. Reinicie o programa para a próxima pessoa; os atendimentos e as notas anteriores ficam salvos.
6. Depois de todas as sessões, abra o programa e selecione `3` para ver os indicadores e `4` para exportar o CSV. Confira as dúvidas sem solução. Faça ao menos uma melhoria baseada em uma dificuldade observada, como adicionar uma expressão na lista de palavras-chave da orientação adequada. Teste se ela resolveu o problema e descreva isso no README. **Registre os indicadores do teste original antes de fazer novas demonstrações.**

## Exemplos de tarefas para os participantes

Use apenas como sugestões, sem obrigar todos a escrever exatamente as mesmas frases. Uma pessoa pode navegar por categoria em vez de digitar uma pergunta. Incentive dúvidas nas palavras dela.

1. Descobrir como iniciar a primeira CNH.
2. Saber a idade mínima para tirar a primeira habilitação.
3. Procurar como renovar a CNH perto do vencimento.
4. Procurar como baixar a habilitação digital.
5. Descobrir onde consultar pontos da CNH.
6. Consultar como ver multas de trânsito.
7. Procurar o documento digital do veículo.
8. Descobrir como consultar um recall.
9. Procurar orientações sobre credencial de vaga especial.
10. Encontrar informações sobre o Passe Livre interestadual.

Se alguma pergunta não for reconhecida, a pessoa deve usar a opção de tentar outras palavras ou finalizar o atendimento. Não altere a resposta registrada para parecer correta. Consulte o arquivo de histórico apenas em ambiente local e confira se não contém dados pessoais antes de qualquer publicação.

## Resultado para copiar ao README

Preencha somente depois do teste real:

```text
Quantidade de pessoas externas: [     ]
Atendimentos concluídos: [     ]
Resposta encontrada: [     ]% ([     ] / [     ])
Resposta ajudou: [     ]% ([     ] / [     ])
Tempo médio dos atendimentos com orientação: [     ] segundos
Tentativas por atendimento: [     ]
Facilidade média: [     ] de 5, em [     ] avaliações
Dúvidas sem solução, sem dados pessoais: [     ]
Dificuldade observada: [     ]
Melhoria implementada após o teste: [     ]
Como verificamos a melhoria: [     ]
```

Ao usar o programa para gravar, utilize outra cópia da pasta, para não alterar o conjunto de resultados dos testes reais.
