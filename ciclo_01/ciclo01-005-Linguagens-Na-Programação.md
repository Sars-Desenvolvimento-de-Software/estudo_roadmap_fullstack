# Ciclo 01: Linguagens na Programação

Usamos uma pseudolinguagem até agora para gerar nossos pseudocódigos, porém veremos a partir de agora as linguagens existentes na programação e teremos uma noção geral sobre quais sãos os tipos de linguagens que existem e seus características. Você também verá que não é apenas a linguagem de programação que existe e que muitas vezes você precisará usar do que uma linguagem para ser capaz de criar um projeto.

## Conteúdo

> ### Estilização

As linguagens de estilização são linguagens cujo objetivo é apenas implementar alterações em aspectos visuais de componentes que serão usados na interface gráfica do usuário. Falando em outras palavras, você não usará elas para criar funcionalidades, mas são elas que fazendo um botão ter uma cor específica ou a borda arredondada.

Alguns exemplos de linguagens de estilização são:

### CSS (Cascading Style Sheets)

É a principal linguagem de estilização para web, permitindo definir para página HTML layouts e como a aparência será.

Exemplo: 
```
.botao {
  width: 100%,
  color: #fff,
  backgroud-color: #000
}
```

### SASS (Syntactically Awesome Style Sheets)

É uma estensão do CSS que adiciona funcionalidades que complementam os recursos do CSS. É chamada de linguagens de pré-processamento, pois ao gerar o código final o que é gerado a partir do SASS é o CSS.

Exemplo: 
```
$cor-branco: #fff;
$cor-preto: #000;
.botao {
  width: 100%;
  color: $cor-branco;
  backgroud-color: $cor-preto;
}
```

> ### Marcação

As linguagens de marcação sçao usadas para estruturar o conteúdo de um documento (seja uma página web, uma tela de aplicativo ou um documento texto).

Ela define elementos e hierarquia, mas não implementa funcionalidades.

### HTML (HyperText Markup Language)

É a linguagem padrão usada para estrututar páginas web, permitindo específicar os elementos da tela e sua hierarquia.

Nas última versão o HTML se preocupou em trazer formas de dar sentido ao que se estrutura e facilitar assim para que pessoas e mecanismos de busca consigam ler a página web. Isso é chamado de semântica.

Exemplo: 
```
<body>
  <header>
    <img></img>
  </header>
  <main>
    <h1>Título da página</h1>
    <p>Parágrafo da página!</p>
  </main>
</body>
```

### XAML (eXtensible Application Markup Language)

É uma linguagem usada pela Microsoft para criação de interfaces gráficas na tecnologias WPF e Xamarin, criando as interfaces de modo declarativo.

Exemplo: 
```
<Button content="Clique aqui!" width="100" Height="50"/>
```

> ### Configuração

São linguagens usadas para definir parâmetros e configurações que uma aplicação pode usar facilitando ajustes parametrizáveis sem a necessidade de alteração do código-fonte da aplicação.

### YAML (YAML Ain't Markup Language)

Usada em DevOps e CI/CD para definir as configurações de ambiente e processos de automação. Usa identação para estabelecer hierarquia e é muito usada por ferramentas como Docker Compose e Ansible.

Exemplo: 
```
site_permitido: https://site.com
```

### JSON (JavaScript Object Notation)

Originalmente derivada da forma que a linguagem JavaScript trata seus objetos, essa linguagem passou a ser muito usada em arquivos de configuração por ser legível e fácil de manipular usando JavaScript. É muito usada em aplicações Web.

Exemplo: 
```
{
  "site_permitido": "https://site.com"
}
```

> ### Transferência de dados

São linguagens e formatos que permitem transferir dados e trocar informações usando um padrão fácil de processamento.

### JSON (JavaScript Object Notation)

Novamente o JSON está aqui! 😄

Amplamente usada para transferência de dados pela internet devido a sua simplicidade e compatibilidade com várias outras linguagens (por terem bibliotecas para processamento de JSON).

Exemplo: 
```
{
  "nome": "Pedro Augustus",
  "idade": "55",
  "filhos": ["Lucas", "Barbara"]
}
```

### XML (eXtensible Markup Language)

Apesar de mais complexo e verboso do que o JSON, o XML ainda é usado para transferência de dados em algumas aplicações que seguem o padrão SOAP (padrão usado em algumas Web APIs mais antigas).

