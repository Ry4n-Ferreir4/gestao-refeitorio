# Sistema de Controle de Refeitório Escolar

## UC07. Gerar relatórios de consumo e desperdício.

Este caso de uso descreve as etapas percorridas pelo Gestor e Administrador para gerar relatórios de consumo e desperdício.

### Atores
- 💼 Gestor
- 👨‍💼 Administrador

### Condições
#### Pré-condições
O ator deve estar logado no sistema.

#### Pós-condições
O relatório foi gerado com sucesso.

### Cenário principal
#### Ações do ator (💼👨‍💼) e Ações do sistema (⚙️)
1. 💼👨‍💼 O usuário seleciona a data a partir da qual deseja iniciar e a data que deseja encerrar o relatório.
2. 💼👨‍💼 O usuário seleciona a refeição desejada pro relatório (café da manhã, almoço, jantar, dia completo).
3. ⚙️ O sistema formula o relatório baseado nas informações disponíveis no sistema.
4. ⚙️ O sistema exibe o relatório e disponibiliza opção de download.
5. 💼👨‍💼 O usuário visualiza e opta por exportar em formatos como PDF ou Excel.
6. ⚙️ O sistema exibe mensagem de conclusão.

### Restrições e validações
1. Os campos de data devem ser preenchidos corretamente, sendo utilizado apenas datas válidas (datas que não são feriados, finais de semana ou datas que ainda não aconteceram).
2. O campo de refeições não pode estar vazio.

### Cenários alternativos
#### Cenário alternativo 1 – Data inválida
1. ⚙️ O sistema detecta que a data selecionada não é válida (por exemplo: feriado, fim de semana, data que nao ocorreu ainda).
   1. ⚙️ O sistema nforma ao Gestor que a data selecionada não é válida.
   2. 💼👨‍💼 O usuário seleciona uma nova data.
   3. ⚙️ O sistema retorna ao passo 3 do cenário principal.

### Exceções
Não se aplica.
