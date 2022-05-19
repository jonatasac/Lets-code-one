# Algoritmos

## Introdução

Sequência de passos lógicos para resolução de um determinado problema.

Por exemplo: Sequência de passos para fazer um bolo.

Coloque primeiro no copo do liquidificador os itens líquidos (ovos,  leites, etc) e só depois entre com os sólidos (farinha, chocolate...).

## Fluxos Simples, Sequencial

Início > Entrada > **Processamento** > Saída > Final

Exemplo: Escrever nome da pessoa.

- Início
- Pedir nome da pessoa
- Armazenar nome da pessoa
- Juntar nome da pessoa ao texto "Bom dia"
- Mostra a frase montada
- Final

Precisamos montar o passo-a-passo para a resolução de problemas antes de passar pro computador executar.

PseudoCódigo:

> INICIO principal
>
>    MOSTRAR 'Digite seu nome'
>
>    ESPERAR_DIGITACAO -> nome
>
>    JUNTAR_TEXTO 'Bom dia'.nome -> saudacao
>
>    MOSTRAR_TEXTO saudacao
>
> FIM

Teste de Mesa:

| comando                                  | saída na tela      | armazenamento                                  |
| ---------------------------------------- | ------------------ | ---------------------------------------------- |
| MOSTRAR 'Digite seu nome'                | 'Digite seu nome'  |                                                |
| ESPERAR_DIGITACAO + nome                 |                    | Nome = 'Julia'                                 |
| JUNTAR_TEXTO 'Bom dia, ' nome = saudacao |                    | Nome = 'Julia'<br>Saudacao = 'Bom dia, Julia'  |
| MOSTRAR saudacao                         | **Bom dia, Julia** | Nome = 'Julia'<br/>Saudacao = 'Bom dia, Julia' |

## Tipos de Dados

Precisamos informar ao computador quais tipos de dados estão sendo informados para que o computador possa processar para nós.

- Numérico. Valor que pode expressar valor, volume etc. Pode ser utilizado para operações matemáticas que envolva valores dentro do programa.
  - Inteiros. Números inteiros.
  - Ponto flutuante. Os que tem casa depois da vírgula.

- Texto. Definidos geralmente entre aspas para exibir algum texto na tela.
- Booleano. True (verdadeiro) ou False (Falso).

### Variáveis

Um identificador de um valor dentro da memória do computador. Sempre que definimos uma variável precisamos mostrar ao computador o Tipo de dados dessa variável (Numérico, Texto ou Booleano).

São muito importantes na construção de algo no computador. É onde registramos no computador uma informação que passamos ao computador.

Exemplo:

- Obter o Primeiro número
- Armazenar o primeiro número -> n1
- Obter o segundo número
- Armazenar o segundo número -> n2
- Somar n1 e n2 -> resultado
- Mostrar resultado

Guardamos as informações em 2 variáveis e definimos uma terceira para mostrar o resultado da soma dessas 2 variáveis.

PseudoCódigo:

> INICIO principal
>
>    VAR n1: INTEIRO
>
>    VAR n2: INTEIRO
>
>    DEFINIR 0 -> n1
>
>    DEFINIR 0 -> n2
>
>    MOSTRAR "Digite o primeiro número: "
>
>    ESPERAR_DIGITACAO -> n1
>
>    MOSTRAR "Digite o segundo número: "
>
>    ESPERAR_DIGITACAO -> n2
>
>    SOMAR n1, n2 -> resultado
>
>    MOSTRAR resultado
>
> FIM

Sem as variáveis não conseguimos armazenar as informações na memória de trabalho do computador e não conseguimos fazer nosso algoritmo funcionar.

## Estruturas de Decisão

Nos dá a oportunidade de decidir quais funções vamos rodar e quais não vamos rodar em determinada tarefa. E essa decisão pode voltar ao fluxo inicial de um determinado algoritmo.

Exemplo1:

- Idade maior ou igual a 16 anos?
  - Se não:
    - Esperar ter pelo menos 16 anos
    - FINAL
  - Se sim:
    - Ir até o cartório eleitoral mais próximo
    - votar em outubro
    - FINAL

Exemplo2:

- INICIO
- mostrar 'Digite seu nome'
- armazenar o nome na variavel NOME
- mostrar 'que horas são?'
- armazenar a hora na variavel HORA_ATUAL
- avaliar o valor em HORA_ATUAL
  - Se 0 a 12
    - armazenar 'Bom dia' em MENSAGEM
  - Se 12 a 18
    - armazenar 'Boa tarde' em MENSAGEM
  - Se 18 a 24
    - armazenar 'Boa noite' em MENSAGEM
- Mostrar MENSAGEM, NOME
- FINAL

PseudoCódigo:

