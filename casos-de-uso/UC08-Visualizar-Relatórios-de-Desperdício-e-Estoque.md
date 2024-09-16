# Sistema de Controle de Refeitório Escolar

## UC08. Visualizar Relatórios de Desperdício e Estoque

Este caso de uso descreve as etapas necessárias para que o Gestor ou Nutricionista visualize relatórios de desperdício e estoque no sistema.

### Atores
💼 Gestor
👩‍🍳 Nutricionista

### Condições
#### Pré-condições
- O usuário deve estar logado no sistema.

#### Pós-condições
- O relatório de desperdício e/ou estoque é exibido para o usuário.

### Cenário principal
#### Ações do ator (💼👩‍🍳) e Ações do sistema (⚙️)
1. 💼👩‍🍳 O usuário seleciona a opção para visualizar relatórios de desperdício ou de estoque no menu do sistema.
2. 💼👩‍🍳 O usuário escolhe o tipo de relatório desejado (desperdício, estoque ou ambos).
3. 💼👩‍🍳 O usuário seleciona as datas que deseja gerar.
4. ⚙️ O sistema valida as datas fornecidas e o tipo de relatório selecionado.
5. ⚙️ O sistema gera o relatório baseado nas informações disponíveis no sistema para o período e tipo selecionado.
6. ⚙️ O sistema exibe o relatório na tela.
7. 💼👩‍🍳 O usuário pode optar por exportar o relatório para formatos como PDF ou Excel.
8. ⚙️ O sistema exibe uma mensagem de conclusão, confirmando que o relatório foi exibido e/ou exportado com sucesso.


### Restrições e validações
- Os dados selecionados devem ser válidos. 

### Cenários alternativos
#### Cenário alternativo 1 – Data inválida
1. ⚙️ O sistema detecta data inválida.
   1. ⚙️ O sistema informa ao usuário que as datas selecionadas são inválidas e solicita a correção das datas.
   2. 💼👩‍🍳 O usuário muda os valores.
   3. ⚙️ Retorna ao passo 3 do cenário principal.

### Exceções
### Exceção 1 – Dados indisponíveis
1. ⚙️ O sistema informa que não há dados disponíveis para o período ou tipo de relatório selecionado.
2. ⚙️ O sistema mostra opções para ajustar o período ou tipo de relatório e tentar novamente.
