# Sistema de Controle de Refeitório Escolar

## UC10. Acessar Informações Nutricionais dos Alimentos

Este caso de uso descreve as etapas necessárias para o Nutricionista/Gestor acessar informações nutricionais dos alimentos.

### Atores
- 👩‍🍳 Nutricionista
- 💼 Gestor

### Condições
#### Pré-condições
- O usuário deve estar logado.
- O sistema deve ter dados nutricionais sobre os alimentos registrados.

#### Pós-condições
- Não se aplica.

### Cenário principal
#### Ações do ator (👩‍🍳💼) e Ações do sistema (⚙️)
1. 👩‍🍳💼 O usuário navega até a seção de informações nutricionais.
2. ⚙️ O sistema exibe uma lista de alimentos disponiveis.
3. 👩‍🍳💼 O usuário seleciona o alimento que deseja.
4. ⚙️ O sistema exibe as informações e disponibiliza opção de download.
5. 👩‍🍳💼 O usuário visualiza e opta por exportar em formatos como PDF ou Excel.
6. ⚙️ O sistema exibe mensagem de conclusão.

### Restrições e validações
- Não se aplica.

### Cenários alternativos
#### Cenário alternativo 1 – Dados incompletos
1. ⚙️ O sistema detecta que as informações nutricionais do alimento estão incompletas.
   1. ⚙️ O sistema informa ao usuário que existem espaços vazios.
   3. ⚙️ O sistema retorna ao passo 2 do cenário principal.

### Exceções
- Não se aplica.
