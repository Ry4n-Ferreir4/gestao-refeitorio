```mermaid
classDiagram
    Usuario <|-- Administrador
    Usuario <|-- Nutricionista
    Usuario <|-- Gestor
    Usuario <|-- FuncionarioRefeitorio
    Usuario <|-- UsuarioNaoLogado

    class Usuario {
    <<abstract>>
    - id: int
    - nome: string
    - email: string
    - senha: string
    - tipo: string
    - logado: Boolean
    + realizarLogin(email: string, senha: string): Boolean
    + realizarLogoff(): void
    + visualizarCardapioDoDia(): Cardapio
    + confirmarLogin(email: string): Boolean
    + redefinirSenha(email: string): Boolean
    + verificarConfirmacao(email: string): Boolean
    }

    class Banco de Dados {
    + validarDadosDB(email: string, senha: string) : Boolean
    }

    class handleValidacao {
    + autenticar(): Boolean
    + validarDados(email: string, senha: string) : Boolean
    }
    
    class Administrador {
    - tipo: string = "Administrador"
    + criarCardapio(cardapio: Cardapio): void
    + editarCardapio(cardapio: Cardapio): void
    + excluirCardapio(cardapio: Cardapio): void
    + listarCardapios(): List<Cardapio>
    + criarConta(usuario: Usuario): void
    + editarConta(usuario: Usuario): void
    + excluirConta(usuario: Usuario): void
    + listarContas(): List<Usuario>
    + gerarRelatorioDeConsumo(): Relatorio
    + monitorarDesperdicio(): void
    }

    class Nutricionista {
    - tipo: string = "Nutricionista"
    + criarItemEstoque(item: Estoque): void
    + editarItemEstoque(item: Estoque): void
    + excluirItemEstoque(item: Estoque): void
    + listarItensEstoque(): List<Estoque>
    + visualizarRelatorioDesperdicioEEstoque(): Relatorio
    + registrarPreparoEDistribuicao(refeicao: PreparoDistribuicaoRefeicao): void
    }

    class Gestor {
    - tipo: string = "Gestor"
    + criarCardapio(cardapio: Cardapio): void
    + editarCardapio(cardapio: Cardapio): void
    + excluirCardapio(cardapio: Cardapio): void
    + listarCardapios(): List<Cardapio>
    + criarConta(usuario: Usuario): void
    + editarConta(usuario: Usuario): void
    + excluirConta(usuario: Usuario): void
    + listarContas(): List<Usuario>
    + visualizarRelatorioDesperdicioEEstoque(): Relatorio
    + registrarPreparoEDistribuicao(refeicao: PreparoDistribuicaoRefeicao): void
    + gerarRelatorioDeConsumo(): Relatorio
    + monitorarDesperdicio(): void
    }

    class FuncionarioRefeitorio {
    - tipo: string = "FuncionarioRefeitorio"
    + registrarPreparoEDistribuicao(refeicao: PreparoDistribuicaoRefeicao): void
    }

    class UsuarioNaoLogado {
    - tipo: string = "UsuarioNaoLogado"
    }

    class Cardapio {
    - id: int
    - nome: string
    - dataInicio: Date
    - dataFim: Date
    - alimentos: List<Refeicao>
    + adicionarRefeicao(refeicao: Refeicao): void
    + removerRefeicao(refeicao: Refeicao): void
    }

    class Alimento {
    - id: int
    - nome: string
    - quantidade: int
    }

    class Estoque {
    - id: int
    - alimento: Alimento
    - quantidade: int
    + atualizarQuantidade(novaQuantidade: int): void
    }

    class Relatorio {
    - id: int
    - tipo: string
    - dataInicio: Date
    - dataFim: Date
    - dados: string
    + gerarDados(): void
    }

    class PreparoDistribuicaoRefeicao {
    - id: int
    - data: Date
    - quantidadePreparada: int
    - quantidadeDistribuida: int
    - cardapio: Cardapio
    + atualizarQuantidades(preparada: int, distribuida: int): void
    }

    class Refeicao {
    - id: int
    - nome: string
    - alimentos: List<Alimento>
    + adicionarAlimento(alimento: Alimento): void
    + removerAlimento(alimento: Alimento): void
    }

    Usuario "1" o-- "0..*" Relatorio : gera
    Usuario "1" o-- "0..*" PreparoDistribuicaoRefeicao : registra
    Administrador "1" o-- "0..*" Cardapio : gerencia
    Administrador "1" o-- "0..*" Estoque : gerencia
    Administrador "1" o-- "0..*" Relatorio : gerencia
    Gestor "1" o-- "0..*" Cardapio : gerencia
    Gestor "1" o-- "0..*" Estoque : gerencia
    Gestor "1" o-- "0..*" Relatorio : gerencia
    Nutricionista "1" o-- "0..*" Estoque : gerencia
    Nutricionista "1" o-- "0..*" Relatorio : visualiza
    FuncionarioRefeitorio "1" o-- "0..*" PreparoDistribuicaoRefeicao : registra
    UsuarioNaoLogado "1" o-- "0..*" Cardapio : visualiza

