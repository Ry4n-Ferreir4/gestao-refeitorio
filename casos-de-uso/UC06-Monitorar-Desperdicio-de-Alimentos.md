# Sistema de Controle de Refeitório Escolar

## UC06. Monitorar Desperdício de Alimentos

Este caso de uso descreve as etapas necessárias para o Nutricionista/Gestor monitorar desperdício de alimentos.

### Atores
- 👩‍🍳 Nutricionista
- 💼 Gestor

### Condições
#### Pré-condições
- O usuário deve estar logado no sistema.
- O sistema deve ter relatórios de consumo e desperdício disponíveis.

#### Pós-condições
- Não se aplica.

### Cenário principal
#### Ações do ator (👩‍🍳💼) e Ações do sistema (⚙️)
1. 👩‍🍳💼 O usuário navega até a seção de relatórios gerados.
2. ⚙️ O sistema exibe uma lista de opções de relatórios gerados.
3. 👩‍🍳💼 O usuário seleciona a opção de consumo e desperdício.
4. 👩‍🍳💼 O usuário define os dados do relatório, como:
   1. Tipo de refeição (almoço, lanche, janta);
   2. Tipo de alimento.
   3. Data.
5. ⚙️ O sistema procura relatório com esses dados.
6. ⚙️ O sistema disponibiliza opção de download.
7. 👩‍🍳💼 O usuário visualiza e opta por exportar em formatos como PDF ou Excel.
8. ⚙️ O sistema exibe mensagem de conclusão.

### Restrições e validações
- Os dados devem ser válidos.

### Cenários alternativos
#### Cenário alternativo 1 – Relatório não existente
1. ⚙️ O sistema detecta que não há relatório com os dados definidos.
   1. ⚙️ O sistema informa o usuário.
   2. 💼 O usuário escolhe outros dados.
   3. ⚙️ Retorna ao passo 5 do cenário principal.

### Exceções
Não se aplica.
