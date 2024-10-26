# Ciclo 01: Plataformas

Agora que você já sabe o básico de computadores e que eles não estão limitados ao computador tradicional que temmos em casa ou no trabalho, vamos conhecer sobre as plataformas disponíveis e que todo desenvolvedor deve conhecer.

O assunto será abordado de modo superficial ainda, porém você terá uma boa visão macro que te ajudará a entender a ampla ganha de plataformas que um desenvolvedor pode destinar seu programa e algumas características de cada uma.

## Conteúdo

> #### Computadores de Área de Trabalho

Computadores de Área de Trabalho ou Computador Pessoal (PC) ou Desktop 🖥️ estes são os nomes usados para o tradicional computador que costumamos ter em alguma escrivaninha em nossa casa e que de modo geral usado para trabalhar ou jogar games, uma vez que os smartphones já dominaram o mundo e são muito mais práticos para uso corriqueiro.

Esses computadores costumam ter um poder de processamento mediano, mas tem como vantagem a possibilidade de ampliar seus recursos substituindo ou adicionandos novas peças internas (memória, processador, periféricos), e isso o torna uma ótima opção se o usuario conhece sobre manutenção de computadores.

Neste grupo também estão dos notebooks ou laptops (nomes que referenciam o mesmo equipamento) 💻, porém como os notebooks são criados para dar ênfase a portabilidade, geralmente eles exigem ferramentas e um conhecimento maior caso o usuário decida fazer alguma manutenção.