> INICIO principal
>
> ​	VAR nome: STRING
>
> ​	VAR hora: INTEIRO
>
> ​	VAR mensagem: STRING
>
> ​	MOSTRAR "Digite seu nome: "
>
> ​	ESPERAR_DIGITACAO -> nome
>
> ​	MOSTRAR "Digite a hora atual (somente a hora): "
>
> ​	ESPERAR_DIGITACAO -> hora
>
> ​	SE (hora MAIOR_QUE 0) E (hora MENOR_QUE 12)
>
> ​		DEFINIR "Bom dia " -> mensagem
>
> ​	OU_SE (hora MAIOR_OU_IGUAL_A 12) E (hora MENOR_QUE 18)
>
> ​		DEFINIR "Boa noite " -> mensagem
>
> ​	MOSTRAR mensagem, nome
>
> FIM

O computador vai se adaptar a uma regra definida e assim executar a lista de comandos específica.

As estruturas de decisão são usadas para decidir o que fazer com cada informação que der entrada.

Pode usar várias estruturas de decisão dentro de outras estruturas de decisão, sempre que necessário.

## Estruturas de Repetição

Vão ter comandos pra decidir o que fazer e comandos para repetir este comando de decisão. É mais chamado de Loop. A quantidade de loops que foi executado é chamado de iterações.

Exemplo1:

- Início
- Iteracao_atual = 1
- soma=0
- mostrar "entre com um numero"
- esperar numero -> num
- somar soma com num
- somar 1 em iteracao_atual
  - se iteracao_atual > 3
    - mostrar soma
  - senao
    - retornar a mostrar "entre com um numero"
- FIM

PseudoCódigo: (Pedir para o usuario digitar numeros ate que a soma seja igual ou maior a 100 e depois mostrar a soma)

>INICIO principal
>
>​	VAR soma: INTEIRO
>
>​	ARMAZENAR 0 -> soma
>
>​	ENQUANTO soma MENOR QUE 100
>
>​		MOSTRAR "Digite um número: "
>
>​		ESPERAR_DIGITACAO -> numero
>
>​		SOMAR soma, numero -> soma
>
>​	FIM ENQUANTO
>
>​	MOSTRAR soma
>
>FIM

O computador roda todos os comandos do loop até a condição do loop ser atendido. Algumas linguagens permite que seja interrompido o loop no meio, mas não é o caso no momento.

O laço é um grupo de comandos que vai ser executado até a variável de avaliação seja verificada como não válida.

É preciso estar bem definida a variável de avaliação para o programa saber quando interromper, se não vai rodar sem parar.

## Listas/Arrays

As variáveis possuem limitação, só é possível armazenar um item por vez.

Arrays são usados para armazenar uma sequência de informações na ordem que são fornecidos.

Em algumas linguagens é possível armazenas em uma array vários tipos de dados, em outras linguagens é necessário que na array só tenha um tipo de dados.

Exemplo1:

> INICIO principal
>
> ​	VAR lista_numeros: LISTA(INTEIRO)
>
> ​	VAR numero_atual: INTEIRO
>
> ​	DEFINIR 1 -> numero_atual
>
> ​	ENQUANTO (QUANTIDADE_INTENS(lista_numeros) MENOR_QUE 20)
>
> ​		SE (RESTO(DIVISAO(numero_atual, 2)) IGUAL_A 0) OU (RESTO(DIVISAO(numero_atual, 5)) IGUAL_A 0)
>
> ​		ADICIONAR_ITEM numero_atual, lista_numeros
>
> ​		FIM SE
>
> ​	DEFINIR numero_atual + 1 -> numero_atual
>
> ​	FIM ENQUANTO
>
> ​	MOSTRAR lista_numeros
>
> FIM

Geralmente a contagem de posições em uma lista começa em 0 (zero).

Exemplo2:

> INICIO principal
>
> ​	VAR lista_numeros: LISTA(INTEIRO)
>
> ​	VAR numero_atual: INTEIRO
>
> ​	DEFINIR 1 -> numero_atual
>
> ​	ENQUANTO (QUANTIDADE_INTENS(lista_numeros) MENOR_QUE 20)
>
> ​		SE (RESTO(DIVISAO(numero_atual, 2)) IGUAL_A 0) OU (RESTO(DIVISAO(numero_atual, 5)) IGUAL_A 0)
>
> ​			ADICIONAR_ITEM numero_atual, lista_numeros
>
> ​		FIM SE
>
> ​	DEFINIR numero_atual + 1 -> numero_atual
>
> ​	FIM ENQUANTO
>
> ​	MOSTRAR lista_numeros
>
> ​	PARA CADA item EM lista_numeros
>
> ​		SE (RESTO(DIVISAO(item, 2)) IGUAL_A 0)
>
> ​			MOSTRAR "Numero ", item, " é par"
>
> ​		SENAO
>
> ​			MOSTRAR "Numero ", item, " é ímpar"
>
> ​		FIM SE
>
> ​	FIM PARA
>
> FIM

## Funções

São usados para organizar códigos e algorítmos. Sempre tem uma entrada e tem uma saída, lembra até a idéia de algoritmos e muitas pessoas chamam funções de subprogramas. As funções permitem reaproveitar boa parte dos códigos. Sempre bom deixar isolado e só chamar quando for preciso.

Exemplo1:

