# Sistema de Controle de Refeitório Escolar

## UC014. Visualizar Relatórios de Desperdício e Estoque
Este caso de uso descreve as etapas percorridas pelo Gestor para visualizar os relatórios de desperdício de alimentos e de estoque no sistema.

## Atores
💼 Gestor

## Condições
### Pré-condições
O Gestor deve estar autenticado no sistema.

### Pós-condições
Os relatórios de desperdício e estoque foram visualizados com sucesso.

## Cenário principal
### Ações do ator (💼 ) e Ações do sistema (⚙️)
1. 💼 Seleciona a opção de "Relatórios" no menu principal.
2. ⚙️ Exibe as opções de "Relatório de Desperdício" e "Relatório de Estoque".
3. 💼 Escolhe entre "Relatório de Desperdício" ou "Relatório de Estoque".
4. ⚙️ Exibe os filtros disponíveis (período, tipo de alimento, etc.).
5. 💼 Aplica os filtros desejados.
6. ⚙️ Gera o relatório baseado nos filtros aplicados.
7. ⚙️ Exibe o relatório solicitado, mostrando os dados de desperdício ou estoque detalhados.
8. 💼 Visualiza o relatório gerado.
9. 💼 (Opcional) Escolhe a opção de exportar o relatório em formato PDF ou Excel.

## Restrições e validações
1. Os filtros de período devem ser preenchidos corretamente, com datas válidas e lógicas.
2. O Gestor deve ter permissão para visualizar os relatórios de desperdício e estoque.


## Cenários alternativos
Cenário alternativo 1 – Falta de dados para o período selecionado
1.⚙️ Identifica que não há dados disponíveis para o período ou filtros aplicados.
  1.1. ⚙️ Exibe uma mensagem informando que não há dados disponíveis para o critério selecionado.
  1.2  💼 Modifica os filtros e repete a busca.
  1.3  ⚙️ Retorna ao passo 5 do cenário principal.
Cenário alternativo 2 – Erro na geração do relatório
1.⚙️ Encontra um erro ao tentar gerar o relatório.
  1.1. ⚙️ Exibe uma mensagem de erro informando que ocorreu um problema na geração do relatório.
  1.2  💼 Retorna ao passo 4 do cenário principal para tentar novamente ou reporta o problema ao suporte.
  
## Exceções
Não se aplica.