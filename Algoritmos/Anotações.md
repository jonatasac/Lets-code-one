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

## Decisão

