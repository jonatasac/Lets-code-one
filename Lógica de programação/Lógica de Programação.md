# Lógica de Programação

## [Parte I: Crie programas com Javascript e HTML](https://cursos.alura.com.br/course/logica-programacao-javascript-html)

> Professor: [Flavio Henrique de Souza Almeida](https://cursos.alura.com.br/user/flavio-almeida) | [Linkedin](https://www.linkedin.com/in/fl%C3%A1vio-henrique-almeida-a6315747/)
>
- Dê seus primeiros passos de maneira prática!
- Inicie na programação com JavaScript no seu Navegador
- Entenda variáveis e seu uso
- Repita tarefas com laços, loops, fors e whiles
- Mostre seus programas para seus colegas

### [Comece a programar hoje ](https://cursos.alura.com.br/course/logica-programacao-javascript-html/section/4172/tasks)

#### Converse com seu navegador

Assim como em qualquer profissão, o programador precisa de ferramentas para que possa exercer esta função. Uma delas é o próprio navegador, o browser que você costuma utilizar para navegar na web. Podem ser utilizados o Edge, o Firefox, Chrome, no caso, utilizarei o **Google Chrome**.

Browser é uma ferramenta de desenvolvimento, basta olharmos para qualquer página e percebermos que tudo que está ali é resultado do trabalho de programação de algum indivíduo. No caso, observaremos a página inicial da [Alura](https://www.alura.com.br/). Alguém elaborou um conjunto de instruções, que ao serem interpretadas pelo navegador, exibiu uma página para nós.

Ao clicarmos na página e utilizarmos o atalho "Ctrl + U", veremos o conjunto de instruções, os códigos que foram escritos para gerar tudo que foi feito, que foi pensado por uma equipe de desenvolvedores:

![imagem do código](https://s3.amazonaws.com/caelum-online-public/440+-+L%C3%B3gica+de+Programa%C3%A7%C3%A3o/Aula+01/01.01_001_imagem-do-codigo.png)

Além do browser, será necessário utilizarmos algum **editor de texto**, pode ser um simples, que já vem no sistema operacional. Entretanto, caso seja usuário do **OS Windows**, é interessante utilizar algum outro, como o [NotePad++](https://notepad-plus-plus.org/downloads/v7.9.5/), ou o [Sublime](https://www.sublimetext.com/3). No meu caso, utilizarei o [Visual Studio Code](https://code.visualstudio.com/) e [Typora](https://typora.io/) para anotações.

> Como falava o antigo filósofo Aristóteles: bem começado, metade feito. Sucesso e bom estudo!

O Chrome, a partir da versão 55, passou a detectar automaticamente o *encoding* dos arquivos. Então, é possível pensar que não é mais necessária a tag `<meta charset="UTF-8">`.

No entanto, ela deve continuar a ser usada, porque nem todos os navegadores detectam o *encoding* automaticamente, sendo assim, é uma boa prática manter a tag `<meta>` indicando o `charset` usado na hora de criar o arquivo.

#### Criando seu próprio arquivo HTML

Tendo o arquivo, é importante a inserção do `.html`, por esta ser a linguagem que o navegador entende e, ao utilizarmos a extensão, estamos orientando-o sobre qual deve ser a interpretação do arquivo por parte do navegador e do sistema operacional.

Quando digitamos em nosso editor de texto, no código-fonte ou origem, pulamos duas linhas, entretanto, ao exibir no navegador, isto é ignorado completamente, e as frases são exibidas lado a lado.

Por que isso acontece?

A primeira coisa que precisamos entender é que o navegador está preparado para ler código **HTML**. Ele não sabe que, ao pularmos a linha com a tecla "Enter", ainda que sejam várias vezes, ele deve pular linhas. Tentaremos colocar quantas linhas quisermos entre as duas frases, e recarregar a página utilizando o botão "Recarregar", logo ao lado da barra onde se digita o endereço no navegador:

A ideia é que precisamos utilizar um comando especial, que o HTML tenha preparado, para pular linhas, no caso o `<br>`

Trata-se de uma *tag* HTML, e todas têm esta característica de começar com o símbolo de "menor" (**`<`**), o nome da tag - "br" é abreviação de *break* -, e fecha com o símbolo de "maior" (**`>`**). Isto indica ao navegador que ele deve pular uma linha.

É esta a primeira tag HTML que aprendemos, para pular linhas. Como estamos criando o programa, geraremos uma área de destaque que exibe a mensagem "Meu primeiro teste!".

O **HTML** conta com a tag `<h1>`. O "h" se origina da palavra *heading*, ou seja, cabeçalho. Significa que este é o primeiro título, ou título principal é algo que precisa ser destacado em uma página.

Uma particularidade da tag `<br>` é que, no início, inserimos `<>` e pronto - já para a tag `<h1>` e a maioria das tags HTML, precisaremos da mesma tag com uma barra `</h1>` para fechá-la.

#### Dê olá ao mundo

`<a>` - Tag usada de **âncora**, representada pela letra a. Por meio do atributo `href`, indicaremos o endereço web, ficando: `<a href="http://www.alura.com.br">aqui</a>`

O problema do código que escrevemos é que, apesar de interessante, o HTML é estático, isto é, não é dinâmico. E se quisermos que o HTML, em vez de pular poucas linhas, pule dez, quinze, ou vinte? Teremos que abrir o arquivo HTML e inserir diversas *tags* do tipo `<br>`.

Assim, sempre que quisermos aumentar ou diminuir o número de quebras de linha teremos que remover ou adicionar as *tags* `<br>`, sempre modificando o documento. Como ele é estático, não é possível, por exemplo, exibir um contador na tela com a passagem das horas, tampouco será possível capturar as informações do usuário.

Para que possamos de fato programar, precisaremos utilizar uma outra linguagem. O navegador é poliglota, e "fala" algumas linguagens além de HTML, sendo capaz de trabalhar com uma linguagem verdadeiramente de programação, que é o **JavaScript**.

<center> Neste treinamento, aprenderemos a lógica de programação utilizando a linguagem <b>JavaScript</b>. </center>

