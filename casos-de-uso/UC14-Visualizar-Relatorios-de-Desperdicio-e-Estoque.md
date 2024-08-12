# Sistema de Controle de Refeitório Escolar

## UC011. Registrar Preparo e Distribuição de Refeições
Este caso de uso descreve as etapas percorridas pelo Nutricionista para registrar o preparo e a distribuição das refeições no sistema.

## Atores
👩‍🍳 Nutricionista

## Condições
### Pré-condições
O Nutricionista deve estar autenticado no sistema.

### Pós-condições
O registro do preparo e distribuição das refeições foi salvo com sucesso no sistema.

## Cenário principal
### Ações do ator (👩‍🍳 ) e Ações do sistema (⚙️)
1. 👩‍🍳 Seleciona a opção "Registrar Preparo e Distribuição de Refeições" no menu principal.
2. 👩‍🍳 Escolhe a refeição a ser registrada (lanche da manhã, almoço, lanche da tarde, jantar).
3. ⚙️ Exibe o formulário para registro de preparo e distribuição.
4. 👩‍🍳 Preenche os campos obrigatórios, como quantidade de alimentos utilizados, número de porções preparadas, tempo de preparo, e quantidade distribuída.
5. 👩‍🍳 Adiciona qualquer observação relevante (por exemplo, se houve algum problema no preparo ou na distribuição).
6. 👩‍🍳 Confirma o registro.
7. ⚙️ Valida as informações fornecidas.
8. ⚙️ Salva o registro no banco de dados.
9. ⚙️ Exibe uma mensagem de sucesso confirmando que o registro foi concluído.

## Restrições e validações
1. Todos os campos obrigatórios do formulário devem ser preenchidos antes de confirmar o registro.
2. A quantidade de alimentos utilizados e de porções preparadas deve ser coerente e dentro dos limites esperados.


## Cenários alternativos
Cenário alternativo 1 –  Informações incompletas ou inválidas
1.⚙️ Identifica que as informações fornecidas são incompletas ou inválidas.
  1.1. ⚙️ Exibe uma mensagem de erro especificando o problema (por exemplo, quantidade incoerente).
  1.2  👩‍🍳 Corrige as informações.
  1.3  ⚙️ Retorna ao passo 7 do cenário principal.
Cenário alternativo 2 – Falta de ingredientes registrados no estoque
1.⚙️ Exibe uma mensagem informando que não há ingredientes suficientes registrados no estoque.
  1.1. ⚙️ Exibe uma mensagem informando que não há ingredientes suficientes registrados no estoque.
  1.2  👩‍🍳 Revê as quantidades e ajusta o registro.
  1.3  ⚙️ Retorna ao passo 7 do cenário principal.
  
## Exceções
Não se aplica.