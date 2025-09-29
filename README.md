

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


  ## Aula Dia 28/08

  ## Características da arquitetura
  
  Características da Arquitetura = Requisitos Não Funcionais
  Nos dias de hoje o principal foco é na segurança do site, pois se a segurança não for boa compromete não so o site como informações de clientes. 
  
 - Disponibilidade    - Confiabilidade    - Testabilidade    - Escalabilidade
 - Segurança    - Agilidade    - Tolêrancia a falhas    - Elasticidade
 - Recuperabilidade    - Desempenho    - Implementabilidade    - Capacidade de aprendizagem
    
  ## Princípios do design

  Sempre que possível, utilize a mensageria assíncrona entre os serviços para aumentar o desempenho. 

  Um princípio é o da comunicação. 

  ## Estrutura

  


  ## Decisões de arquitetura

  As decisões de arquitetura são quando você define como será sua arquitetura, qual modelo que será usado (python, java, etc..).

 Microseviço - busca reduzir o acoplamento 


## Aula 01/09


## Expectativas de um Arquiteto

- Tomar decisões de arquitetura 
- Analisar continuamente a arquitetura
- Manter-se atualizado com as últimas tendências
-  Assegurar a conformidade com as decisões
-  Ter conhecimento sobre domínio do negócio
-  Ter habilidades interpessoais
-  Entender e lidar bem com questões políticas

## Tomar decisões de arquiteto

Orientação é a palavra de ordem nessa primeira expectativa , framework reativo para o desenvolvimento web front-end 
Ele deve ser o guia da equipe, o cara mais experiente que já passou por tudo dentro de empresa. 

Ele deve analisar continuamente a arquitetura e o ambiente de tecnologia atual.

## Manter-se Atualizado com as Últimas Tendências 

Um arquiteto deve ficar atualizado com as últimas tendências da tecnologia e do setor. 

Ele não precisa dominar tudo, porem deve estar por dentro de todas as mudanças nas tecnologias mundiais. 

## Assegurar a Conformidade com as Decisões 

Um arquiteto deve assegurar a conformidade com as decisões de arquitetura e os princípios de design.

## Ter Habilidades Interpessoais 

Um arquiteto deve ter habilidade interpessoais excepcionais, inclusive trabalho em equipe, facilitação e liderança.

## Operações/DevOps

DevOps é a prática que integra desenvolvimento e operações para entregar software mais rápido, com qualidade e adaptável às mudanças. 

Ele não resolve todos os problemas na primeira semana, ele leva tempo porem ele vai melhorando cada vez mais. 


## Aula 04/09

- Arquitetura de software define a estrutura geral do sistema e trata de decisões de alto nível, como a organização dos componentes e as tecnologias usadas.

- Design de software foca nos detalhes de implementação dentro desses componentes, como algoritmos, classes e métodos.

- A Arquitetura é o formato geral do sistema e o design é o detalhamento interno.

------------------------------------------------------------------------------------------------------------

 O arquiteto modelo T tem uma visão generalista e tambem possui uma capacidade técnica em certas áreas, permitindo-o atuar em diferentes times e ainda tem autoridade técnica em assuntos críticos.  


 ## Aula 08/09 

 ## Trade OFF
 
 Refere-se a necessidade de equilibrar decisões.
 
 Trade-off é igual o sistema de um leilão.
 
 Da pra fazer um leilão com um banco de dados, porém se o leilão estiver acontecendo em apenas um lugar e não em varios ao mesmo tempo. 


Brokers:
- apache kafka
- rabbitmq
- AWS SNS
- Azure ServiceBus

  Protocolo de Rede:
  - AMQP
  - Web socket
  - MQTT

## Topico
Alguem publica e todos recebem a mensagem, como um alerta de promoção em um aplicativo que você liberou seus dados ou uma mensagem de whatsapp.
Porém se por algum acaso o Rastrear Lance perder a conexão pois a bateria do celular acabou ou algo do tipo,ele não recebe mais aquela mensagem. 
Publisher - Publica 
Senders - Envia 
Receiver - Recebe

## Fila:
Pooling é você pedir para receber a mensagem. 
A mensagem é um para um, diferentemente do outro topico que a mensagem era 1 para n (igual em um grupo de familia).
Senders e Receiver

A diferença do Fila pro Tópico seria que na fila tem um maior acoplamento.
Se você tiver a necessidade de mensagens mais diretas o fila é o mais recomendado. 

Buffer - as mensagens ficam armazenadas na fila, para caso de problema na conexão de alguns dos consumidores eles consigam resgata-las.

----------------------------------------------------------------------------------------------------------------------------------------------

## Aula 11/09



