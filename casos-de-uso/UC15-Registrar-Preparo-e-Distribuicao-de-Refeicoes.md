# Sistema de Controle de Refeitório Escolar

## UC012. Visualizar Cardápio do Dia
Este caso de uso descreve as etapas percorridas pelo usuário (aluno, funcionário, gestor, Administrador) para visualizar o cardápio do dia no sistema.

## Atores
👤 Usuário não Logado
👷 Funcionários do Refeitório
👩‍🍳 Nutricionista
💼 Gestor
## Condições
### Pré-condições
Não se aplica
### Pós-condições
O cardápio do dia foi visualizado com sucesso.

## Cenário principal
### Ações do ator (👤 / 👷 / 💼 / 👩‍🍳 ) e Ações do sistema (⚙️)
1. 👤 / 👷 / 💼 / 👩‍🍳  Seleciona a opção "Visualizar Cardápio do Dia" no menu principal.
2. ⚙️ Exibe os cardápios completo do dia, incluindo as refeições (Lanche da manhã, almoço, lanche da tarde, jantar) e as opções de alimentos disponíveis em cada refeição.
3. 👤 / 👷 / 💼 / 👩‍🍳 Visualiza o cardápio detalhado, com informações sobre os pratos, ingredientes, e possíveis alertas de alérgenos.
4. ⚙️ Exibe o cardápio correspondente ao período selecionado.
## Restrições e validações
1. O cardápio deve ser atualizado diariamente pelo sistema, com base nas informações fornecidas pelo Nutricionista.


## Cenários alternativos
Cenário alternativo 1 –  Cardápio não disponível
1.⚙️ Identifica que o cardápio do dia ainda não foi disponibilizado ou atualizado.
  1.1. ⚙️ Exibe uma mensagem informando que o cardápio do dia ainda não está disponível.
  1.2  👤 / 👷 / 💼 / 👩‍🍳  Aguarda a disponibilização do cardápio ou retorna ao menu principal.

  
## Exceções
1.⚙️ Identifica uma falha ao tentar carregar o cardápio do dia.
  1.1. ⚙️ Exibe uma mensagem de erro informando sobre a falha.
  1.2  👤 / 👷 / 💼 / 👩‍🍳 Pode optar por tentar recarregar a página ou reportar o problema ao suporte.
  1.3  ⚙️ Tenta carregar novamente o cardápio ou retorna ao menu principal.