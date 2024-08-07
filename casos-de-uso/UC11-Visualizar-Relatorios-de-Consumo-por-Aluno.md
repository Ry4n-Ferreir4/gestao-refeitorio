# Sistema de Controle de Refeitório Escolar

## UC11. Visualizar Relatórios de Consumo por Aluno

Este caso de uso descreve as etapas necessárias para que o Gestor visualize relatórios de consumo por aluno.

### Atores
- 💼 Gestor

### Condições
#### Pré-condições
- O Gestor deve estar logado no sistema.

#### Pós-condições
- Não se aplica.

### Cenário principal
#### Ações do ator (💼) e Ações do sistema (⚙️)
1. 💼 O gestor navega até a seção de relatórios gerados.
2. ⚙️ O sistema exibe uma lista de opções de relatórios gerados.
3. 💼 O gestor seleciona a opção de consumo por aluno.
4. 💼 O gestor define os dados do relatório, como:
   1. Tipo de refeição (almoço, lanche, janta);
   2. Tipo de alimento.
   3. Data.
5. ⚙️ O sistema procura relatório com esses dados.
6. ⚙️ O sistema disponibiliza opção de download.
7.  💼 O gestor visualiza e opta por exportar em formatos como PDF ou Excel.
8. ⚙️ O sistema exibe mensagem de conclusão.

### Restrições e validações
- Deve existir um relatório gerado com os dados escolhidos.

### Cenários alternativos
#### Cenário alternativo 1 – Relatório não existente
1. ⚙️ O sistema detecta que não há relatório com os dados definidos.
   1. ⚙️ O sistema informa o usuário.
   2. 💼 O usuário escolhe outros dados.
   3. ⚙️ Retorna ao passo 5 do cenário principal.

### Exceções
Não se aplica.
