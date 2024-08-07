# Sistema de Controle de Refeitório Escolar

## UC09. Gerar Relatórios de Eficiência Nutricional

Este caso de uso descreve as etapas necessárias para o Nutricionista/Gestor gerar relatórios de eficiência nutricional.

### Atores
- 👩‍🍳 Nutricionista
- 💼 Gestor

### Condições
#### Pré-condições
- O usuário deve estar logado.
- O sistema deve ter dados suficientes para gerar o relatório.

#### Pós-condições
- O sistema gera o relatório.

### Cenário principal
#### Ações do ator (👩‍🍳💼) e Ações do sistema (⚙️)
1. 👩‍🍳💼 O usuário navega até a seção de relatórios.
2. ⚙️ O sistema exibe uma lista de opções de relatórios.
3. 👩‍🍳💼 O usuário seleciona a opção para gerar relatório de eficiência nutricional.
4. 👩‍🍳💼 O usuário define os valores do relatório, como:
   1. Tipo de refeição (almoço, lanche, janta);
   2. Tipo de alimento.
5. ⚙️ O sistema valida os valores inseridos.
6. ⚙️ O sistema exibe o relatório gerado e disponibiliza opção de download.
7. 👩‍🍳💼 O usuário visualiza o relatório e opta por exportá-lo em formatos como PDF ou Excel.
8. ⚙️ O sistema exibe mensagem de conclusão.

### Restrições e validações
- Os dados devem ser válidos.

### Cenários alternativos
#### Cenário alternativo 1 – Dados inválidos
1. ⚙️ O sistema detecta que alguns dados inseridos são inválidos.
   1. ⚙️ O sistema informa que ocorreu incompatibilidade com os valores e solicita correção.
   2. 👩‍🍳💼 O usuário muda os valores.
   3. ⚙️ Retorna ao passo 5 do cenário principal.

### Exceções
Não se aplica.
