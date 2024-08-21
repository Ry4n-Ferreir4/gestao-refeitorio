# Relações entre Usuario e Relatorio e PreparoDistribuicaoRefeicao:

### Usuario "1" o-- "0..*" Relatorio : gera

- Significado: Um Usuário pode gerar zero ou mais Relatórios. A relação indica que qualquer instância de Usuario (como Administrador, Gestor, etc.) pode estar associada a vários relatórios que ele mesmo gerou.

- Detalhes: O "1" indica que a relação é com um único usuário, e o "0..*" indica que pode haver nenhum ou múltiplos relatórios gerados por esse usuário.

### Usuario "1" o-- "0..*" PreparoDistribuicaoRefeicao : registra

- Significado: Um Usuário pode registrar zero ou mais PreparoDistribuicaoRefeicao. Isso significa que qualquer usuário pode estar associado a múltiplos registros de preparo e distribuição de refeições.

- Detalhes: O "1" representa um único usuário, e o "0..*" representa a possibilidade de que o usuário registre nenhum ou vários preparos e distribuições de refeições.

### Relações entre Administrador e Cardapio: Administrador "1" o-- "0..*" Cardapio : cria

- Significado: Um Administrador pode criar zero ou mais Cardapios. Isso significa que o administrador pode estar associado a vários cardápios que ele criou.

- Detalhes: O "1" indica um administrador específico, e o "0..*" indica a quantidade de cardápios que ele pode criar.

### Administrador "1" o-- "0..*" Cardapio : edita

- Significado: Um Administrador pode editar zero ou mais Cardapios. Isso significa que o administrador tem a capacidade de modificar vários cardápios.

- Detalhes: O "1" representa um administrador, e o "0..*" indica que ele pode editar nenhum ou vários cardápios.

### Administrador "1" o-- "0..*" Cardapio : exclui

- Significado: Um Administrador pode excluir zero ou mais Cardapios. Isso implica que o administrador tem a capacidade de remover vários cardápios do sistema.

- Detalhes: O "1" representa um administrador, e o "0..*" significa que ele pode excluir nenhum ou vários cardápios.

### Relações entre Administrador e Estoque: Administrador "1" o-- "0..*" Estoque : cria

- Significado: Um Administrador pode criar zero ou mais Itens de Estoque. Isso significa que o administrador pode adicionar novos itens de estoque.

- Detalhes: O "1" representa um administrador, e o "0..*" indica a quantidade de itens de estoque que ele pode criar.

### Administrador "1" o-- "0..*" Estoque : edita

- Significado: Um Administrador pode editar zero ou mais Itens de Estoque. Isso significa que o administrador pode modificar os detalhes dos itens de estoque existentes.

- Detalhes: O "1" representa um administrador, e o "0..*" representa os itens de estoque que ele pode editar.

### Administrador "1" o-- "0..*" Estoque : exclui

- Significado: Um Administrador pode excluir zero ou mais Itens de Estoque. Isso significa que o administrador pode remover itens de estoque do sistema.

- Detalhes: O "1" indica um administrador, e o "0..*" representa os itens de estoque que ele pode excluir.

### Administrador "1" o-- "0..*" Estoque : lista

- Significado: Um Administrador pode listar zero ou mais Itens de Estoque. Isso significa que o administrador pode visualizar a lista de itens de estoque disponíveis.

- Detalhes: O "1" representa um administrador, e o "0..*" indica a quantidade de itens de estoque que ele pode listar.

### Administrador "1" o-- "0..*" Relatorio : visualiza

- Significado: Um Administrador pode visualizar zero ou mais Relatórios. Isso indica que o administrador pode acessar e visualizar relatórios gerados no sistema.

- Detalhes: O "1" representa um administrador, e o "0..*" significa que ele pode visualizar nenhum ou vários relatórios.

### Relações entre Gestor e Cardapio: Gestor "1" o-- "0..*" Cardapio : cria

- Significado: Um Gestor pode criar zero ou mais Cardapios. Isso significa que o gestor tem a capacidade de adicionar novos cardápios.

- Detalhes: O "1" representa um gestor específico, e o "0..*" representa a quantidade de cardápios que ele pode criar.

### Gestor "1" o-- "0..*" Cardapio : edita

 - Significado: Um Gestor pode editar zero ou mais Cardapios. Isso implica que o gestor pode modificar cardápios existentes.

- Detalhes: O "1" representa um gestor, e o "0..*" indica os cardápios que ele pode editar.

### Gestor "1" o-- "0..*" Cardapio : exclui

- Significado: Um Gestor pode excluir zero ou mais Cardapios. Isso significa que o gestor tem a capacidade de remover cardápios do sistema.

