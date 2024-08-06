# Sistema de Controle de Refeitório Escolar

## UC01. Cadastrar Cardápio do Dia

Este caso de uso descreve as etapas percorridas pelo Administrador para cadastrar o cardápio do dia no sistema.

### Atores
- 👨‍💼 Administrador

### Condições
#### Pré-condições
Não se aplica.

#### Pós-condições
O sistema deve cadastrar o cardápio do dia e disponibilizá-lo para consulta pelos usuários.

### Cenário principal
#### Ações do ator (👨‍💼) e Ações do sistema (⚙️)
1. 👨‍💼 Seleciona a data para a qual deseja cadastrar o cardápio.
2. 👨‍💼 Informa os pratos disponíveis para o café da manhã, almoço e jantar.
3. ⚙️ Armazena as informações do cardápio do dia no sistema.
4. ⚙️ Exibe uma mensagem confirmando que o cardápio do dia foi cadastrado com sucesso.

### Restrições e validações
1. Todos os campos do cardápio do dia devem ser preenchidos corretamente, incluindo a data e os pratos disponíveis para cada refeição.
2. O sistema deve validar se a data selecionada pelo Administrador está correta e se os pratos informados estão de acordo com as opções disponíveis.

### Cenários alternativos
#### Cenário alternativo 1 – Data inválida
2. ⚙️ Identifica que a data selecionada não é válida (por exemplo, data passada ou data fora do período letivo).
   1. ⚙️ Informa ao Administrador que a data selecionada não é válida.
   2. 👨‍💼 Opta por selecionar uma nova data ou cancelar o cadastro.
   3. ⚙️ Se o Administrador optar por selecionar uma nova data, retorna ao passo 1 do cenário principal.

#### Cenário alternativo 2 – 

### Exceções
Não se aplica.
