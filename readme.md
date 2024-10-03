# Tags HTML

## p

Para conteudo em texto, modo de display inline.

## span

Tag que conterá conteudos de qualquer tipo, modo de display inline.

## h1, h2, h3, h4, h5 e h6

Para conteudo em texto sendo as headings do site, modo de display inline.

## a

Tag para utilização de links, sejam eles locais ou online os recebendo atraves do atributo { href = "link" }, entre as tags de abertura e fechamento se coloca um conteudo no qual o seu click resultará no acesso do link, modo de display inline.

## img

Utilizada para inserir imagens no site, recebendo dois atributos { src="link" alt="para caso a imagem não carrege"}, essa tag é uma tag sem fechamento só tendo a tag de abertura com um / no final, modo de display block.

## div

Tag que conterá conteudos de qualquer tipo, utilizada para a organização do site em blocos para melhor posicionamento, modo de display block.

# Tags CSS

## background

Define a cor do background.

## font-size

Define o tamanho da fonte.

## text-decoration

Define se o texto tem underline, pontos embaixo dentre outros ou não apresenta nenhum desses.

## color

Define a cor do conteudo, geralmente usado para colorir texto.

## font-family

Define o tipo de fonte que será utlizada.

## display

Define como o elemento será exibido inline, block, inlien-block e etc.

## width e height

Definem a largura e a altura de um elemento respectivamente.

## margin

Adiciona margem a elementos.

## padding

Adiciona padding a elementos.

## border

Adiciona uma borda a os elementos, border: size style color;.

## border-width

Define a largura da borda já colocada.

## text-align

Define o alinhamento do texto justificado, centralizado e etc.

## border-radius

Adiciona uma borda arredondada recebendo o raio da borda.

# Top Right Bottom Left

No caso de algumas estilizações como margin, padding e border, podemos querer valores diferentes em diferentes extremidades do elemento.
Com duas variaveis a aplicação será: margin top/bottom right/left.
Com quatro variaveis a aplicação será: margin top right bottom left.

# Id e Class

## Id

Tags podem receber um id unico assim alterando o seu estilo, a tag receberá id="nome_do_id", e o id será definido no css por #nome_do_id { estilização }.

## Class

Tags podem receber varias classes alterando o seu estilo, a tag receberá class="classe1 classe2" assim recebendo os estilos de cada classe, a classe no css por .nome_da_classe { estilização }.

## Estilização Sem Id ou Class

Se pode adicionar estilos a uma tag declarando no css nome_da_tag { estilização }, tambem podemos aplicar em somente em tags que estejam dentro de outras tags, exemplo div p { estilização }, assim estariamos aplicando somente aos p's dentro de div's.
Tambem se pode colocar a estilização dentro da tag de abertura, contudo isso não é recomendavel.

# Inline

Elementos inline utilizarão somente o espaço nescessário para a sua exibição, não recebendo estilização de tamanho ou posicionamento.

# Block

Elementos block utilizão de parametros passados pelo css para definir sua exibição.

# inline-block

Utilizado para que elementos inline recebam estilização de tamanho e posicionamento.

# grid item

Um grid item tem um container definido para sí, que inclui o tamanho de margin, e os elementos dependendo da sua natureza iram ou não praencher todo o conteiner.

# grid

Modo de exibição dos itens em Grid, assim dando tornando seus itens em grid items.
Defina display: grid;

## grid-template-columns

Define os espaçamentos de cada coluna com grid-template-columns: 1fr 1fr;
Não utilize porcentagem para definir o tamanho das colunas, utilize fr que é uma medida que pega o restante de tamanho e divide de acordo com os pesos.

## gap

Define o gap entre os elementos, se houver margin nesses elementos irá somar a elas.

## align-content e justify-content

O align-content define o alinhamento dos conteudos na vertical.
O justify-content define o alinhamento dos conteudos na horizontal.
Nescessita ter o espaço para fazer o alinhamento.
space-evenly, space-around, space-between.

## place-content

Uma tag que define as duas acima, recebendo dois atributos, o primeiro sendo o align-content e o segundo justify-content, se só passar um irá aplicar para os dois.

## grid-column

Usada nos elementos para definar em quais colunas elesocuparão, se receber uma variavel ele ocupará uma coluna e aquela coluna passada será sua inicial, contudo podemos passar o aonde queremos que o elelemento começe e termine, separando os atributos por barra, grid-column: 1 / -1, -1 serve para referenciar até a ultima.

## align-items e justify-items

O align-items define o alinhamento dos items na vertical.
O justify-items define o alinhamento dos items na horizontal.
Dentro do grid um conteiner de um item tem efeito sobre o tamanho de seus adjacentes, assim podendo aumenta-los ou diminui-los, assim podemos alinhar os itens entre sí, para que os items sejam alinhados no centro um do outros start, end e etc.

## place-items

Uma tag que define as duas acima, recebendo dois atributos, o primeiro sendo o align-items e o segundo justify-items, se só passar um irá aplicar para os dois.

## align-self e justify-self

O align-self define o alinhamento do elemento na vertical.
O justify-self define o alinhamento do elemento na horizontal.
Essas tag são dadas aos elementos dentro do grid não ao grid, e definem como os elementos se posicionarão dentro do conteiner delas

## place-self

Uma tag que define as duas acima, recebendo dois atributos, o primeiro sendo o align-items e o segundo justify-items, se só passar um irá aplicar para os dois.

## grid-template-rows

Define os espaçamentos de cadalinha com grid-template-rows: 1fr 1fr;
Não utilize porcentagem para definir o tamanho das linha, utilize fr que é uma medida que pega o restante de tamanho e divide de acordo com os pesos.

## grid-auto-rows

Defini os espaçamentos das linhas nas quais não s~ao definidas pelo programador.

## grid-row

Similar ao grid-column mas para as linhas ao inves de colunas

## grid-area

Define o grid-column e grid-row no mesmo atributo, grid-area: column / row;

# flex

Defina display: flex;
Maioria dos comandos de grid funcionam no flexbox

## flex-wrap

Define se os conteudos vão ser distribuidos em varias linhas ou se vão quebrar o conteudo para caber em uma tela que não cabem.

## flex-grow

Defini se o elemento deve crescer para ocupar o espaço em branco, 0 impede o crescimento e valores acima haverá crecimento.

## flex-basis

Valor inicial antes de distribuir o espaço.

## flex-shrink

Caso exista um valor base ele determinará se o elemento pode ser reduzido ou não, 0 significa que não pode ser reduzido.

## flex

flex: 1; atalho para flex-grow: 1; flex-shrink: 1; flex-basis: 0;

# Positions

Servem para posicionar os elementos de mais formas.
Defina position: Type;
Tag usuais são top, bottom, right, left.

## fixed

Deixa o elemento preso em uma posição da tela sem ser afetado pelo scroll, exemplo aquelas barras de cookies em sites.

## relative

O elemento pode ser alterado apartir do ponto no qual ele estavá originalmente, ele ainda ocupará o espaço que ele ocuparia sem as mudanças do posicionamento.

## absolute

Se ele não tiver um elemento pai com position: relative; ele tratará seu ponto de origem sendo o top left, se ele tiver um elemento pai configura com relative ele tratará sua posição original como seu ponto de origem.

## z-index

Define a sobreposição de elementos, qual irá ficar por cima e qual por baixo, naturalmento o html segue a ordem no qual as tags foram escritas, contudo utilizando z-index podemos ter um controle sobre isso, o elemento de valor maior ficará no topo e o de menor abaixo.
