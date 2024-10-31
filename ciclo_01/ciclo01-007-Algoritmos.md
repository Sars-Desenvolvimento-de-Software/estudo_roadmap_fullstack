# Ciclo 01: Algoritmos

Chegamos ao último passo do ciclo 01, um ciclo que foi focado em dar uma base necessária para entendimento de conceitos mais complexos na programação.

Neste último tópico do ciclo trabalharemos o conceito inicial para qualquer programador, o Algoritmo. Esse conceito já foi explorado no tópico [Lógica na programação](./ciclo01-004-Lógica-De-Programação.md) de maneira discreta, portanto acredito que será algo bem simples para quem acompanhou o conteúdo.

Um algoritmo é um conjunto de passos bem definidos e que buscam solucionar uma problema, ele recebe entradas, executa algum processamento e gera as saídas esperadas.

Um algoritmo portanto é o código-fonte construído pelo programador, porém ele não é o aplicativo, ou um módulo ou uma funcionalidade, ele é a implementação da sua lógica portanto o melhor trecho do código-fonte que atenda a definição é um algoritmo.

**"A partir de agora começaremos a usar o JavaScript como nossa linguagem de programação para as explicações e para as atividades"**

## Conteúdo

> ### Abstração

Como foi comentado no tópico anterior, o processo de abstração é a habilidade de olhar para um cenário e decidir como ele será tratado, dependendo de como decidir lidar com o problema (ou melhor dizendo, como você abstrair ele) talvez faça sentido usar duas funções e cinco variáveis, ou possa resolver o problema apenas usando uma função e uma variável.

Vamos usar um exemplo:

```
Você precisa criar um software para ler um arquivo texto e para cada linha você deve extrair um nome existente.
```
Analisando essa necessidade eu posso pensar que ler o arquivo todo, depois identificar as quebras de linha e depois percorrer todos os caracteres da linha até achar o nome seja um abordagem.

Porém, eu também poderia pensar que abrir o arquivo, ler a primeira linha, percorrer os caracteres e achar o nome, depois pegar a segunda linha e fazer isso sucessivamente é uma abordagem mais válida.

Essas foram as formas que eu abstrai o meu problema e pensei usando o paradigma imperativo, você talvez encontre outra forma.

**Lembre-se: Uma boa abstração costuma poupar muito tempo no desenvolvimento de software!**

> ### Tipos de dados

JavaScript e fracamente tipada, sendo assim os tipos nas variáveis são inferidos durante seu uso e podem mudar ao longo da execução do programa.

Os tipos de dados são os tipos que podemos usar para armazenar as informações durante a execução de um programa. Os tipos de dados podem ser primitivos ou compostos.

#### Primitivos

- **Boolean**: Valores lógicos como verdadeiro (true) ou falso (false)
- **Number**: Valores numéricos com ou sem casas decimais
- **String**: Valores alfanuméricos
- **null**: Palavra-reservada para indicar que o valor de uma variável é nulo
- **undefined**: Palavra-reservada para indicar que a variável não teve valor atribuido ou é indefinido

```
let anoBissexto = true;
let cotacaoDolar = 5.36;
let nome = "Augustus Maximus";
let semValor = null;
let valorNaoDefinido; // Esse será undefined
```

#### Compostos

- **Arrays**: São variáveis que se comportam como uma coleção de valores que podem ser do mesmo tipo ou não. Se forem do mesmo tipo chamamos de vetor homogêneo, se tiverem tipos diferentes chamamos de vetor heterogêneo.

- **Objetos**: São grupos de propriedades e valores que podem ser usados para armazenar dados complexos. Por exemplo: um objeto poderia armazenar os campos de um cadastro de funcionário.

```
let listaDeNomes = ["maira", "maria", "manu"]; //vetor homogêneo de Strings

let listaDe = ["pedro", 15.98, false]; //vetor heterogêneo com Strings, Number e Boolean

let paciente = {
  nome: "Marcela Faria",
  idade: 45,
  convenio: true
}; // Objeto
```

#### Tipos de variáveis

Além dos tipos de dados vamos olhar os tipos de "variáveis" que podemos criar.

- **variável**: Espaço em memória alocado para armazenar um dado que pode ser modificado depois.

- **constante**: Espaço em memória alocado para armazenar um dados que não poderá ser mudado depois.

```
let nomeDoPaciente = "PacienteA";
nomeDoPaciente = "PacienteB";

const nomeDoMedico = "Plantonista";
nomeDoMedico = "MedicoA"; // Isso gera um erro!
```

#### Operadores

Agora podemos ver um pouco sobre os operadores que podem ser usados em JavaScript.

- Aritméticos
  - (+) soma
  - (-) subtração
  - (*) multiplicação
  - (/) divisão
  - (=) igualdade

- Concatenação de texto
  - (+) une duas strings

- Lógicos
  - (&&) usando para testar se duas coisas são verdadeiras
  - (||) usado para testar se ao menos uma coisa é verdadeira

