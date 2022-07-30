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

#### 1. Converse com seu navegador

Assim como em qualquer profissão, o programador precisa de ferramentas para que possa exercer esta função. Uma delas é o próprio navegador, o browser que você costuma utilizar para navegar na web. Podem ser utilizados o Edge, o Firefox, Chrome, no caso, utilizarei o **Google Chrome**.

Browser é uma ferramenta de desenvolvimento, basta olharmos para qualquer página e percebermos que tudo que está ali é resultado do trabalho de programação de algum indivíduo. No caso, observaremos a página inicial da [Alura](https://www.alura.com.br/). Alguém elaborou um conjunto de instruções, que ao serem interpretadas pelo navegador, exibiu uma página para nós.

Ao clicarmos na página e utilizarmos o atalho "Ctrl + U", veremos o conjunto de instruções, os códigos que foram escritos para gerar tudo que foi feito, que foi pensado por uma equipe de desenvolvedores:

![imagem do código](https://s3.amazonaws.com/caelum-online-public/440+-+L%C3%B3gica+de+Programa%C3%A7%C3%A3o/Aula+01/01.01_001_imagem-do-codigo.png)

Além do browser, será necessário utilizarmos algum **editor de texto**, pode ser um simples, que já vem no sistema operacional. Entretanto, caso seja usuário do **OS Windows**, é interessante utilizar algum outro, como o [NotePad++](https://notepad-plus-plus.org/downloads/v7.9.5/), ou o [Sublime](https://www.sublimetext.com/3). No meu caso, utilizarei o [Visual Studio Code](https://code.visualstudio.com/) e [Typora](https://typora.io/) para anotações.

> Como falava o antigo filósofo Aristóteles: bem começado, metade feito. Sucesso e bom estudo!

O Chrome, a partir da versão 55, passou a detectar automaticamente o *encoding* dos arquivos. Então, é possível pensar que não é mais necessária a tag `<meta charset="UTF-8">`.

No entanto, ela deve continuar a ser usada, porque nem todos os navegadores detectam o *encoding* automaticamente, sendo assim, é uma boa prática manter a tag `<meta>` indicando o `charset` usado na hora de criar o arquivo.

#### 2. Criando seu próprio arquivo HTML

Tendo o arquivo, é importante a inserção do `.html`, por esta ser a linguagem que o navegador entende e, ao utilizarmos a extensão, estamos orientando-o sobre qual deve ser a interpretação do arquivo por parte do navegador e do sistema operacional.

Quando digitamos em nosso editor de texto, no código-fonte ou origem, pulamos duas linhas, entretanto, ao exibir no navegador, isto é ignorado completamente, e as frases são exibidas lado a lado.

Por que isso acontece?

A primeira coisa que precisamos entender é que o navegador está preparado para ler código **HTML**. Ele não sabe que, ao pularmos a linha com a tecla "Enter", ainda que sejam várias vezes, ele deve pular linhas. Tentaremos colocar quantas linhas quisermos entre as duas frases, e recarregar a página utilizando o botão "Recarregar", logo ao lado da barra onde se digita o endereço no navegador:

A ideia é que precisamos utilizar um comando especial, que o HTML tenha preparado, para pular linhas, no caso o `<br>`

Trata-se de uma *tag* HTML, e todas têm esta característica de começar com o símbolo de "menor" (**`<`**), o nome da tag - "br" é abreviação de *break* -, e fecha com o símbolo de "maior" (**`>`**). Isto indica ao navegador que ele deve pular uma linha.

É esta a primeira tag HTML que aprendemos, para pular linhas. Como estamos criando o programa, geraremos uma área de destaque que exibe a mensagem "Meu primeiro teste!".

O **HTML** conta com a tag `<h1>`. O "h" se origina da palavra *heading*, ou seja, cabeçalho. Significa que este é o primeiro título, ou título principal é algo que precisa ser destacado em uma página.

Uma particularidade da tag `<br>` é que, no início, inserimos `<>` e pronto - já para a tag `<h1>` e a maioria das tags HTML, precisaremos da mesma tag com uma barra `</h1>` para fechá-la.

#### 3. Dê olá ao mundo

`<a>` - Tag usada de **âncora**, representada pela letra a. Por meio do atributo `href`, indicaremos o endereço web, ficando: `<a href="http://www.alura.com.br">aqui</a>`

O problema do código que escrevemos é que, apesar de interessante, o HTML é estático, isto é, não é dinâmico. E se quisermos que o HTML, em vez de pular poucas linhas, pule dez, quinze, ou vinte? Teremos que abrir o arquivo HTML e inserir diversas *tags* do tipo `<br>`.

Assim, sempre que quisermos aumentar ou diminuir o número de quebras de linha teremos que remover ou adicionar as *tags* `<br>`, sempre modificando o documento. Como ele é estático, não é possível, por exemplo, exibir um contador na tela com a passagem das horas, tampouco será possível capturar as informações do usuário.

Para que possamos de fato programar, precisaremos utilizar uma outra linguagem. O navegador é poliglota, e "fala" algumas linguagens além de HTML, sendo capaz de trabalhar com uma linguagem verdadeiramente de programação, que é o **JavaScript**.

<center> Neste treinamento, aprenderemos a lógica de programação utilizando a linguagem <b>JavaScript</b>. </center>

Queremos exibir um alerta para o usuário, um *pop-up* que surja na tela e contenha a seguinte mensagem: "isso aqui é uma linguagem dinâmica" ou "isso aqui é uma linguagem de programação".

Como fazer isso? Primeiro, definiremos a mensagem em JavaScript. E para criarmos um texto no JavaScript, é necessário que ele esteja entre aspas!

O JavaScript nos permite exibir um *pop-up* na tela, que será de alerta. Precisaremos utilizar uma instrução da linguagem indicando que um alerta deverá ser exibido: 

`alert("Isso sim é um programa");`

Há uma peculiaridade: o texto deve estar entre **parênteses e aspas duplas** **`" "`**, e com um **`;`** (ponto e vírgula) no fim:

Uso do ponto e vírgula no final de uma instrução JavaScript é opcional e neste treinamento não teremos problemas com sua ausência. Contudo, ao avançar nesta linguagem você verá determinados processamentos de código podem resultar em algo não esperado na ausência do ponto e vírgula. Sendo assim, vamos criar desde já o hábito de terminar uma instrução com o ponto e vírgula.

Adiante veremos mais sobre isso. Em teoria, isto é suficiente para escrevermos nosso primeiro código em **JavaScript**.

Porém, o *pop up* não aparece. O que temos é o texto que gostaríamos que fosse exibido na tela para o usuário aparecendo no corpo do HTML e, ainda, com um problema de acentuação - que resolveremos adiante.

Por que isto acontece? Como o navegador é poliglota, ou seja, entende mais de uma linguagem (por exemplo, HTML e JavaScript), temos que indicar que determinada linha é uma instrução.

Como faremos isto? Com uma tag `<script>`, que também abre e fecha.

```javascript
<script>
alert("Isso sim é um programa");
</script>
```

Para resolvermos o problema da acentuação, ao salvarmos o arquivo em nosso disco, o faremos com um conjunto de caracteres, e o padrão é `UTF-8`. Sendo assim, utilizamos a tag desta maneira:

```html
<meta charset="UTF-8">
```

Estamos indicando ao navegador como deve ser a interpretação das cadeias de caracteres, ou seja, do texto que está sendo exibido. Portanto, a simples adição desta *tag* resolverá o problema de acentuação.

No depurador, há uma aba chamada "Console", localizada na barra de menu superior. É possível o abrirmos acessando o menu "Visualizar" também, na barra de menu superior, selecionando "Desenvolvedor > Console JavaScript".

Os elementos que vimos agora - **o browser, o editor de texto, o depurador** - são usados para identificarmos os erros em nosso código e compõem as ferramentas que utilizaremos por todo nosso treinamento.

#### 4. Resumo

- Aprendemos que desenvolver **não** exige um ambiente complexo;
- É possível utilizar o próprio navegador, e todo sistema operacional possui um. Ao longo do curso utilizaremos o **Google Chrome**;
- Podemos utilizar um editor de texto padrão. Nós usaremos o **Sublime Text**, disponível para todas as plataformas;
- Compreendemos que o HTML é uma linguagem de marcação, pois ela possibilita marcar conteúdos por meio de *tags*;
- Algumas *tags* não possuem marcação, como o `<br>`, que serve para pular uma linha;
- A *tag* `<a>` nos permite sair de uma página e mudar para outra;
- O HTML é estático, isto é, não muda. Não podemos fazer nada muito sofisticado com ele. Por esse motivo o navegador entende também a linguagem JavaScript, que é uma linguagem de programação dinâmica, com a qual podemos desenvolver de maneira mais avançada;
- Para o navegador interpretar uma instrução JavaScript, não basta colocarmos a instrução JavaScript direto no HTML. Temos que utilizar a *tag* `<script>`. Dessa forma o navegador saberá que deve processar essa parte do código como linguagem JavaScript e não como HTML;
- A primeira instrução que vimos do JavaScript foi o `alert`, que recebe como parâmetro um texto;
- Por último, aprendemos que todo texto em JavaScript vem entre aspas.

Por incrível que pareça, a mesma ferramenta que você utiliza para navegar na web será a mesma que você utilizará para interpretar o código que você escreverá. Além disso, ele é capaz de entender mais de uma linguagem, por isso o chamo de poliglota. E como todo sistema operacional já vem com um navegador padrão instalado, isso tornará ainda mais fácil a nossa jornada no mundo da programação. Contudo, para que você tenha uma paridade visual comigo ao longo do treinamento, sugiro fortemente que você use o Chrome.

#### 5. Extensão de arquivos

Você já utilizou um processador de texto ou planilha? Por exemplo, arquivos do Microsoft Word possuem a extensão `.doc` ou `.docx`. Assim, caso você tenha salvo um arquivo chamado "receitas", dentro do computador ele será "receitas.docx". A mesma coisa serve para as planilhas do Excel, por exemplo, uma planilha chamada "custos" quando salva no computador agrega a extensão `.xls`, sendo assim, o nome completo do arquivo é `custos.xls`.

A extensão do arquivo é importante, pois confere ao Sistema Operacional uma pista de qual programa deve ser usado para abrir o arquivo em questão. Assim, todo arquivo que criarmos até o final do curso utilizará a extensão `.html`.

**Convenção (sendo politicamente correto)**

Assim como o condomínio de um prédio possui uma convenção, o mundo da programação é repleto delas. Por exemplo, uma convenção muito utilizada é criar arquivos com letras minúsculas e se houver mais de uma palavra usamos um "_" como separador. Além disso, não usamos acentos no nome dos arquivos. É claro que, assim como a convenção de um condomínio pode não ser seguida, nada impede que o programador crie o arquivo do jeito que quiser. E, da mesma forma que um morador que comete infrações não será bem visto pelos demais condôminos, o mesmo ocorre com o programador.

#### 6. Importância da tag meta.

Quando salvamos um arquivo texto no disco ele é salvo usando uma cadeia de caracteres (*character set encoding*). Se no editor de texto salvamos o arquivo contendo `charset` UTF-8, precisamos dar uma pista para o navegador de como ele deve ser processado. Se não fizermos isso, ele não conseguirá exibir corretamente qualquer texto acentuado.

Contudo, muito cuidado! Vamos supor que acidentalmente seu editor de texto não salvou o arquivo como `UTF-8`, mas em `latin1`. Se colocarmos a tag `<meta charset="UTF-8">` estaremos dando uma dica errada para o navegador e isso nos trará problemas na acentuação. Para resolver esse tipo de situação, podemos usar `<meta charset="latin">` ou mudar nosso arquivo para `UTF-8`, o que é mais difícil.

Pode ser que o editor de texto escolhido não siga o padrão UTF e utilize outro qualquer que nem eu ou você sabemos.

Mais do que os caracteres saírem certos ou errados, o importante é aprender a lógica de programação. O que estamos abordando serve para tornar sua experiência melhor e seu programa mais bonito.

### [Comunique-se com o usuário](https://cursos.alura.com.br/course/logica-programacao-javascript-html/task/17659)

#### 1. Convenção de código

Há uma convenção de que as tags HTML devem ser escritas com letras minúsculas. Porém, se utilizarmos `<H1>` ela funcionará perfeitamente.

Outro ponto: da mesma forma, se na tag `<script>` escrevermos em letras maiúsculas, o resultado não será alterado, mas a convenção aconselha a mantermos as letras minúsculas. No entanto, tenha **atenção**, o mundo JavaScript é mais rígido.

#### 2. Concatenação

Se utilizarmos o `alert` no mundo JavaScript para exibir um texto para o usuário, e caso tenhamos dez mensagens, quantas vezes o usuário terá de pressionar "OK"? Várias. Isso tornará a experiência do visitante ruim. Se ele quiser ler a última linha, não conseguirá, porque surgirão muitos alertas seguidos.

O que fazer? O mundo JavaScript é representado por tudo que está inserido na tag `<script>`. Todo o conteúdo desta tag é interpretado pelo navegador como JavaScript. O mundo HTML é compreendido como tudo que está **fora** da tag `<script>`. O que faremos é escrever, a partir do mundo JS, um HTML. Para isto, adicionaremos `document.write()`.

A palavra `document` significa, em português, "documento". Nossa página HTML, nosso programa, é um documento. Já a palavra `write` corresponde à palavra "escrever". O `write` recebe parênteses ao final, ou seja, ele aceita receber algo para escrever no documento. Como vimos, o texto no JavaScript é incluído entre aspas. O texto é chamado de `string`, tanto em JS como em outras linguagens de programação.

Se quisermos pular uma linha, por exemplo, podemos utilizar a tag `<br>`. Isso porque a frase exibida no navegador está inserida no mundo HTML, e neste contexto, utilizamos esta tag sempre que queremos pular uma linha. Como estamos escrevendo no mundo HTML, quando o navegador for processar a informação verá o `<br>` e entenderá que deve pular uma linha.

Portanto, na programação há diversas formas de se atingir um mesmo objetivo. Em algumas delas, escreveremos mais código, enquanto outras são mais diretas e simples. A forma a ser utilizada dependerá do tipo de problema que você está tentando resolver.

O JavaScript só considera algo como texto se estiver entre aspas, portanto, da forma como escrevemos `18`, o número será interpretado como texto? Não. Como sua representação é numérica, ele será interpretado como um número.

Portanto, o `document.write` aceita trabalhar com tipo `texto` - "tipo" indica que é um tipo de dado -, cujo termo técnico é *string*, e "18", que é um número. Minha idade real não é 18, entretanto, os números nos permitem realizar operações.

Quando temos uma operação de soma envolvendo texto, o JavaScript não entende se tratar de um número, e portanto realiza uma operação à qual damos o nome de **concatenação**. Isto significa que ele juntou um texto ao outro. Este é então passado para o `write`, que o imprime desta forma.

Estamos tentando somar um texto com um número. Uma string somada a outra resulta em uma concatenação, um número somado a outro resulta na soma numérica dos dois, mas quando temos uma string a ser somada com um número converte este último para texto, ou seja, quando há texto e número, ele converte tudo para texto.

#### 6. Operações com textos e números

A programação, assim como na matemática, prioriza a avaliação das multiplicações e divisões. Sendo assim, se quisermos indicar que algo deve ser avaliado primeiro, devemos inseri-lo entre parênteses, sem confundir com os parênteses que seguem o comando `write`.

A primeira coisa que o JavaScript fará é identificar a presença de parênteses, que indiquem uma operação a ser priorizada. Feito isso, a análise ocorrerá normalmente, da esquerda para a direita. Por fim, será concatenado o `<br>`, já que o comando está inserido no código HTML, resultando na quebra de linha entre uma frase e a seguinte.

### [Torne seu programa dinâmico com variáveis](https://cursos.alura.com.br/course/logica-programacao-javascript-html/section/4174/tasks)

#### 1. Reduzindo alterações

Em nosso programa, conseguimos este efeito de "envelope" por meio da criação de **variáveis**. Como o próprio nome sugere, elas variam, e são representadas da seguinte forma:

```javascript
var ano = 2016;
```

Dessa forma reduzimos o número de alterações no javascript, criando variáveis e quando ela for alterada, altera no texto todo onde ela estiver inserida.

Quando o JavaScript se depara com a variável `ano`, ele somente a interpretará como uma string se estiver em aspas (`"ano"`). Como não é o caso, ele verificará se é um número. Não se tratando de um numeral, o JS determinará se é uma variável. Anteriormente, escrevemos `var ano`, sendo assim, ela existe, e quando o valor for computado, a palavra `ano` será trocada pelo valor `2016`.

O processo de "raciocínio" do JavaScript será questionar se determinado trecho está entre aspas, e se estiver, é uma string, caso negativo, será feita uma próxima pergunta: trata-se de um número? Caso a resposta seja "não", significa que se trata de uma **variável**.

É interessante trabalharmos com variáveis, porque ao declaramos eles em um único lugar, várias instruções podem depender de uma mesma variável e, quando alteramos seu valor, isso é refletido em todos os pontos do código onde aparece.

**Cuidado**, como dito anteriormente, a variável é escrita somente com letras minúsculas.

Em qualquer momento, no próprio código, podemos indicar um novo valor para esta mesma variável. O navegador processará a tag `<script>` linha a linha, na ordem em que foram declaradas.

O prefixo `var` só é utilizado ao declararmos a variável pela primeira vez, então não é necessário utilizá-lo ao definirmos um novo valor. As variáveis nos ajudam, também, a fazer a manutenção de nosso código, já que ela é declarada em um único ponto e pode ser utilizada em diversos momentos.

#### 2. Variáveis

Uma variável pode guardar praticamente o que você quiser: um número, uma string ou outro pedaço de código.

Podemos criar novas variáveis para também diminuir o número de parênteses e ficar mais visual e organizado o código.

Para arredondar números usamos um comando contido em Javascript:

```javascript
Math.round()
```

Assim passando um parâmetro para os parênteses, esse comando consegue arredondar os números. 

Uma convenção importante: o nome de uma variável sempre se iniciará com uma letra **minúscula**. Se a variável contém duas palavras, por exemplo "idade + (nome)", a próxima palavra deve ser escrita com a primeira letra **maiúscula**. Este padrão recebe o nome de **camelCase**.

E se quisermos escrever a variável inteira em letras minúsculas, mesmo que sejam duas palavras? O seu código funcionará da mesma forma, o nome da variável apenas não vai seguir a convenção do mundo da programação.

Para esclarecer que as variáveis não podem guardar somente números, criaremos o seguinte trecho:

```javascript
var nome = 'Jonatas';
```

No JavaScript, podemos utilizar tanto as aspas simples (**`'`**) quanto aspas (**`"`**). Colocaremos as aspas duplas, mesmo porque outras linguagens de programação as utilizam.

### [Crie suas próprias funcionalidades](https://cursos.alura.com.br/course/logica-programacao-javascript-html/section/4175/tasks)

#### 1. Melhorando a manutenção do código
