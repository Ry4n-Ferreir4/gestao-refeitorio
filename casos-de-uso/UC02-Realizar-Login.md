# Sistema de Controle de Refeitório Escolar

## UC02. Realizar Login

Este caso de uso descreve as etapas necessárias para que o Usuário não Logado faça o login no sistema.

### Atores
- 👤 Usuário não Logado

### Condições
#### Pré-condições
O usuário não pode estar logado.

#### Pós-condições
Não se aplica.


### Cenário principal
#### Ações do ator (👤) e Ações do sistema (⚙️)

1. 👤 O USUÁRIO seleciona a opção “Fazer login”.
2. 👤 Redirecionar o USUÁRIO para a página de login, com campos para a inserção dos dados necessários (ID de login e endereço de e-mail vinculado a conta).
3. ⚙️ Mostrar mensagem de sucesso, pedindo para que o USUÁRIO confirme no endereço de Email vinculado.
4. ⚙️ Mostrar mensagem de sucesso ao fazer login para o usuário.

### Restrições e validações
Não se aplica.

### Cenários alternativos
#### Cenário alternativo 1 – Redefinição de senha
1. 👤 O USUÁRIO seleciona a opção “Esqueci minha senha”.
2. ⚙️ Redirecionar o USUÁRIO para a página de redefinição de senha, com campos para a inserção dos dados necessários (ID de login e endereço de e-mail vinculado a conta).
3. ⚙️ Mostrar mensagem de sucesso, pedindo para que o USUÁRIO confirme a redefinição de senha no endereço de Email vinculado.

### Exceções
#### Exceção 1 – Id de usuário e/ou senha incorretas
1. ⚙️ Informar ao USUÁRIO que as informações de login fornecidas não foram válidas.
2. ⚙️ Voltar à tela de login.

#### Exceção 2 – Falha na redefinição de senha
1. ⚙️ Mostrar mensagem de falha ao tentar redefinir a senha pois os dados inseridos não estão vinculados à uma conta cadastrada.
2. ⚙️ Mostrar opções de voltar para a tela de login e de tentar novamente a redefinição de senha.

#### Exceção 3 – Múltiplas tentativas falhas de fazer login
1. ⚙️  Informar ao USUÁRIO que houve um excesso de tentativas falhas de fazer login no sistema..
2. ⚙️  Executar caso de uso ACESSO BLOQUEADO, enviando mensagem detalhando o erro correspondente.

#### Exceção 4  – Tentativa de login à um usuário que já está logado
1. ⚙️ Informar ao USUÁRIO que o login não foi possível devido à conta associada às informações de login fornecidas já estar conectada ao sistema.
2. ⚙️ Executar caso de uso ACESSO BLOQUEADO, enviando mensagem detalhando o erro correspondente.