Exemplo: 
```
<dados>
  <nome>Pedro Augustus</nome>
  <idade>55</idade>
  <filhos>
    <filho>Lucas</filho>
    <filho>Barbara</filho>
  <filhos>
</dados>
```

> ### Consultas

São linguagens usadas para gerenciamento e consulta de dados em um banco de dados.

### SQL (Structured Query Language)

Linguagem padrão para usar em banco de dados relacionais (banco baseados em entidades e relacionamentos entre os dados normalizados).

Exemplo: 
```
Select * from Tabelas a where a.ID = 1;
```

> ### Scripts

Essas linguagens são voltadas para automatizar tarefas e executar comandos dentro dos sistemas operacionais.

### Bash ou Shell Script

Linguagem padrão dos sistemas operacionais baseados em Linux, e permitem criar arquivos, percorrer diretórios, excerrar processos em execução pelo sistema operacional, etc.

Exemplo: 
```
#!/bin/bash
echo "Texto impresso no terminal!"
```

### CMD ou PowerShell 

Linguagem padrão do sistema operacional Windows e seu funcionamento do ponto de vista do usuário é semelhante ao do Bash.

Exemplo: 
```
Write-Output "Texto impresso no console!"
```

> ### Programação

Finalmente chegamos nas linguagens de programação, as responsáveis por dar vida as aplicações implementando funcionalidades.

Dentre as linguagens que existem na programação esse grupo é o que tem maior variedade e quantidade de linguagens. Algumas focadas em desenvolvimento de aplicações, outras em execuções de pequenas rotinas, outras ainda focadas em perfomance.

### JavaScript

Linguagem padrão das aplicações web e reconhecida por todos os navegadores. Foi criada inicialmente para proporcionar interatividade a páginas web, porém com suas evoluções atualmente atende a uma grande variedade de objetivos.

Exemplo: 
```
console.log("Olá estudante!");
```

### Java

Linguagem robusta que é independente de plataforma. Muito usada em desenvolvimento de softwares corporativos, aplicativos android e web services que precisam ser capazes de suportar alta carga.

Exemplo: 
```
public class TESTE {
  public static void main(String[] args) {
    System.out.println("Olá estudante!");
  }
}
```

### Python

Linguagem com foco em simplicidade e legibilidade do código-fonte. Inicialmente foi criada para execução de tarefas menores e sem interface gráfica, porém atualmente evoluiu para atender vários cenários ficando muito famosa em processamento de grandes quantidades de dados e inteligência artificial.

Exemplo: 
```
print("Olá estudante!");
```

### C/C++

Linguagem de baixo nível conhecida por sua performance e controle sobre o hardware. É amplamente usada em softwares de alto desempenho como jogos e dispositivos embarcados.

Exemplo: 
```
#include <iostream>
int main() {
  std::cout << "Olá estudante!" << std::endl;
  return 0;
}
```

### Conclusão

Como foi possível ver existem muitas linguagens além da linguagem de programação e espero que pelas descrições resumidas tenha sido possível perceber que em projetos reais você não usará apenas uma linguagem, mas terá que usar uma combinação de várias para chegar ao comportamento esperado.

Há muito o que estudar para ser programador, e mais ainda para se tornar um FullStack, porém nada que não possa ser aprendido com persistência, dedicação e dando tempo ao tempo 👊

## FIXAÇÃO

### Atividade 01

Escolha a linguagem ou o conjunto de linguagens que melhor atendem a necessidade abaixo:

__Proposta:__ Você precisa criar um site com design personalizado e responsivo.

### Atividade 02

Escolha a linguagem ou o conjunto de linguagens que melhor atendem a necessidade abaixo:

__Proposta:__ Você precisa automatizar uma rotina da sua empresa que leva muito tempo sendo feita por uma funcionária. Todos os dias ela precisa verificar se existem notas fiscais geradas em uma pasta (que os vendedores colocam), copiar o nome do cliente, a chave da nota fiscal e alimentar um arquivo texto com essas informações.

### Atividade 03

Escolha a linguagem ou o conjunto de linguagens que melhor atendem a necessidade abaixo:

__Proposta:__ Você foi contratado por uma empresa para desenvolver um sistema para monitorar via câmeras de vídeo todos que entram e saem do estabelecimento.

---
---
---

<div style="text-align: center;">

   [<<< Anterior: Lógica de Programação](./ciclo01-004-Lógica-De-Programação.md) ::::::::::::: [Próximo: Linguagem de programação >>>](./ciclo01-006-Linguagem-De-Programação.md)

</div>