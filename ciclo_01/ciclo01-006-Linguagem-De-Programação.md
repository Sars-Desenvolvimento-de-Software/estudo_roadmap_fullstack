# Ciclo 01: Lógica de Programação

Agora vamos falar especificamente das linguagens de programação e suas características. Entender alguns aspectos que diferencial elas e um pouco do que as torna semelhantes.

O primeiro passo é entender que as linguagens de programação foram evoluindo ao longo das decadas e a principal alteração foi a proximidade da linguagem com a nossa linguagem natural, ou no caso com o inglês que é o idioma mais comum entre as linguagens na programação.

Isso nos permite classificar as linguagens de programação por nível de abstração, sendo linguagens de baixo nível, intermediário e alto nível. Quanto mais próxima da linguagem de máquina mais baixo nível, e quanto mais próxima da linguagem humana mais alto nível.

## Conteúdo

> ### Tipagem

Uma linguagem de programação pode ser classificada pela forma que decide trabalhar o gerenciamento de variáveis durante sua execução.

Linguagens que exigem que o tipo de um dado seja definido antes de usa utilização são chamadas fortemente tipadas e sua principal característica é que uma variável criada para receber data não pode receber outro tipo.

Linguagens que não exigem esse controle sobre o tipo de uma variável são chamadas linguagens fracamente tipadas, e diferente da outra classificação, aqui se uma variável criada receber uma data ela será do tipo data apenas enquanto seu valor não for alterado.

> ### Geração do código final

Linguagens de programação podem ser classificadas pela forma que geração o código de máquina para serem executados pelo dispositivo.

Linguagens que geram o código de máquina que fica em um arquivo do tipo executável são chamadas linguagens compiladas, pois o processo de transforma o código da linguagem em código de máquina é feito separadamente no processo de compilação e depois disso o arquivo executável pode ser usado sempre que desejar.

Linguagens que não geram arquivos executáveis e são lidos e convertidos no momento da sua utilização pelo dispositivo são chamadas de linguagens interpretadas.

> ### Gerenciamento de memória

O gerenciamento de memória é outra característica de uma linguagem que pode fazer o gerenciamento pelo programador ou deixar que ele mesmo faça.

Devido a complexidade desse gerenciamento e aos erros que falhas podem ocasionar (travando computadores ou corrompendo a memória) se tornou padrão linguagens de alto nível (que são mais recentes) usarem o auto gerenciamento (chamado de Garbage Colletion).

Linguagens de baixo nível ou de alta performance ainda permitem que o desenvolvedor faça esse gerenciamento.

Na prática o Garbage Colletion fica monitorando a memória e quando uma variável cai em desuso, ele desaloca o espaço na memória permitindo ao Sistema Operacional reusar o espaço. Caso isso não seja feito, a memória RAM de um computador acabaria e o computador travaria.

> ### Paradigmas

Paradigmas são formas de abstrair (pensar em um problema trazendo ele do mundo real para o código) o problema que se deseja solucionar. Existem alguns paradigmas e dependendo do paradigma a linguagem de programação deve ter recursos que a permitam se adaptar.

Portanto, algumas linguagens usam paradigmas expecíficos e outras optaram duraante sua evolução a múltiplos paradigmas, são as chamadas linguagens multiparadigmas.

O paradigma imperativo permite ao usuário desenvolver seu código-fonte como sendo um conjuntos de ordens dadas a um computador que serão executadas sequencialmente.

O paradigma modular permite ao usuário desenvolver seu código-fonte como se ele fosse um conjunto de peças de lego que se comunicam e constroem as funcionalidades desejadas.

O paradigma Orientado a Objetos permite ao usuário desenvolver seu código-fonte como se ele fosse um conjunto de objetos com responsabilidade bem definidas. A comunicação entre esses objetos é que criam os comportamentos esperados para o sistema.

### Conclusão

Assim que começamos a nos aprofundar em linguagens de programação podemos ver que existem várias características que podem indicar uma linguagem ou outra como melhor para atender uma certa necessidade.

Todos esses pontos são ser melhor detalhados em uma oportunidade futura enquanto usamos uma linguagem de programação específica, porém é importante você já compreender que essas características existem e refletir um pouco sobre o que você concluí a partir delas.

## FIXAÇÃO

Não há

---
---
---

<div style="text-align: center;">

   [<<< Anterior: Linguagens na programação](./ciclo01-005-Linguagens-Na-Programação.md) ::::::::::::: [Próximo: Algoritmos >>>](./ciclo01-007-Algoritmos.md)

</div>