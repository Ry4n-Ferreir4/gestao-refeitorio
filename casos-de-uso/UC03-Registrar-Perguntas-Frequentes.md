# Sistema de Controle de Refeitório Escolar

## UC03. Registrar perguntas frequentes
Este caso de uso descreve as etapas percorridas pelo Administrador ou Nutricionista para registrar perguntas frequentes no sistema.

Atores
👨‍💼 Administrador
👩‍🍳 Nutricionista
Condições
Pré-condições
O Administrador ou Nutricionista deve estar autenticado no sistema.
Pós-condições
A pergunta frequente foi registrada com sucesso no sistema.
Cenário principal
Ações do ator (👨‍💼 / 👩‍🍳) e Ações do sistema (⚙️)
👨‍💼 / 👩‍🍳 Seleciona a opção de registrar perguntas frequentes no menu principal.
👨‍💼 / 👩‍🍳 Clica no botão "Adicionar Nova Pergunta".
⚙️ Exibe um formulário para registro da pergunta frequente.
👨‍💼 / 👩‍🍳 Preenche os campos obrigatórios do formulário (pergunta, resposta).
👨‍💼 / 👩‍🍳 Confirma a inserção da pergunta frequente.
⚙️ Valida as informações fornecidas.
⚙️ Salva a pergunta e a resposta no banco de dados.
⚙️ Exibe uma mensagem de sucesso.
Restrições e validações
Todos os campos obrigatórios do formulário devem ser preenchidos.
A pergunta deve ser única, ou seja, não pode haver duplicação de perguntas no sistema.
Cenários alternativos
Cenário alternativo 1 – Informações inválidas
⚙️ Identifica que as informações fornecidas são inválidas ou incompletas.
⚙️ Exibe uma mensagem de erro especificando o problema.
👨‍💼 / 👩‍🍳 Corrige as informações.
⚙️ Retorna ao passo 6 do cenário principal.
Cenário alternativo 2 – Pergunta duplicada
⚙️ Identifica que a pergunta já existe no sistema.
⚙️ Exibe uma mensagem informando que a pergunta já está registrada.
👨‍💼 / 👩‍🍳 Modifica a pergunta para evitar duplicação.
⚙️ Retorna ao passo 6 do cenário principal.
Exceções
Não se aplica.