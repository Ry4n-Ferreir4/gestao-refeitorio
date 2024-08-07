# Sistema de Controle de Refeitório Escolar

## UC08. Configurar Parâmetros do Sistema

Este caso de uso descreve as etapas necessárias para que o administrador configure parâmetros do sistema.

### Atores
- 👨‍💼 Administrador

### Condições
#### Pré-condições
- O administrador deve estar logado no sistema no modo administrador.

#### Pós-condições
- O sistema atualiza com as novas configurações.

### Cenário principal
#### Ações do ator (👨‍💼) e Ações do sistema (⚙️)
1. 👨‍💼 O administrador navega até o painel de administração e configuração.
2. 👨‍💼 O administrador seleciona o parâmetro que deseja configurar.
3. 👨‍💼 O administrador ajusta os valores.
4. 👨‍💼 O administrador revisa as modificações e confirma as alterações.
5. ⚙️ O sistema avalia se os valores são válidos.
6. ⚙️ O sistema salva as novas configurações e atualiza.

### Restrições e validações
- Somente administradores podem acessar e modificar os parâmetros do sistema.
- Os parâmetros devem ser válidos.

### Cenários alternativos
#### Cenário alternativo 1 – Dados inválidos
1. ⚙️ O sistema detecta que alguns dados inseridos são inválidos.
   1. ⚙️ O sistema informa que ocorreu incompatibilidade com os valores e solicita correção.
   2. 👨‍💼 O administrador muda os valores.
   3. ⚙️ Retorna ao passo 5 do cenário principal.

### Exceções
Não se aplica.
