# Ciclo 01: Lógica de Programação

Após as etapas 2 e 3 do ciclo 01, que buscavam nivelar o conhecimento básico para seguir com o curso, iniciaremos a parte 4 e a partir de agora você já começará a criar códigos e programar, ainda não usará uma linguagem de programação. Apesar disso, não subestime esta etapa, pois será a base para tornar sua vida muito mais simples quando estiver programando, então muita atenção ao conteúdo e aos execícios deste documento 👀

Colocarei alguns destaques com o `ícone 🆙 <Referência>` durante o conteúdo sempre que eu for "amarrar" algo que estamos vendo agora com assuntos que vimos nas etapas anteriores, espero que isso ajude a fixar o aprendizado e que você perceba que tudo que estamos vendo está conectado e te ajudará de alguma forma. Vamos começar! ⏯️

## Conteúdo

> ### Lógica

A lógica pode ser resumida na habilidade ou estudo de construir um raciocínio através de premissas e gerar uma conclusão, que pode estar certa ou errada, porém sempre será coerente ou como dizemos "fará sentido"/"terá lógica" 😄

Por mais que as vezes negligenciamos propositalmente ou inconscientemente a lógica no nosso dia a dia, usamos o raciocínio lógico a cada decisão que tomamos, pois estamos sempre buscando argumentos positivos ou negativos para ajudar a decidir.

De uma maneira simples, podemos dizer que as premissas ou proposições são os argumentos, a forma como organizamos os argumentos para tomar uma decisão é a aplicação da lógica e a decisão que tomamos é a conclusão  do nosso racíocinio.

Note que quando se trata de lógica é mais importante coerência na construção do que chegar a uma conclusão certa, e isso é parecido na programação, pois muitas vezes você terá várias formas de fazer a mesma coisa e entender o que se deseja fazer é mais importante do que discutir qual forma usar.

