# Flex Container

O flex container é a teg que envolve os intens flex, ao dicar display: flex, essa tag passa a ser um flex container

## Display

`display: flex;`

Define o elemento como um flex container, tornando os seus filhos flex-itens.


## flex-direction

Define a direção dos flex itens. Por padrão ele é row (linha), por isso quando o display: flex; é adicionado, os elementos ficam em linha, um do lado do outro.

A mudança de row para column geralmente acontece quando estamos definindo os estilos em media queries para o mobile. Assim você garante que o conteúdo seja apresentado em coluna única.

`flex-direction: row;`
 Os itens ficam em linha

`flex-direction: row-reverse;`
 Os itens ficam em linha reversa, ou seja 3, 2, 1.

`flex-direction: column;`
 Os itens ficam em uma única coluna, um embaixo do 
 outro.

`flex-direction: column-reverse;`
 Os itens ficam em uma única coluna, um embaixo do outro, porém em ordem reversa: 3, 2 e 1.


 ## flex-wrap

 Define se os itens devem quebrar ou não a linha. Por padrão eles não quebram linha, isso faz com que os flex itens sejam compactados além do limite do conteúdo.

Essa é geralmente uma propriedade que é quase sempre definida como flex-wrap: wrap; Pois assim quando um dos flex itens atinge o limite do conteúdo, o último item passa para a coluna debaixo e assim por diante.

`flex-wrap: nowrap;`
Valor padrão, não permite a quebra de linha.

`flex-wrap: wrap;`
Quebra a linha assim que um dos flex itens não puder mais ser compactado.

`flex-wrap: wrap-reverse;`
Quebra a linha assim que um dos flex itens não puder mais ser compactado. A quebra é na direção contrária, ou seja para a linha acima.


## flex-flow

O flex-flow é um atalho para as propriedades flex-direction e flex-wrap. Você não verá muito o seu uso, pois geralmente quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

E quando mudamos o flex-wrap para wrap, mantemos o padrão do flex-direction que é row.

`flex-flow: row nowrap;`
Coloca o conteúdo em linha e não permite a quebra de linha.

`flex-flow: row wrap;`
Coloca o conteúdo em linha e permite a quebra de linha.

`flex-flow: column nowrap;`
Coloca o conteúdo em coluna e não permite a quebra de linha.