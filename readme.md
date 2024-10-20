# Tags HTML

O html deve ser feito de forma a conter o conteudo de forma semantica, sem se preucupar com estilização.

## p

Para conteudo em texto, modo de display inline.
Semantica: paragrafo, conteudo em texto.

## span

Tag que conterá conteudos de qualquer tipo, modo de display inline.
Semantica: none.

## h1, h2, h3, h4, h5 e h6

Para conteudo em texto sendo as headings do site, modo de display inline.
Semantica: Titulos.

## a

Tag para utilização de links, sejam eles locais ou online os recebendo atraves do atributo { href = "link" }, entre as tags de abertura e fechamento se coloca um conteudo no qual o seu click resultará no acesso do link, modo de display inline.
Semantica: Links.

## img

Utilizada para inserir imagens no site, recebendo dois atributos { src="link" alt="para caso a imagem não carrege"}, essa tag é uma tag sem fechamento só tendo a tag de abertura com um / no final, modo de display block.
Semantica: Imagens.

## div

Tag que conterá conteudos de qualquer tipo, utilizada para a organização do site em blocos para melhor posicionamento, modo de display block.
Semantica: None.

## ul

Semantica:Lista não ordenada.

## ol

Semantica: Listas ordenadas.

## dl

Semantica: Lista de definições.
Se defini o elemento com dt.
E abaixo se dá a descrição com dd.

## blockquote

Semantica: Usado para criar uma citação para o conteudo que ele encapsula.
cite = "link".

## q

Semantica: Citação dentro de uma frase, com estilo basico coloca em aspas.
cite = "link".

## cite

Semantica: Para citar o nome de uma obra.

## em

Semantica: Para dar enfasi ao conteudo.

## strong

Semantica: Para dar importancia ao conteudo.

## Meta tag

### viewport

content = "widht=device-width, initial-scale=1"
Essa tag definirá o tamanho da view port e seus nivel de zoom inicial, recebendo as variaveis acima.

# Tags Landmarks HTML

Funcionam como se fosse uma div, contudo com valor semantico.

## aria-label

Serve para dar uma descrição para landmarks, ajuda a dar mais sentido a cada secção.

## aria-labeledby

Recebe o id de alguma tag e o aria-label será a informação que está nesse conteudo, e ele não será repetido duas vezes.

## main

Serve para localizar o conteudo principal do site.

## nav

Serve para envolver uma navegação do site.

## article

Encapsular um conteudo que por si só faz sentido sem o seu entorno.
Cria e não cria landmarks, por si só no html não é um landmark mas nos leitores de tela utiliza como.

## section

Utilizado para agrupar elementos similares.
Não cria landmark;

## aside

Demarca um conteudo complementar ao principal.

## header

Demarca o cabeçalho do site, o banner.
Dentro de outras landmarks se torna o banner somente daquele conteudo.

## footer

Demarca o rodapé do site.
Dentro de outras landmarks se torna o rodapé somente daquele conteudo.

# Unidades

## px

Unidade em pixels.

## rem

Uma unidade que equivale a 16px normalmente, o rem é um valor definido pelo browser/html que ajuda na acessibilidade.

Pode ser alterado utilizando:

html {
font-size: size;
}

## em

Uma unidade que equivale a o font size dos elementos pai.

## ch

Valor da largura da tipografia do caracter 0.

# Tags CSS

Serve para definir a estilização do site.

## background-color

Define a cor do background.

## backgroun-image

define o background como sendo uma imagem, existindo uma repetição infinita dessa imagem.

### linear-gradient

Cria um gradiente linear entre cores.

### radial-gradient

Cria um gradiente radial entre cores.

## background-repeat

Define se o background vai se repetir infinitamente ou não.

## background-size

Define o tamanho da imagem, contain e cover dão uma capacidade de resize boa.

## background-positon

Define o posicionamento do background.

## font-size

Define o tamanho da fonte.

## text-decoration

Define se o texto tem underline, pontos embaixo dentre outros ou não apresenta nenhum desses.

## color