📹 Se aprofunde mais sobre o tema vendo o [VÍDEO - Nerdologia](https://www.youtube.com/watch?v=Vb0iORewZDA)

#### Sistemas Operacionais

O sistema operacional (SO) é o software mais importante de qualquer equipamento. O SO é responsável por todo gerenciamento das partes do dispositivo, além de controlar toda comunicação da parte física com softwares que rodam no dispositivo. Ou seja, sem os SOs os dispositivos não teriam evoluido, já que todos programador teria que conhecer de linguagens de máquina para conseguir rodar qualquer coisa no computador.

Para ter uma visão mais nítida sobre o que é o SO e sua importância, imagine ele como um gerente que tem todas as chaves dos setores de uma empresa. É esse gerente que abre a empresa para que os funcionarem entrem, é ele quem liga a eletricidade, é ele quem abre e tranca cada uma das portas sempre que alguém quer entrar ou sair dos setores, sem ele basicamente nada funciona na empresa, nem mesmo saber a hora seria possível.

Vários SOs foram criados e se popularizaram, sendo o Windows o mais famoso, porém a lista é grande:

- Windows: Microsoft, pago
- macOS: Apple, pago e excluivo para computadores da Apple
- ChromeOS: Google, gratuito
- Ubuntu: Canonical, gratuito
- etc...

📑 E essa lista segue com vários outros sistemas operacionais com foco em usabilidade, interface gráfica, recursos de segurança, entre outros... veja mais no [TEXTO - Wikipédia](https://pt.wikipedia.org/wiki/Sistema_operativo#Para_desktop/servidores)

📹 E saiba um pouco mais com o [VÍDEO - Código Fonte TV](https://www.youtube.com/watch?v=5by78s9rv2s)

Para um desenvolvedor de software é importante entender que apesar de todos os sistemas operacionais executarem um conjunto de ações comuns para o gerenciado do computador, cada sistema operacional possui sua forma de fazer isso (não vamos nos aprofundar nos casos de SOs que por semelhanças no seu funcionamento "tem formas iguais de fazer as coisas" - Neste momento assuma que cada SO se comunica de uma forma peculiar) e por isso ao desenvolver um software você deve considerar em quais SOs essa aplicação será executada.

#### Arquitetura Desktop

Quando pensamos em arquitetura para Desktops estamos pensando em aplicações monolíticas ou sistemas distribuídos em sua grande maioria. Em uma visão superficial, uma aplicação do tipo monolito é uma aplicação que foi construida como uma bloco único de código com todas as funcionalidades necessárias dentro desse bloco, e uma aplicação distribuída é uma aplicação que é composta por dois ou mais blocos que juntos conseguem entregar um resultado esperado.

Simplificando um pouco mais com exemplo: 

Imagine que você criou um programa e instalou no seu computador, esse programa deve ser capaz de ler várias pastas salvas em uma unidade de armazenamento (pendrive, CD, HD externo o que você desejar) e organizar isso em uma lista por categoria e em ordem alfabética.

Se seu programa instalado lê as informações dessa unidade, processa os dados e gera as lista para você em aproximadamente duas horas devido ao grande volume, você tem um monolito! Porque independente de como você organizou seu código, todas as funcionalidades estão sendo executados apenas por seu programa (que podemos ver como um bloco único).

Agora pense que duas horas é muito tempo, e você precisa que esse mesmo resultado (a lista categorizada) esteja pronta em menos de 40 minutos... um baita desafio! O que fazer? 😕

Você começa tentar encontrar formas de fazer seu programa rodar mais rápido, e até consegue uma melhoria após alguns ajustes (não vamos nos aprofundar nos possíveis ajustes, isso é um tema avançado para o momento) e chega ao tempo de execução de 1 hora e 20 minutos, porém ainda está longe do máximo definido de 40 minutos. Então você tem uma ideia genial 💡 "E se eu colocar três computadores para trabalhar juntos?" - Pronto aqui nasce a ideia do sistema distribuído.

Essa ideia exige que você invista um tempo considerável alterando sua aplicação para trabalhar sabendo como dividir as tarefas, como se comunicar com outros computadores, como reunir os resultados individuais e por fim como entregar isso de maneira segura para o usuário (escrevi isso para enfatizar que não é algo sem esforço para ser feito). Ao final desse processo, você instalou seu programa em três computadores e conseguiu colocar eles para trabalharem em sincronia dividindo o processamento e gerando a lista categorizada em 25 minutos.

Espero que tenha fica claro as diferenças das arquiteturas e suas principais características, e além disso é importante destacar que aplicações monolíticas são a maioria dos casos, pois em geral as aplicações não precisam processar volumes enormes de dados de uma vez, mas em casos de processamento massivo de dados (uma empresa de armazenamento de arquivos, um data center com milhões de dados ou processamento de dados cientificos como genoma de espécies) a arquitetura distribuida em rede acaba compensando o esforço de implementação.

Estava quase esquecendo, mas uma ótimo exemplo de arquitetura distribuída que não tem foco em processamento, mas em comunicação, são as aplicações de jogos em rede local ou um chat interno de uma empresa (que execute dentro da rede local).

📑 Explore mais no [TEXTO - DevTo](https://dev.to/otaviovb/arquitetura-monoliticos-monoliticos-distribuidos-e-microsservicos-3epc)

📹 Veja mais em [VÍDEO - Código Fonte TV](https://www.youtube.com/watch?v=CsrHHHPHKwE)

📹 Veja mais em [VÍDEO - Prof. Bruno Clemente](https://www.youtube.com/watch?v=nHU8gl-ovwQ)

> #### Dispositivos móveis

Os dispositivos móveis são um grupo que inclui equipamentos com capacidade computacional alta e que permitem as mesmas funcionalidades de um computador, porém em um dispositivo que cabe na palma da sua mão. Os mais famosos são os smartphones 📱, mas existem tablets, e atualmente até smartwatches ⌚ podem entrar nessa lista, sendo uma tecnologia inovadora de um subgrupo chamado de wearables, que são os dispositivos "vestíveis".

É importante destacar que o grupo de dispositivos móveis devem ter dispositivos que permitam uma interação envolvendo muitas funcionalidades que um computador teria, então por exemplo um relógio inteligente que permite pagar por aproximação, acessar a internet, responder uma mensagem, controlar uma agenda, fazer ligações e cronometrar algo, já não é mais apenas um relógio haha

Porém, isso não significa que se você comprar um relógio com cronometro e acompanhamento de batimentos cardiacos, você possa considerar ele na categoria de dispositivos móveis, pois suas funcionalidades são bem especificas, e ele se encaixa no grupo de embarcados que veremos mais adiante.

📑 Explore mais no [TEXTO - Wearables](https://usemobile.com.br/wearable/)

📹 Explore mais no [VÍDEO - Celulares](https://www.youtube.com/watch?v=LM2wSf5NL_A)

#### Sistemas Operacionais

Assim como nos computadores, os SOs aqui tem o mesmo propósito (gerenciar o hardware e ser uma ponte para os aplicativos). Dentros os sistemas operacionais mais famosos estão o iOS da Apple e o Android do Google. Assim como ocorre para os computadores Desktops, o desenvolvedor deve decidir para quais SOs o seu software será criado.

Como os Smartphone se popularizam, o interesse por facilitar o desenvolvimento de aplicativos aumentou e tecnologias foram criadas para permitir que com poucos ajustes uma aplicação criada para Android possa ser executada também no iOS e vice-versa. Porém, lembre-se que não existem fórmulas mágicas e portanto toda tecnologias tem suas vantagens e desvantagens, falaremos mais sobre isso em tópicos futuros.  

#### Arquitetura Mobile

Quando se trata de desenvolvimento para dispositivos móveis precisamos considerar as características do dispositivo, por exemplo: Um smartphone não tem mouse e teclado, mas tem touch screen; um smartwatch tem uma tela minuscula logo não é possível ler da forma que faríamos em um monitor de computador.

Sendo assim as aplicações mesmo sendo monolíticas tem preocupações na usabilidade e desempenho que as aplicações em desktops não precisam ter (não entraremos no mérito da importância das otimizações para desktop), então pense em aplicações leve tanto para processamento quanto para armazenamento quando pensar em desenvolver algo para essa plataforma.

Uma outra opção que se popularizou entre os desenvolvedores foi a arquitetura cliente-servidor. Nesta arquitetura o aplicativo é projetado pensando que teremos uma interface gráfica instalada nos dispositivos, mas que através da internet todo o processamento será feito em um servidor (computador muito poderoso perdido em algum lugar da internet 😆) e assim conseguimos ter recursos legais em dispositivos móveis desde que esteja conectado a internet.

> #### Em nuvem (Internet)

Até aqui você já sabe um pouco sobre computadores, e viu também que computadores podem ser colocados juntos para se comunicarem e executar tarefas com mais velocidade. Agora pare por alguns minutos e imagine se fosse possível conectar dois computadores que estão distantes? O que seria preciso para fazer isso, uma cabo de rede enorme? mas aí esbarraríamos na perda de sinal após muitos metros, então o que fazer? E se colocarmos outros "computadores" específicos no meio do caminho para processar e repetir o sinal entre esses computadores que querem se comunicar?

Assim nasceu a Web, uma "teia" 🕸️ global de "computadores" (servidores, roteadores, repetidores, e outros) que permitem que um sinal saia de um computador e encontre outro em qualquer parte do mundo que a web esteja conectada. Portanto quando usamos o termo "nuvem" 🌥️, é apenas porque esse termo é melhor que teia e trás a ideia de que não importa do que a nuvem é feita, nossa mensagem será levada por ela até onde precisa chegar.

Certo, mas e de onde surgiu o termo internet? Ele vêm das classificações de redes quando estudamos redes de computadores (ou seja, a forma como os computadores podem se conectar) e lá temos a intranet, que é uma rede fechada para outros computadores deixando a comunicação só no grupinho VIP escolhido de computadores locais, e a Internet, que é uma rede aberta que se comunica com outras redes que possam estar conectadas pela Web.

#### Navegadores

Enquanto os Sistemas operacionais são o gerente geral de qualquer equipamento, o navegador ou browser é a porta de entrada para a internet. Ele é um software específico que tem como função prioritária permitir ao usuário de um computador se comunicar com redes externas, acessando conteúdos (como sites, aplicativos web e arquivos de mídia (vídeo, áudio, imagens)) e traduzindo isso para mostrar em tela.

Podemos "pular" direto no mar (internet) e nadar (pegar dados) sem um navegador, porém não consigo nem imaginar a internet ganhando toda a popularidade que tem atualmente sem eles, já que teríamos que ler textos puros sem códigos que gerem animações, cores chamativas, e lidar com vários pedaços de arquivos ao invés de tudo organizado e visualmente bonito no monitor.

O navegador portanto é um aplicativo importante para qualquer desenvolvedor web que crie sites, blogs ou queira disponibilizar algum conteúdo na nuvem. Os principais navegadores são Firefox da Mozilla, Chrome do Google e Edge da Microsoft, mas há outros e o mais famoso disparado é o Google Chrome. Assim como acontece com os sistemas operacionais os navegadores tem peculiaridades que pode fazer um site rodar bem em um navegador e "quebrar" algo em outro, porém no caso dos navegadores isso é bem mais difícil comparado aos sistemas operacionais.

Explore mais vendo esse [VÍDEO - Browsers](https://www.youtube.com/watch?v=VMHP10hnDQU)

#### Arquitetura Web

Devido a sua natureza de conexão entre computadores e a outros fatores como tamanho da internet que se tornou global e padrões que dizem como a comunicação tem que ocorrer dentro da internet algumas arquiteturas ficaram famosas e se destacaram:

- Cliente/Servidor: A arquitetura mais comum, pois foca na premissa básica da internet "um computador consome recursos disponibilizados por outro". Ou seja, você tem um computador (servidor) na internet que disponibiliza notícias e os computadores (clientes) que desejam conhecer as notícias fazem requisições que são respondidas por ele.

- Sistemas distribuídos: Semelhante ao que ocorreu na plataforma desktop, na web você pode ter um computador que recebe uma solicitação de recurso, porém ao invés dele te disponibilizar os dados diretamente, ele vai solicitar esses dados para outros servidores e só depois te encaminhar. Para você (cliente) quem está te atendendo é o servidor para o qual a requisição foi feita, porém na prática outros servidores foram acionadas.

- Microsserviços: A arquitetura em alta do momento, a bala de prata de alguns haha Essa arquitetura é também uma arquitetura do tipo distribuída, porém ela não apenas solicita recursos de outros servidores, ela na sua essência uma aplicação divida em vários servidores e que com a integração entre eles você tem a funcionalidades desejada.

Vamos simplificar com um exemplo:

Tenho uma aplicação que disponibiliza vídeos e permite aos usuários cadastrados dar uma nota para ranquear os vídeos. Se considerarmos a arquitetura Cliente/Servidor tradicional, eu teria um servidor com os vídeos e um aplicativo que permite fazer o cadastro e salva as notas dadas para os vídeos.

Se considerarmos um sistema distribuído, teríamos um servidor de aplicação com o cadastro dos usuários e que salva as notas e um servidor de arquivos com os vídeos que é acessado pelo servidor de aplicação para disponibilzar ao usuário.

Por fim se considerarmos a arquitetura de microsserviço, teríamos um servidor para receber solicitações, um servidor para realizar o cadastro dos usuários, um servidor para salvar as notas, um servidor para retornar os vídeos ranqueados e um servidor de arquivos com os vídeos, tudo disso se comunicando para funcionar.

📑 Explore mais no [TEXTO - Cliente/Servidor](https://pt.wikipedia.org/wiki/Modelo_cliente%E2%80%93servidor)

📑 Explore mais no [TEXTO - Microsserviços](https://cloud.google.com/learn/what-is-microservices-architecture?hl=pt-BR#what-is-microservices-architecture)

📹 Explore mais no [VÍDEO 1](https://www.youtube.com/watch?v=9xGC195XeAo) 
[VÍDEO 2](https://www.youtube.com/watch?v=r6VxrQA3VkA) 
[VÍDEO 3](https://www.youtube.com/watch?v=SEC-tbKa1KQ) 

> #### Embarcados

Um embarcado é um dispositivo eletrônico que tem integrado um componente que permite fazer alguma função computacional específica e limitada a poucas funcionalidades. Em geral são equipamento para finalidades bem definidas e que possuem poucos recursos de memória e processamento, e portanto devem ser projetados e desenvolvidos visando otimizar esses recursos.

Desenvolvedores que trabalham com embarcados geralmente atual com eletrônicos que usamos no dia a dia (microondas, máquinas de lavar, ar condicionados, entre outros), mas também podem atuar em automações residenciais e robótica (com dispositivos para casas inteligente ou drones por exemplo) ou com equipamentos críticos (hospitalares, módulos de aviação, módulos de maquinários grandes, etc...). 

O nível de conhecimento do hardware é prerrequisito e geralmente não existe um sistema operacional para trazer facilidades no gerenciamento, apenas bibliotecas para comunicação com o dispositivo. O desenvolvimento costuma ser feito em linguagem de baixo nível, para otimizar o uso de memória e outros recursos.

#### Dispositivos

📹 Explore mais vendo esse [VÍDEO](https://www.youtube.com/watch?v=XppU8kKpa6I)

📹 Explore mais vendo esse [VÍDEO](https://www.youtube.com/shorts/o7DMHJKhpws)

📑 Explore mais lendo o [TEXTO](https://embarcados.com.br/o-que-sao-sistemas-embarcados/)

📑 Explore mais lendo o [TEXTO](https://embarcados.com.br/projetos-de-iot-sem-fio-ficaram-mais-faceis/)


#### Arquitetura Embarcada

Não há muita margem para fazer arquiteturas mirabolantes, então geralmente são monolitos por serem softwares com finalidade bem específica, porém o foco na otimazação de recurso é o que torna esse tipo de software tão desafiador de ser criado, só para se ter uma noção, geralmente desenvolvendo para qualquer outra plataforma teremos algumas milhões de unidade de memória, mas em um embarcado pode ser que você só tenha algumas centenas... sim a diferença é gigante 😱 e o gerenciamento exige muito mais controle do programador.   

📹 Explore mais no [VÍDEO](https://www.youtube.com/watch?v=HzYcvUE3bSM)

### Conclusão

Nesse conteúdo vimos sobre as várias plataformas que existem e que os desenvolvedores devem conhecer para decidir para qual plataforma criar sua aplicação. Vimos de maneira macro as características de cada uma e um pouco sobre aspectos arquiteturais.

Existem muitos detalhes que não vimos quando se trata de escolher uma plataforma, porém com essa visão superficial você já sabe diferenciar elas, e assim consegue ter noção do mais importante, se eu quero um aplicativo que rode em tudo, eu tenho que estar disposto a trabalhar muito para atender as características de cada uma, tenho que me acostumar a trabalhar com várias arquiteturas e algumas vezes terei que programar mais de uma vez a aplicação para que funcione em plataformas diferentes. 

Pois é... precisa de muito trabalho para fazer software para todas as essas plataformas 😥


## FIXAÇÃO

### Atividade 01

Crie uma proposta de software, respondendo as seguintes perguntas:

- Qual o objeto do seu software?
- Quais as funcionalidades que ele tem que ter? Pense em ao menos cinco.

Agora pensei em como adaptar seu software para cada uma das plataformas abaixo:

- Desktop
- Mobile
- Web
- Embarcado

Não precisa se preocupar sobre ter que programar de forma diferente ou em detalhes tecnicos, foque apenas em como as funcionalidades devem se comportar em cada plataforma (se precisar adapte a funcionalidade) e se você terá um ou várias partes do software se comunicando.

---
---
---

<div style="text-align: center;">

   [<<< Anterior: Arquitetura de Computadores](./ciclo-01-002-Arquitetura-De-Computadores.md) ::::::::::::: [Próximo: Lógica de Programação >>>](./ciclo01-003-Plataformas.md)

</div>