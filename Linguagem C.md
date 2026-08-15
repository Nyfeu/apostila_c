
> Este tópico é voltado para o estudo da **linguagem de programação C**. Aqui serão tratados diversos assuntos, como: configuração do ambiente para a linguagem, alocação de memória, sistema binário, compilação, números pseudoaleatórios, controle do fluxo do programa, estruturas de dados etc.

## 1. Hello, World!

Abaixo temos o código mais fundamental de todos, o famoso “**hello_world.c**” que será o primeiro código a ser destrinchado.

```c
/*
	Seu primeiro programa em C
	** Para dar sorte! hehe ** 
*/
	
#include <stdio.h>         // Inclui a biblioteca padrão de input e output
						 // Standard Input and Output
int main() {

	printf("Hello, World!");   // Exibe "Hello, World!" na tela
	return 0;                 
	
}
```

Apesar de ser um programa muito simples (nosso primeiro programa) - que é repleto de mitos e superstições por trás - podemos entender já alguns conceitos fundamentais acerca do funcionamento da linguagem com esse código.


### 1.1. Estrutura do Código


A primeira coisa que encontramos no código, logo de cara, são os comentários. Eles podem ser de uma única linha ou de várias linhas - sendo respectivamente demarcados por:

```c
/* 
		 Esse é um comentário de múltiplas linhas!
*/

//   Esse é um comentário de uma única linha!
```

Mas, o que são comentários? São trechos do código que são ignorados pelo compilador - este sendo responsável por transformar um código de extensão `.c` em executável `.exe` - esta parte da será tratada no seguinte subtópico: [[Métodos de Tradução]].

**Nota: preste atenção que eu disse “compilador” -** sim, a linguagem **C** é um linguagem compilada. Outras linguagens podem ser interpretadas (caso do JavaScript ou Python etc) ou ter um processo híbrido (caso do Java). 

> [!quote] Ok… agora que sabemos como ser ignorados pelo compilador (parece até a vida real).

A próxima linha de código tem relação direta com o **pré-processador**, tratando das chamadas **diretivas**. A diretiva em questão aqui é o **include** que serve para incluir outros arquivos ao nosso programa. No caso a biblioteca “**standard input/output**” que provê funções que tratam sobre inserção e exibição de dados, que é o caso da função `printf` que será usado nesse mesmo programa posteriormente.

Mais sobre o pré-processador, bibliotecas, inserção e exibição de dados poderá ser visto nos tópicos específicos.

Em seguida, temos a definição da função `main()` :

```c
int main(void) { 

     // dentro dos parênteses acima - onde está "void" 
     // (que é chamado de argumentos) podemos por parâmetros de 
     // execução do programa, que será exposto no tópico: "Argumentos 
     // na função main()".

...
```

Tudo que estiver dentro do bloco/escopo (demarcado com as chaves `{ }` ) fará parte da chamada função `main()` .

O próximo comando é o `printf()` que serve para expor na saída padrão (que será tratada posteriormente - em “[[Manipulação de Entradas e Saídas]]” ) um conteúdo que, no caso, é a string `“Hello, world!”`.

Em seguida temos o retorno do código de erro da execução do programa, através da função `return 0` que denota a ausência de erros. Este é um conceito de suma importância quando tratamos de engenharia de software!

Perceba também que todos os comandos são finalizados com ponto e vírgula (`;`). Na maioria das vezes pode ser o problema para o seu programa não compilar hahaha…. 🥲

### 1.2. Rodando o Programa

Para rodar o programa precisamos compilá-lo e executá-lo.

Para compilar, precisamos executar o **gcc** que é tratado no tópico de “compilação”:

```bash
> gcc -o hello_world hello_world.c
```

E para executá-lo de fato:

```bash
> ./hello_world
> Hello, World!
```

## 2. Considerações Importantes

Este tópico é voltado à exploração de conceitos fundamentais para a programação. Sejam bases numéricas - como binário e hexadecimal, até sobre a memória, processo de compilação etc.

- [[Sistema Binário]]
- [[Sistema Octal e Decimal]]
- [[Relações de Sistemas Numéricos]]
- [[Memória]]
- [[Pré-Processamento]]
- [[Compilação]]
- [[Números Pseudoaleatórios]]

## 3. Declarações da Linguagem

Este tópico é voltado para as funções que de fato declaramos no código, sejam as diretivas, as principais bibliotecas, estruturas de controle de fluxo - métodos de manipulação de arquivos, memória etc.

- [[Tipos de Variáveis]]
- [[Bibliotecas de Software]]
- [[Protótipos de Funções]]
- [[Estruturas de Decisões]]
- [[Lações de Repetição]]
- [[Desvios]]
- [[Arranjos Unidimensionais]]
- [[Arranjos Bidimensionais]]
- [[Ponteiros]]
- [[Alocação de Memória Dinâmica]]
- [[Registros e Structs]]
- [[Input]]
- [[Output]]
- [[Manipulação de Entradas e Saídas]]
- [[Operadores]]
- [[Argumentos de Entrada]]
- [[Segmentando o Programa]]
- [[Uniões]]
- [[Casting (Conversão)]]
- [[Enumeração (enum)]]
- [[Ponteiros de Funções]]