📑 Se aprofunde mais sobre o tema lendo o [TEXTO - Wikipedia](https://pt.wikipedia.org/wiki/L%C3%B3gica)

📑 Explore um pouco mais lendo o [TEXTO - Toda Matéria](https://www.todamateria.com.br/falacia/) -  _Neste texto observe que as vezes mesmo um racíocinio parecendo coerente, ele pode não ser._

> ### Lógica na programação

Na programação a lógica está intimamente presente, pois seu programa será tão bem escrito quanto for sua habilidade de colocar em palavras os passos necessários que o computador precisa executar para chegar no resultado desejado.

Caso você pule algum passo ou descreva ele de maneira confusa o computador não conseguirá executar ele ou executará de uma forma indesejada, então ser preciso no que se deseja e entender profundamente o funcionamento esperado são as chaves 🔑 para não ficar quebrando a cabeça desnecessariamente enquanto se programa.

Na programação usamos linguagens específicas para dizer ao computador os passos que queremos que ele execute (_falaremos mais sobre isso em etapas futuras nesse momento basta pensar que são como idiomas diferentes_). Para simplificar usaremos nesta etapa o português como linguagem com algumas limitações.

> 🆙 [Ciclo 01 Etapa 001: Introdução #Pseudolinguagem](./ciclo-01-001-Introdução.md)<br/>
> Caso queira se recordar sobre o que é uma pseudolinguagem e quais regras definimos, basta clicar no link e reler, porém se desejar seguir não tem problema, pois descreverei as regras quando necessário!

> ### Pseudocódigo

Como já sabemos o que é uma pseudolinguagem e definimos as regras que seguiremos agora precisamos aplicar isso na criação de comandos, e como estamos usando uma pseudolinguagem daremos o nome de pseudocódigo ao código-fonte dos programas que criaremos 🤓

💡 Interessante comentar que apesar de termos definido uma pseudolinguagem para nossos exercícios, existem softwares criados para executar pseudocódigos e te permitir "programar" mais próximo de como seria com uma linguagem de programação. <br/>
Caso queria conhecer um pouco mais veja o [TEXTO - Wikipedia](https://pt.wikipedia.org/wiki/Portugol) ou pesquise no Google por Portugol e VisualG.

### Armazenar dados em memória

A primeira coisa que precisamos decidir como aplicar no nosso pseudocódigo é a forma de armazenar dados, já que basicamente softwares são programas que controlam e processam dados, teremos que gerenciar eles o tempo todo.

#### Como faremos:

> Diremos no código que a informação será guardada em uma palavra qualquer. <br/>
> Por exemplo: `Guardar em IDADE a idade do usuário`
>
> E quando quisermos recuperar essa informação diremos que usaremos ela <br/>
> Por exemplo: `SOMAR 10 a IDADE`
>
> _Neste exemplo a idade informada no momento em que guardamos é usada na ação de somar mais 10 a ela._

> 🆙 [Ciclo 01 Etapa 002: Arquitetura de computadores #Memória](./ciclo-01-002-Arquitetura-De-Computadores.md)<br/>
> Ao estudar as memórias de um computador vimos que existiam os tipos voláteis (RAM) e os tipos não voláteis (HD/SSD).<br/>
> Ao guardar um dados em seu programa você está usando a memória RAM para isso, e portanto caso o computador seja desligado seu programa perderá as informações que guardou durante sua execução.

> 🆙 [Ciclo 01 Etapa 003: Plataformas](./ciclo01-003-Plataformas.md)<br/>
> Ao estudar sobre as plataformas vimos que as plataformas Desktop e Nuvem costumam ter mais recursos disponíveis do que dispositivos móveis, e que embarcados costumam ser bem limitados neste aspecto.<br/>
> Portanto ao escrever o comando `Guardar em` em seu programa lembre-se de considerar para qual plataforma ele está sendo desenvolvido para evitar sobrecarregar o equipamento por consumir muito recurso.

### Exibir dados

Uma vez que temos os dados guardados e processamos eles temos que devolver o resultado ao usuário de alguma forma, e para isso usaremos a exibição dos dados na tela para o usuário.

#### Como faremos:

> Diremos no código que a informação será exibida. <br/>
> Por exemplo: `Exibir IDADE`
>
> _Neste exemplo a idade armazenada é exibida para o usuário._

> 🆙 [Ciclo 01 Etapa 002: Arquitetura de computadores](./ciclo-01-002-Arquitetura-De-Computadores.md)<br/>
> Ao estudar o processador e os periféricos de um computador vimos que o processador é o responsável or executar as instruções e enviar ao monitor que transforma a informação de forma a iluminar os pixels da monitor e gerar a imagem.<br/>
> Assim ao executar o comando `Exibir` você está usando programas criados por outras pessoas que fazem toda essa comunucação entre processador e monitor para que a imagem seja gerada.

> 🆙 [Ciclo 01 Etapa 003: Plataformas](./ciclo01-003-Plataformas.md)<br/>
> Quando abordamos o suporte e a importância dos sistemas operacionais era sobre comandos assim que falamos.<br/>
> Sem um SO ou software fazendo a comunicação entre seu aplicativo e o hardware, você teria que aprender sobre cada tipo de computador e monitor que seu aplicativo poderia usar e criar códigos específicos para cada fabricante, tornando o trabalho de programação caro e inviável 😥 

### Operadores

Operadores são símbolos que ajudam a executar algumas ações. Em nosso pseudocódigo usaremos o nome dos operadores aritméticos e relacionais, e a exceção será o operador `+` que usaremos para dizer que estamos unindo textos para apresentar uma mensagem única.

#### Como faremos:

> Usaremos no código o nome do operador. <br/>
> Por exemplo 1: `Guardar em SOMA 25 multipliacado por 4`
>
> Por exemplo 2: `Se 100 dividido por 4 é maior que 30 então ... Fim Se`
>
> Por exemplo 3: `Exibir "Oi" + " tudo bem " + "?"`

### Verificações

As verificações são necessárias para testar condições e fazer nossos aplicativos mais inteligentes, então suponha que você só deve somar 10 a idade se a pessoa tiver menos do que 25 anos, é para casos assim que usaremos as verificações.

#### Como faremos:

> Diremos no código que se a informação for algo faremos algo. <br/>
> Por exemplo: `Se IDADE menor que 25 então ... Fim Se`
>
> _Neste exemplo se a idade for menor do que 25 algo será feito._

> 🆙 [Ciclo 01 Etapa 002: Arquitetura de computadores](./ciclo-01-002-Arquitetura-De-Computadores.md)<br/>
> A CPU de um computador executará as instruções de modo sequencial, buscando na memória RAM (ou mais precisamente na CACHE) os dados e se comunicando com os periféricos.<br/>
> Então se você parar para pensar por alguns minutos perceberá que as verificações criam trechos de código que precisarão ser "pulados" pelo processador, como o processador consegue pular os trechos dependendo do resultado das verificações❓- Isso é possível porque mesmo que "escondido" existem comandos de baixo nível que ajudam a fazer uma verificação funcionar, logo um comando `Se` é uma forma simplificada que foi criada para fazer algo que leva um conjuntos de outros comandos em linguagem de máquina.
>
> __Para isso damos o nome de abstração!__

### Repetições

Agora imagine que você receberá a idade de 10 usuários, você terá que escrever as mesmas cinco linhas de comandos 50 vezes? 😕 É claro que não, para isso existe o comando para executar repetições 🥹

#### Como faremos:

> Diremos no código que o trecho será repetido até uma condição ser atendida. <br/>
> Por exemplo: `Repetir até 10 usuários ... Fim Repetir`
>
> _Neste exemplo o trecho seguinte será repetido 10 vezes._

> 🆙 [Ciclo 01 Etapa 003: Plataformas](./ciclo01-003-Plataformas.md)<br/>
> Quando estudamos as plataformas vimos diversos dispositivos e agora vendo o comando de repetição pense por alguns minutos: Você conhece algum equipamento que é ligado, executa uma determina ação e desliga logo em seguida automaticamente? 🤨
>
> Na vida real fora dos exercícios didáticos de um curso equipamentos não podem funcionar e desligar, isso gera uma experiência de uso ruim. Neste ponto espero que já tenha fico claro a importância do comando de repetição para manter softwares aguardando instruções ou monitorando algo.


### Conclusão

Nesse conteúdo vimos um pouco sobre o que é lógica e como ela é aplicada na programação de software, também definimos os comandos que usaremos no nosso pseudocódigo. Apesar de não tem muito conteúdo, foi uma etapa importante para o passo programar nossas lógicas e buscamos fazer correlações entre os assuntos que vimos até aqui e como eles estão sendo aplicados.

Agora é com você! 👊
Nas atividades de fixação deixarei várias propostas de softwares para você criar a lógica, não se incomode com os formalismos, tente seguir as regras que estabelescemos e concentre-se em construir comandos com coerência e detalhados. __Lembre-se que quando estiver programando você fará algo bem parecido com isso, então leve essas atividades a sério!__

Vou deixar aqui um exemplo para caso tenha ficado alguma dúvida sobre como começar:

__Proposta:__ Criar um software que leia a idade, o nome, o sexo e o estado cívil de uma pessoa e responda adequadamente cumprimentando o usuário. 

```
INICIO
  Repetir até o usuário digitar "sair"
    Exibir "Informe seu nome: "
    Guardar em NOME
    Exibir "Informe sua idade: "
    Guardar em IDADE
    Exibir "Informe seu sexo (M - Masculino ou F - Feminino): "
    Guardar em SEXO
    Exibir "Informe seu estado cívil (S - Solteiro ou C - Casado): "
    Guardar em ESTADOCIVIL

    Se SEXO igual a "M" então
      Se ESTADOCIVIL igual a "S" então
        Se IDADE maior ou igual a 40 então
          Guardar em TITULO o texto "Senhor"
        Fim Se
      Fim Se

      Se ESTADOCIVIL igual a "C" então
        Guardar em TITULO o texto "Senhor"
      Fim Se
    Fim Se

    Se SEXO igual a "F" então
      Se ESTADOCIVIL igual a "S" então
        Se IDADE maior ou igual a 40 então
          Guardar em TITULO o texto "Senhora"
        Fim Se

        Se IDADE menor que 40 então
          Guardar em TITULO o texto "Senhorita"
        Fim Se
      Fim Se

      Se ESTADOCIVIL igual a "C" então
        Guardar em TITULO o texto "Senhora"
      Fim Se
    Fim Se

    Exibir "Olá " + TITULO + NOME

  Fim Repetir
FIM
```
#### DICAS

- Escreva o texto que vêm depois do comando `Guardar em` em maiusculo

- Use `""` para diferenciar o que é texto do comando, para o que é um texto digitado pelo usuário

- Respeite o recuo da margem esquerda. Isso se chama identação e ajuda a identificar quais comandos estão dentro de quais

- Lembre-se:

   - Deve ter apenas uma ação (verbo) por linha

   - Comece seu grupo de comandos com INICIO e termine eles com FIM


## FIXAÇÃO

### Atividade 01

__Proposta:__ Criar um programa que permita ao usuário organizar suas listas de receita culinárias de família.

### Atividade 02

__Proposta:__ Criar um programa para que duas pessoas possam jogar Jokenpo (o famoso pedra, papel e tesoura)

### Atividade 03

__Proposta:__ Criar um programa para que duas pessoas possam jogar o jogo da velha

### Atividade 04

__Proposta:__ Criar um programa para que o usuário possa planejar uma viagem e decidir se ficará caro ou não

### Atividade 05

__Proposta:__ Criar um programa para que o usuário possa organizar um cronograma de estudo respeitando um limite de horas de estudo por dia

### Atividade 06

__Proposta:__ Criar um programa que funcione como um carrinho de compra online recebendo produtos e exibindo o valor total da compra

### Atividade 07

__Proposta:__ Criar um programa que funcione como uma calculadora com as quatro operações básicas (soma, subtração, multiplicação e divisão)

### Atividade 08

__Proposta:__ Criar um programa que receba uma lista de números inteiros e ajude o usuário a organizar esses números em ordem crescente

### Atividade 09

__Proposta:__ Criar um programa que receba o valor de uma comanda de bar e ajude os usuário a dividir a conta entre as pessoas da mesa considerando uma taxa de cover e os 10% da taxa de serviço

### Atividade 10

__Proposta:__ Criar um programa que implemente a cifra de Cesar, recebendo uma palavra e um número inteiro e exibindo a palavra cifrada.

💡A [cifra de Cesar](https://pt.wikipedia.org/wiki/Cifra_de_C%C3%A9sar) é uma forma de criptografar uma palavra, você pega cada letra da palavra e substitui pela letra X posições depois (para isso serve o número inteiro que será recebido).

__Dica__: Usando a tabela [ASCII](https://www.ascii-code.com/pt) que tem um valor numerico que corresponde a cada letra, fica mais simples implementar a cifra de cesar 🤓

---
---
---

<div style="text-align: center;">

   [<<< Anterior: Plataformas](./ciclo01-003-Plataformas.md) ::::::::::::: [Próximo: Lógica de Programação >>>](./ciclo01-004-Lógica-De-Programação.md)

</div>