- Detalhes: O "1" representa um gestor, e o "0..*" indica os cardápios que ele pode excluir.
Relações entre Gestor e Estoque:

### Gestor "1" o-- "0..*" Estoque : cria

- Significado: Um Gestor pode criar zero ou mais Itens de Estoque. Isso indica que o gestor pode adicionar novos itens de estoque.

- Detalhes: O "1" representa um gestor, e o "0..*" indica a quantidade de itens de estoque que ele pode criar.

### Gestor "1" o-- "0..*" Estoque : edita

- Significado: Um Gestor pode editar zero ou mais Itens de Estoque. Isso significa que o gestor pode modificar os itens de estoque existentes.

- Detalhes: O "1" representa um gestor, e o "0..*" indica os itens de estoque que ele pode editar.

### Gestor "1" o-- "0..*" Estoque : exclui

- Significado: Um Gestor pode excluir zero ou mais Itens de Estoque. Isso significa que o gestor pode remover itens de estoque do sistema.

- Detalhes: O "1" representa um gestor, e o "0..*" indica os itens de estoque que ele pode excluir.

### Gestor "1" o-- "0..*" Estoque : lista

- Significado: Um Gestor pode listar zero ou mais Itens de Estoque. Isso indica que o gestor pode visualizar a lista de itens de estoque disponíveis.

- Detalhes: O "1" representa um gestor, e o "0..*" indica a quantidade de itens de estoque que ele pode listar.

### Gestor "1" o-- "0..*" Relatorio : visualiza

- Significado: Um Gestor pode visualizar zero ou mais Relatórios. Isso significa que o gestor tem a capacidade de acessar e ver relatórios gerados no sistema.

- Detalhes: O "1" representa um gestor, e o "0..*" indica os relatórios que ele pode visualizar.
Relações entre Nutricionista e Estoque:

### Nutricionista "1" o-- "0..*" Estoque : cria

- Significado: Um Nutricionista pode criar zero ou mais Itens de Estoque. Isso significa que o nutricionista tem a capacidade de adicionar novos itens de estoque.
- Detalhes: O "1" representa um nutricionista, e o "0..*" indica os itens de estoque que ele pode criar.

### Nutricionista "1" o-- "0..*" Estoque : edita

- Significado: Um Nutricionista pode editar zero ou mais Itens de Estoque. Isso indica que o nutricionista pode modificar os detalhes dos itens de estoque existentes.

- Detalhes: O "1" representa um nutricionista, e o "0..*" indica os itens de estoque que ele pode editar.

### Nutricionista "1" o-- "0..*" Estoque : exclui

- Significado: Um Nutricionista pode excluir zero ou mais Itens de Estoque. Isso significa que o nutricionista pode remover itens de estoque do sistema.

- Detalhes: O "1" representa um nutricionista, e o "0..*" indica os itens de estoque que ele pode excluir.

### Nutricionista "1" o-- "0..*" Estoque : lista

- Significado: Um Nutricionista pode listar zero ou mais Itens de Estoque. Isso implica que o nutricionista pode visualizar a lista de itens de estoque disponíveis.

- Detalhes: O "1" representa um nutricionista, e o "0..*" indica os itens de estoque que ele pode listar.

### Nutricionista "1" o-- "0..*" Relatorio : visualiza

- Significado: Um Nutricionista pode visualizar zero ou mais Relatórios. Isso significa que o nutricionista pode acessar e visualizar relatórios gerados no sistema.

- Detalhes: O "1" representa um nutricionista, e o "0..*" indica os relatórios que ele pode visualizar.

## Relação entre FuncionarioRefeitorio e PreparoDistribuicaoRefeicao:

### FuncionarioRefeitorio "1" o-- "0..*" PreparoDistribuicaoRefeicao : registra

- Significado: Um Funcionário de Refeitório pode registrar zero ou mais PreparoDistribuicaoRefeicao. Isso significa que o funcionário pode registrar várias ocorrências de preparo e distribuição de refeições.

- Detalhes: O "1" representa um funcionário de refeitório, e o "0..*" indica as ocorrências de preparo e distribuição de refeições que ele pode registrar.

## Relação entre UsuarioNaoLogado e Cardapio:

### UsuarioNaoLogado "1" o-- "0..*" Cardapio : visualiza
- Significado: Um Usuário Não Logado pode visualizar zero ou mais Cardapios. Isso significa que um usuário que não está logado pode acessar e visualizar os cardápios disponíveis.

- Detalhes: O "1" representa um usuário não logado, e o "0..*" indica os cardápios que ele pode visualizar.