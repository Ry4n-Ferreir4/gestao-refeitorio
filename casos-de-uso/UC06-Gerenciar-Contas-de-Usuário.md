# Sistema de Controle de Refeitório Escolar

## UC06. Gerenciar Contas de USUÁRIO

Este caso de uso descreve as etapas percorridas pelo Administrador para gerenciar contas de usuário no sistema.


### Atores
- 👨‍💼 Administrador


### Condições
#### Pré-condições
O Administrador deve estar autenticado no sistema.

#### Pós-condições
A conta de usuário foi criada, editada ou removida com sucesso.


### Cenário principal
#### Ações do ator (👷) e Ações do sistema (⚙️)
Ações do ator (👷) e Ações do sistema (⚙️)

1. 👨‍💼 Seleciona a opção de gerenciamento de contas de usuário no menu principal.
2. 👨‍💼 Escolhe a ação desejada (criar, editar ou remover conta).
3. ⚙️ Exibe o formulário correspondente à ação escolhida.
4. 👨‍💼 Preenche ou modifica os campos necessários (nome, e-mail, perfil de acesso, etc.).
5. 👨‍💼 Confirma a ação.
6. ⚙️ Valida as informações fornecidas.
7. ⚙️ Salva as alterações no banco de dados.
8. ⚙️ Exibe uma mensagem de sucesso.

Restrições e validações
1. Todos os campos obrigatórios devem ser preenchidos.
2. O e-mail deve ser válido e único no sistema.
3. O perfil de acesso deve ser selecionado corretamente.

Cenários alternativos
Cenário alternativo 1 – Informações inválidas
⚙️ Identifica que as informações fornecidas são inválidas ou incompletas.
⚙️ Exibe mensagem de erro especificando o problema.
👨‍💼 Corrige as informações.
⚙️ Retorna ao passo 6 do cenário principal.

Cenário alternativo 2 – Remoção de conta com dependências

⚙️ Identifica que a conta a ser removida possui dependências (por exemplo: registros de atividades).
⚙️ Exibe mensagem informando sobre as dependências.
👨‍💼 Decide se deseja proceder com a remoção ou cancelar a ação.
⚙️ Se optar por proceder, realiza a remoção e lida com as dependências conforme as regras do sistema.
⚙️ Retorna ao passo 7 do cenário principal.
Exceções
Não se aplica.