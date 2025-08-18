

## Aula 31/07

## Princípios de projeto de código
Código deve ser simples e fácil de manter. Evitar repetição e garantir que cada função tenha uma única responsabilidade (coesão). Manter baixo acoplamento entre módulos. Não criar funcionalidades desnecessárias. 


## Padronização de código
Padronizar o estilo e o formato do código facilita sua leitura e manutenção. É importante usar nomes consistentes para variáveis, funções e classes, além de manter uma indentação e espaçamento uniformes. Comentários claros e objetivos também fazem parte da padronização. Ferramentas como linters e formatadores ajudam a aplicar essas regras automaticamente. Seguir as convenções da linguagem ou do projeto melhora a colaboração entre equipes e reduz a chance de erros.
  


## Ocultamento de Informação
Ocultamento de informação consiste em esconder os detalhes internos de um módulo ou classe, expondo apenas o necessário. Isso reduz o acoplamento, facilita a manutenção e protege os dados contra acesso indevido. É fundamental para criar sistemas modulares e seguros.

  

## Aula 04/08

## Coesão
Atributo/Caracteristica que buscamos no nosso sistema, toda classe deve implementar uma única funcionalidade ou serviço.

Vantagens da Coesão:
- Facilita a implementação de uma classe, bem como o seu entendimento e manutenção.
- Facilita a alocação de um único responsavel por manter uma classe.
- Facilita o reúso e teste de uma classe. 

## Acoplamento

Acoplamento é a força da conexão entre duas classes. Apesar de parecer simples, o conceito possui algumas nuances, as quais derivam da existência de dois tipos de acoplamento entre classes: acoplamento aceitável e acoplamento ruim.
 
As recomendações sobre acoplamento e coesão são reunidas em uma única recomendação:
"Maximize a coesão das classes e minimize o acoplamento entre elas."



## SOLID

  ## Princípio da Responsabilidade Única: 
  
  Uma classe deve ter uma única responsabilidade, ela deve ter um único motivo para mudar, com o obejtivo de manter a coesão do código, separando responsabilidades distintas em diferentes classes.

  ## Princípio da Segragação de Interfaces: 
  
  Elas devem ser específicas para o cliente onde nenhuma classe deve ser forçada a depender de métodos que não utiliza, para aumentar a coesão das interfaces e evitar dependências desnecessárias.

  ## Princípio de inversão de Dependencias: 
  
  Esse princípio recomenda que uma classe cliente, deve estabelecer dependências prioritariamente com abstrações e não com implementações concretas.
  A ideia é então trocar ou inverter as dependências: em vez de depender de classes concretas, clientes devem depender de interfaces.Portanto, um nome mais intuitivo para o princípio seria Prefira Interfeces a Classes.

  ## Prefira Composição a Herança

 Prefira composição em vez de herança para reutilizar código, pois composição cria menos acoplamento e é mais flexível. Herança expõe detalhes internos, dificultando manutenção, enquanto composição permite trocar partes do objeto facilmente. Use herança só quando houver uma verdadeira relação de "é-um".


 ## Princípio de Demeter 

- Tambem chamada de Princípio do Menor Conhecimento defende que a implementação de um método deve invocar apenas os seguintes outros métodos:
  - de sua própria classe (caso 1)
  - de objetos passados como parâmetros (caso 2)
  - de objetos criados pelo próprio método (caso 3)
  - de atributos da classe do método (caso 4)

  ## Princípio Aberto/Fechado

  - Uma classe deve estar fechada para modificações e aberta para extensões,ou seja deve ser possível adicionar novos comportamentos sem alterar o código existente, usando herança, interfaces ou padrões de projeto. 
Isso torna o sistema mais flexível e fácil de manter.


 ## Princípio de Substituição de Liskov

O Princípio de Substituição de Liskov (LSP) diz que uma subclasse deve poder substituir sua superclasse sem alterar o comportamento esperado do programa. 
 - Isso significa que os métodos da subclasse devem manter o mesmo contrato da superclasse.
 - Se isso não for respeitado, o uso da herança pode causar erros e comportamentos inesperados.


  