Define a cor do conteudo, geralmente usado para colorir texto.

## font-family

Define o tipo de fonte que será utlizada.

## font-weight

Define o peso da escrita, se a fonte está em negrito ou não falando de uma forma chula, dependendo da fonte talvez não existam alguns peso.

## font-style

O estilo da fonte se está em italico, oblico e etc.

## line-height

A altura da linha do texto.

## text-transform

Altera o texto para maiusculo ou minusculo e outras opções.

## text-indent

A identação do texto.

## text-shadow

Coloca uma sombra no texto, não utilize.

## letter-spacing

Espaçamento entre as letras.

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

## list-style

Define a estilização da lista.

## @media

```css
@media (max-width: 600px) {
  div {
    grid-template-coluns: 1fr;
  }
}
```

Um if dentro do css, muito utilizado para adicionar responsividade no site, utilizando max-width e min-width se pode definir a espressão, tambem se pode utilizar screen, print dentre outros, recebe operadores logicos como and e or.

## object-fit

Serve para o objeto cobrir o conteiner mantendo sua proporção, contudo tende a cortar a imagem se ficar menor.

## object-position

Define como a imagem vai ser cortada em uma situação que ela é diminuida.

## max-width

Define o valor de largura másima de um elemento, abaixo desse valor o objeto é diminuido.
Utilizado em textos para manter eles em um tamanho ideal, se utiliza a unidade ch.

## transition

Faz com que algumas transições de cores e bordas sejam mais suaves, um exemplo seria quando damos hover em um botão.

# Top Right Bottom Left

No caso de algumas estilizações como margin, padding e border, podemos querer valores diferentes em diferentes extremidades do elemento.
Com duas variaveis a aplicação será: margin top/bottom right/left.
Com quatro variaveis a aplicação será: margin top right bottom left.

# Pseudo class

## tag:hover

Altera o elemento quando em cima do elemento.

## tag:focus

Altera o elemento quando o está em foco, quando damos tab e passamos pelo elemento.

## tag:active

Altera o elemento quando foi ativado no caso clicado.

## tag:visited

Altera um link no qual já foi visitado, sobreescreve as outras pseudo classes.

## tag:first-child

Seleciona o primeiro elemento de uma lista ordenada.

## tag:last-child

Seleciona o ultimo elemento de uma lista ordenada.

## tag:nth-child(VALUE)

Seleciona o filho de nume passado pelo valor, tambem se pode usar odd ou even para pares e impares.

## tag:not()

Retira s elementos passados a ele.

# Pseudo element

Vem sem nenhuma estilização ou diplay, então defina quando for utilizar.

## tag::before{}

Cria um conteudo apartir do css antes do elemento.

## tag::after{}

Cria um conteudo apartir do css depois do elemento.

## tag::firstline{}

Estiliza a primeira linha.

## tag::firstletter{}

Estiliza a primeira letra.

## content

Define o conteudo.

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

## Responsividade

```css
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
```

Utilizando repeat e auto-fit com um valor fixo podemos criar responsividade, e com o minmax(valor_fixo, 1 fr); no valor de reapet retiramos o problema de quando tiver mais espaço que o nescessario do valor fixo ele ocupará 1fr.

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

# Responsividade

# img fill grid container

Tendo uma imagem dentro de um grid naturalmente ela nao ocupará todo o espaço por padrão, então envolvemos em uma div com as configurações abaixo.

```css
div {
  display: flex;
  flex-wrap: wrap;
}

div img {
  max-width: 100%;
  height: auto;
  flex: 1 1 auto;
}
```

# hover with tab on the side

```css
tag:hover {
  border-left: 10px solid #c6c6c6;
}
```

# how add border on hover witout jiggle

Defina uma borda no elemento original com cor transparente e no hover coloque a cor.

```css
tag {
  border: 2px solid transparent;
}

tag:hover {
  border: 2px solid #ee2211;
}
```

# alinhar bloco de tamanho maximo definido no centro da tela

Se pode utilizar o margin: 0 auto; com as margens laterais no automatico isso centraliza.
