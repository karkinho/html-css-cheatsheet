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

# Top Right Bottom Left

No caso de algumas estilizações como margin, padding e border, podemos querer valores diferentes em diferentes extremidades do elemento.
Com duas variaveis a aplicação será: margin top/bottom right/left.
Com quatro variaveis a aplicação será: margin top right bottom left.

# Id e Class

## Id

Tags podem receber um id unico assim alterando o seu estilo, a tag receberá id="nome_do_id", e o id será definido no css por .nome_do_id { estilização }.

## Class

Tags podem receber varias classes alterando o seu estilo, a tag receberá class="classe1 classe2" assim recebendo os estilos de cada classe, a classe no css por #nome_da_classe { estilização }.

## Estilização Sem Id ou Class

Se pode adicionar estilos a uma tag declarando no css nome_da_tag { estilização }, tambem podemos aplicar em somente em tags que estejam dentro de outras tags, exemplo div p { estilização }, assim estariamos aplicando somente aos p's dentro de div's.
Tambem se pode colocar a estilização dentro da tag de abertura, contudo isso não é recomendavel.

# Inline

Elementos inline utilizarão somente o espaço nescessário para a sua exibição, não recebendo estilização de tamanho ou posicionamento.

# Block

Elementos block utilizão de parametros passados pelo css para definir sua exibição.

# inline-block

Utilizado para que elementos inline recebam estilização de tamanho e posicionamento.
