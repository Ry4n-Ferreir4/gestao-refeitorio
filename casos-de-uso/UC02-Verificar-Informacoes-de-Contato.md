# Sistema de Controle de Refeitório Escolar

## UC02. Verificar informações de contato

Este caso de uso descreve as etapas percorridas pelo Gestor para verificar as informações de contato dos usuários no sistema.


### Atores
- 💼 Gestor


### Condições
#### Pré-condições
O Gestor deve estar autenticado no sistema.

#### Pós-condições
A conta de usuário foi criada, editada ou removida com sucesso.


### Cenário principal
#### Ações do ator (💼) e Ações do sistema (⚙️)
Ações do ator (💼) e Ações do sistema (⚙️)

1. 💼 Seleciona a opção de gerenciamento de contas de usuário no menu principal.
2. 💼 Pesquisa o usuário por nome, matrícula ou outro identificador.
3. ⚙️ Exibe a lista de resultados correspondentes à pesquisa.
4. 💼 Seleciona o usuário desejado da lista.
5. ⚙️ Exibe as informações de contato do usuário selecionado (telefone, e-mail, endereço, etc.).
6. 💼 Verifica as informações exibidas.


Restrições e validações
1. O campo de pesquisa deve ser preenchido corretamente.
2. Apenas usuários com permissões adequadas (no caso, o Gestor) podem acessar as informações de contato.

Cenário alternativo 1 – Nenhum resultado encontrado
⚙️ Identifica que a pesquisa não retornou resultados.
⚙️ Exibe uma mensagem informando que nenhum usuário foi encontrado com o critério de pesquisa fornecido.
💼 Modifica o critério de pesquisa e repete a busca.
⚙️ Retorna ao passo 3 do cenário principal.

Cenário alternativo 2 – Seleção de usuário incorreta
💼 Seleciona um usuário incorreto da lista de resultados.
⚙️ Exibe as informações de contato do usuário incorreto.
💼 Percebe que selecionou o usuário errado.
💼 Volta à lista de resultados e seleciona o usuário correto.
⚙️ Exibe as informações de contato do usuário correto.
Exceções