- Comparação
  - (>) usado para testar se o que está na esquerda é maior do que o que está na direita
  - (<) usado para testar se o que está na esquerda é menor do que o que está na direita
  - (>=) usado para testar se o que está na esquerda é maior ou igual do que o que está na direita
  - (<=) usado para testar se o que está na esquerda é menor ou igual do que o que está na direita

- Atribuição
  - (=) usado para atribuir o valor da direita a variável da esquerda
  - (+=) usado para atribuir o valor da direita a variável da esquerda somando com o valor existente na esquerda
  - (-=) usado para atribuir o valor da direita a variável da esquerda subtraindo com o valor existente na esquerda
  - (*=) usado para atribuir o valor da direita a variável da esquerda multiplicando com o valor existente na esquerda
  - (/=) usado para atribuir o valor da direita a variável da esquerda dividindo com o valor existente na esquerda
  - (++) usado para atribuir soma 1 ao valor da variável
  - (--) usado para atribuir subtrair 1 ao valor da variável

> ### Estruturas condicionais

Assim como vimos no tópico 4, existem as estruturas condicionais que ajudam a tomar decisões dentro do algoritmo.

- if
  
  O comando if te ajuda a testar uma condição e fazer uma ação que essa condição for verdade ou se for falsa.
  ```
  if( condição ) { 
    Ação se for verdadeiro
  }

  OU 

  if( condição ) {
    Ação se for verdadeiro
  } else {
    Ação se for falso
  }
  ```

- switch
  
  O comando switch permite testar um valor contra vários casos e decidir qual o caso que deve ser executado. Caso nenhum caso seja executado a condição padrão (default) será executada.
  ```
  switch( expressão ) {
    case Valor1:
      Ação se for verdadeiro;
      break;

    case Valor2:
      Ação se for verdadeiro;
      break;

    default:
      Ação se for verdadeiro;
  }
  ```

> ### Estruturas de repetição

Assim como estruturas para tomadas de decisão foram necessárias, estruturas para repetição de trechos de lógica também são e permitem simplificar muito a implementação e o tamanho do código-fonte.

- for
  
  O comando for permite repetir um bloco de código uma quantidade limitada de vezes.

  Ao declarar um for você passa a criação de uma variável e seu valor inicial, depois a condição de parada, por fim você adiciona a regra de incremento da variável
  ```
  for(let passo = 1; passo < 5; passo++) {
    Ação que será repetida;
  }
  ```

- while
  
  O comando while permite repetir um bloco de código enquanto uma condição é verdadeira. Você também pode usar uma variação do comando que garante que a primeira execução sempre será feita.

  É importante observar se estamos atualizando a condição para que o while não se torne um loop infinito indesejado.
  ```
  while(condição) {
    Ação que será repetida;
  }

  do {
    Ação que será repetida;
  } while(condição);
  ```

> ### Funções

Uma função é um trecho de lógica que é guardado com um nome e pode ser chamado sempre que necessário. Ele processa algo e devolve um valor.

```
  function MinhaFunção(parâmetros) {
    Ação que será executada;
    return RetornoDaFunção;
  }

  let retorno = MinhaFunção(1,2,3);
  ```

> ### Procedimentos

Procedimentos são como funções, porém não há um retorno a ser dados, apenas um processamento que é executado.

Em JavaScript não temos procedimentos, mas caso você crie uma função e não defina retornou, na prática isso seria um procedimento.

> ### Funções básicas

Conhecer algumas funções básicas da linguagem poderá te ajudar ao construir seus algoritmos.

- console.log(): Permite exibir no terminal um valor

### Conclusão

Com isso finalizamos o conteúdo do ciclo 01, nele você relembrou sobre o funcionamento básico e as partes que compõem um computador, viu a grande quantidade de plataformas e suas características, conheceu várias linguagens que existem na programação e algumas particularidades das linguagens de programação.

Não podemos esquecer que você estudou um pouco de lógica e conheceu superficialmente detalhes sobre a linguagem JavaScript e como ela pode ser usada para criar algoritmos.

Ao chegar aqui você já é capaz de desenvolver pequenos algoritmos com funcionalidades específicas, e já deu o primeiro passo em relação a construção de aplicativos sofisticados.

No próximo ciclo continuaremos ampliando seu repertório teórico para te dar uma base sólida sobre construção de algoritmos complexos e se aprofundar em bibliotecas específicas da linguagem JavaScript. Bora!

## FIXAÇÃO

### Atividade 01

Reveja os exercícios do tópico 4 desse ciclo, se você conseguiu fazer os algoritmos em pseudocódigo terá metade do trabalho feito, agora você pode construir aqueles algoritmos usando JavaScript.

---
---
---

<div style="text-align: center;">

   [<<< Anterior: Linguagem de programação](./ciclo01-006-Linguagem-De-Programação.md)

</div>