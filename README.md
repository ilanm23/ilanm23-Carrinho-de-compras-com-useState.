Entregável 3 – Interatividade e useState
Desenvolvimento de Interfaces Dinâmicas e Reativas
1. Sobre o projeto

Este projeto consiste no desenvolvimento de um carrinho de compras interativo utilizando React, JavaScript e Tailwind CSS.

O objetivo é praticar o gerenciamento de estados com useState, a manipulação de arrays, a imutabilidade dos dados e a interação com o usuário.

2. Tecnologias utilizadas
React
Vite
JavaScript
Tailwind CSS
HTML5
CSS3
3. Funcionalidades desenvolvidas
Contador interativo utilizando useState.
Listagem de produtos com nome e preço.
Adição de produtos ao carrinho.
Remoção de produtos do carrinho.
Atualização automática do valor total.
Feedback visual ao adicionar produtos.
Formulário de checkout.
Validação do campo nome com mensagem de erro e borda vermelha.
4. Gerenciamento de estado com useState

O hook useState foi utilizado para controlar o contador, os produtos do carrinho e os dados do formulário.

Para adicionar produtos, foi utilizado o spread operator:

jsx
setCarrinho([...carrinho, produto])


Para remover produtos, foi utilizado o método filter.

O valor total da compra é calculado utilizando reduce.

5. Reflexão

Por que não devemos mutar o estado diretamente (ex: carrinho.push(item)) e qual a importância do spread operator ([...carrinho, item]) no React?

No React, não devemos modificar o estado diretamente porque isso pode impedir que o React identifique corretamente as alterações e atualize a interface.

Por exemplo, utilizar carrinho.push(item) modifica o array original, sem criar uma nova referência.

O spread operator (...) permite criar um novo array contendo os elementos anteriores e o novo item, como em [...carrinho, item].

Dessa forma, o React consegue identificar a mudança de estado e atualizar a interface corretamente.

Portanto, utilizar a imutabilidade é importante para manter o código organizado, previsível e garantir o funcionamento adequado da renderização dos componentes.

6. Como executar o projeto

Instale as dependências:

bash
npm install


Inicie o servidor:

bash
npm run dev

7. Conclusão

Com este projeto, foi possível compreender melhor o funcionamento do useState, a atualização de estados, a imutabilidade dos dados e a criação de interfaces interativas utilizando React e Tailwind CSS.