- Inicio
- mostrar 'passo 1, obter os numeros'
- chamar FUNCAO_OBTER_NUMEROS
- mostrar lista_numeros
- Fim

Sendo:

- FUNCAO_OBTER_NUMEROS
- mostrar 'Digite um numero'
- obter numero
- adicionar numero na lista lista_numeros
- tamanho de lista_numeros < 10
  - SE sim
    - Retornar para mostrar 'Digite um numero'
  - SE nao
    - retornar lista_numeros
- Fim

PseudoCódigo

> INICIO principal
>
> ​	VAR lista_numeros: ARRAY(INTEIRO)
>
> ​	MOSTRAR "Vamos Obter os números: "
>
> ​	CHAMAR OBTER_NUMEROS -> lista_numeros
>
> ​	MOSTRAR "Agora, mostrar os números: "
>
> FIM

Função:

> INICIO OBTER_NUMEROS
>
> ​	VAR lista_numeros_func: ARRAY(INTEIRO)
>
> ​	VAR numero: INTEIRO
>
> ​	ENQUANTO TAMANHO(lista_numeros) MENOR_QUE 10
>
> ​		MOSTRAR "Digite um numero "
>
> ​		ESPERAR_DIGITACAO -> numero
>
> ​		ADICIONAR_ITEM numero, lista_numeros_func
>
> ​	FIM ENQUANTO
>
> ​	RETORNAR lista_numeros_func
>
> FIM OBTER_NUMEROS

Após rodar a função os dados obtidos são perdidos, não precisa mais guardar nela os dados.

Conseguimos isolar assim complexidade e responsabilidade. Sabendo assim resolver erros que podem ocorrer no programa.

## Exercício Completo (PSEUDOCÓDIGO)

### Criação de um caixa eletrônico

> INICIO principal
>
> ​	VAR opcao_selecionado: STRING
>
> ​	VAR valor: INTEIRO
>
> ​	VAR saldo: INTEIRO
>
> ​	VAR encerrar_programa: BOOLEANO
>
> ​	DEFINIR encerrar_programa -> Falso
>
> ​	ENQUANTO encerrar_programa = Falso
>
> ​		CHAMAR MOSTRAR_MENU -> opcao_selecionada
>
> ​		SE opcao_seleciona = a
>
> ​			MOSTRAR "Seu saldo é: ", saldo
>
> ​		OU_SE opcao_selecionada = b
>
> ​			MOSTRAR "Digite o valor a depositar: "
>
> ​			ESPERAR_DIGITACAO -> valor
>
> ​			SOMAR valor, saldo -> saldo
>
> ​			MOSTRAR "Depósito efetuado"
>
> ​		OU_SE opcao_selecionada = c
>
> ​			MOSTRAR "Digite o valor a retirar: "
>
> ​			ESPERAR_DIGITACAO -> valor
>
> ​			SE valor > saldo
>
> ​				MOSTRAR "Saque não permitido, saldo insuficiente"
>
> ​			SENAO
>
> ​				SUBTRAIR valor, saldo -> saldo
>
> ​			FIM SE
>
> ​			MOSTRAR "Saque Efetuado"
>
> ​		OU_SE opcao_selecionada = d
>
> ​			DEFINIR Verdadeiro -> encerrar_programa
>
> ​		SENAO
>
> ​			MOSTRAR "Opção inválida, tente novamente!"
>
> ​		FIM SE
>
> ​	FIM ENQUANTO
>
> FIM



> INICIO MOSTRAR_MENU
>
> ​	VAR opcao_selecionada: STRING
>
> ​	MOSTRAR "Menu de operação"
>
> ​	MOSTRAR "[a] Mostrar Saldo"
>
> ​	MOSTRAR "[b] Efetuar depósito"
>
> ​	MOSTRAR "[c] Efetuar Saque"
>
> ​	MOSTRAR "[d] Finalizar"
>
> ​	ESPERAR_DIGITACAO -> opcao_selecionada
>
> ​	RETORNAR opcao_selecionada
>
> FIM MOSTRAR_MENU

## Desempenho de Algoritmos

Programar é construir algoritmos de forma otimizada. Precisamos montar algo que funcione e funcione bem.

A complexidade dos algoritmos podem estar relacionados com a forma que armazenamos os dados. Os dados e os comandos devem estar organizados de forma a deixar os nossos programas rodando mais rápido.

Tipos de Notação a complexidade de algoritmos:

- Acesso direto aos dados. Operação de complexidade 1.
- BIG O. Mostra um O e um número do lado e mostra o numero de operações que foram feitas. BIG O de N.
- O de log de N na base 2. Pesquisa logaritmica que vai reduzindo a quantidade de itens de forma logaritmica, reduzindo assim o numero de operações que precisa fazer.

## Dicas para Montar Algoritmos

Precisamos definir qual problema nós precisamos resolver. Podemos contruir o algoritmo e depois ir melhorando as funcionalidades dele.

Precisamos conhecer bem as ferramentas que vamos utilizar para poder construir programas melhores.

Precisamos testar ao máximo nosso programa para apresentarmos soluções para os possíveis erros que possa aparecer.

