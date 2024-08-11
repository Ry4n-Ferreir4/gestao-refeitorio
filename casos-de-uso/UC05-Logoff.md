# Sistema de Controle de Refeitório Escolar

## UC05. Realizar Logoff
Este caso de uso descreve as etapas necessárias para que o USUÁRIO (Administrador, Nutricionista, Gestor, Funcionário do Refeitório) para realizar o logoff do sistema.

## Atores
👷 Funcionários do Refeitório, 💼 Gestor, 👩‍🍳 Nutricionista, 👨‍💼 Administrador

## Condições
### Pré-condições
O usuário deve estar autenticado no sistema.

### Pós-condições
O usuário foi desconectado do sistema com sucesso.

## Cenário principal
### Ações do ator (👨‍💼 / 👩‍🍳 / 💼 / 👷) e Ações do sistema (⚙️)
1. 👨‍💼 / 👩‍🍳 / 💼 / 👷 Seleciona a opção de logoff no menu principal.
2. ⚙️ Exibe uma mensagem de confirmação de logoff.
3. 👨‍💼 / 👩‍🍳 / 💼 / 👷 Confirma a ação de logoff.
4. ⚙️ Finaliza a sessão do usuário no sistema.
5. ⚙️ Redireciona o usuário para a tela de login.
6. ⚙️ Exibe uma mensagem de confirmação de logoff bem-sucedido.
## Restrições e validações
O usuário deve estar autenticado no sistema para realizar o logoff.

## Cenários alternativos
Cenário alternativo 1 – Cancelamento do logoff
1. ⚙️ Exibe uma mensagem de confirmação de logoff.
2. 👨‍💼 / 👩‍🍳 / 💼 / 👷 Cancela a ação de logoff.
3. ⚙️ Mantém o usuário autenticado no sistema.
4. ⚙️ Retorna ao estado anterior à tentativa de logoff.

## Exceções
Não se aplica.