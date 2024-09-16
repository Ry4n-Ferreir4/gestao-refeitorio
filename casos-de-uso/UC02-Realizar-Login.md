# Sistema de Controle de Refeitório Escolar

Este caso de uso descreve as etapas necessárias para que o Usuário não Logado faça o login no sistema.

## Casos de Uso

### UC02. Realizar Login

Este caso de uso descreve o processo pelo qual um Usuário não Logado pode fazer login no sistema. O objetivo é permitir que um usuário autenticado acesse as funcionalidades do sistema.

#### Atores
- **Usuário não Logado**: Qualquer usuário que ainda não tenha realizado o login no sistema.

#### Condições
- **Pré-condições**: O usuário não pode estar logado no sistema.
- **Pós-condições**: O usuário deve estar autenticado e redirecionado para a página inicial do sistema.

#### Cenário Principal
1. **O USUÁRIO seleciona** a opção “Fazer login”.
2. **O sistema exibe** a página de login com campos para inserção do e-mail e senha.
3. **O USUÁRIO insere** o e-mail e a senha e envia as informações para o sistema.
4. **O sistema valida** as informações fornecidas.
5. **Se as informações estiverem corretas**, o sistema envia um e-mail de confirmação para o e-mail fornecido.
6. **O sistema solicita** que o USUÁRIO confirme a autenticação clicando no link enviado por e-mail.
7. **O USUÁRIO acessa** o e-mail, clica no link de confirmação e retorna ao sistema.
8. **O sistema verifica** a confirmação do link e completa o processo de login.
9. **O sistema notifica** o USUÁRIO sobre o login bem-sucedido e redireciona-o para a página inicial.

#### Restrições e Validações
- O e-mail deve ser válido e estar associado a uma conta existente.
- A senha deve corresponder à senha registrada para o e-mail fornecido.
- O link de confirmação tem um tempo de expiração.

#### Cenários Alternativos
- **Cenário Alternativo 1 – Redefinição de Senha**
  1. **O USUÁRIO seleciona** a opção “Esqueci minha senha”.
  2. **O sistema redireciona** o USUÁRIO para a página de redefinição de senha, com campos para a inserção do e-mail.
  3. **O sistema envia** um e-mail de redefinição de senha para o endereço fornecido.
  4. **O USUÁRIO acessa** o e-mail, clica no link de redefinição de senha e insere uma nova senha.
  5. **O sistema valida** a redefinição de senha e confirma a atualização.

- **Cenário Alternativo 2 – Tentativas Múltiplas Falhas de Login**
  1. **O USUÁRIO insere** informações incorretas várias vezes.
  2. **O sistema informa** sobre o excesso de tentativas falhas.
  3. **O sistema executa** o caso de uso "Acesso Bloqueado", enviando uma mensagem detalhada sobre o bloqueio e orientações para desbloqueio.

#### Exceções
- **Exceção 1 – ID de Usuário e/ou Senha Incorretos**
  1. **O sistema informa** que as informações de login fornecidas não são válidas.
  2. **O sistema retorna** à tela de login, permitindo que o USUÁRIO tente novamente.

- **Exceção 2 – Falha na Redefinição de Senha**
  1. **O sistema informa** que os dados inseridos não estão vinculados a uma conta registrada.
  2. **O sistema apresenta** opções para voltar à tela de login ou tentar novamente a redefinição de senha.

- **Exceção 3 – Múltiplas Tentativas Falhas de Login**
  1. **O sistema informa** sobre o excesso de tentativas falhas.
  2. **O sistema executa** o caso de uso "Acesso Bloqueado", enviando uma mensagem detalhada sobre o erro e orientações para desbloqueio.

- **Exceção 4 – Tentativa de Login para um Usuário Já Logado**
  1. **O sistema informa** que a conta associada às informações de login fornecidas já está conectada ao sistema.
  2. **O sistema executa** o caso de uso "Acesso Bloqueado", enviando uma mensagem detalhada sobre o erro e orientações para resolução.
