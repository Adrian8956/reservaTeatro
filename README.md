
---

# Sistema de Reservas de Teatro

## Visão Geral

Este projeto implementa um sistema simples de reserva de assentos de teatro utilizando HTML, CSS e JavaScript. Os usuários podem selecionar e reservar assentos, que são então marcados como reservados e salvos no armazenamento local até serem confirmados.

## Funcionalidades

- Exibe 240 assentos em formato de grade.
- Os assentos são inicialmente exibidos como disponíveis ou ocupados com base nos dados armazenados localmente.
- Os usuários podem selecionar um assento para reservá-lo, marcando-o temporariamente como reservado.
- Ao confirmar, os assentos reservados são marcados como ocupados permanentemente e salvos no armazenamento local.
- Validação básica garante que apenas números de assentos válidos possam ser reservados.

## Uso

1. **Carregamento da Página:**
   - Quando a página é carregada, os assentos são exibidos com sua disponibilidade atual baseada nos dados do armazenamento local.

2. **Reservando um Assento:**
   - Clique em qualquer assento disponível para marcá-lo como reservado.
   - Uma vez reservado, a imagem do assento muda para indicar que está temporariamente reservado.

3. **Confirmação das Reservas:**
   - Após selecionar os assentos, clique no botão "Confirmar Reservas".
   - Os assentos reservados são marcados como ocupados permanentemente, e o armazenamento local é atualizado.

4. **Recarregando a Página:**
   - Ao recarregar a página, os assentos reservados anteriormente permanecem marcados como ocupados.

## Arquivos

- **index.html**: Contém a estrutura e os elementos básicos de UI.
- **styles.css**: Fornece estilização mínima para a grade de assentos do teatro.
- **script.js**: Implementa a funcionalidade de reserva de assentos, atualizações de status e manipulação do armazenamento local.

## Detalhes de Implementação

- Os assentos são criados dinamicamente com base em uma constante (`POLTRONAS = 240`).
- A disponibilidade de cada assento é gerenciada através do JavaScript e refletida no DOM.
- O armazenamento local (`teatroOcupadas`) é utilizado para persistir o estado dos assentos ocupados entre atualizações da página.

## Dependências

- Este projeto não requer bibliotecas ou frameworks externos.
- Imagens (`img/ocupada.jpg`, `img/disponivel.jpg`, `img/reservada.jpg`) são utilizadas para representar os estados dos assentos.

## Contribuições

- Contribuições são bem-vindas através de pull requests.
- Para mudanças significativas, abra primeiro um problema para discutir o que você gostaria de alterar.

---
