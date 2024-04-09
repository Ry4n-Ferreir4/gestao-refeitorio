# Sistema de Controle de Refeitório Escolar

## UC01. Cadastrar Cardápio do Dia

Este caso de uso descreve as etapas percorridas pelo Gestor para gerar relatórios de consumo e desperdício.

### Atores
- 💼 Gestor

### Condições
#### Pré-condições
Não se aplica.

#### Pós-condições
O relatório foi gerado com sucesso.

### Cenário principal
#### Ações do ator (💼) e Ações do sistema (⚙️)
1. 💼 Seleciona a data a partir da qual deseja iniciar e a data que deseja encerrar o relatório.
2. 💼 Seleciona a refeição desejada pro relatório (café da manhã, almoço, jantar, dia completo).
3. ⚙️ Formula o relatório baseado nas informações disponíveis no sistema.
4. ⚙️ Exibe o relatório e disponibiliza para baixar como PDF.

### Restrições e validações
1. Os campos de data devem ser preenchidos corretamente, sendo utilizado apenas datas válidas (datas que não são feriados, finais de semana ou datas que ainda não aconteceram).
2. O campo de refeições não pode estar vazio.

### Cenários alternativos
#### Cenário alternativo 1 – Data inválida
1. ⚙️ Identifica que a data selecionada não é válida (por exemplo: feriado, fim de semana, data que nao ocorreu ainda).
   1. ⚙️ Informa ao Gestor que a data selecionada não é válida.
   2. 💼 Seleciona uma nova data.
   3. ⚙️ Retorna ao passo 1 do cenário principal.

### Exceções
Não se aplica.
