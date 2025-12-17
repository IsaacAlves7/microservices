# 📦 Microservices 
<img src="https://img.shields.io/badge/Medium-Microservices-5B4638?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Microservices-5B4638?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/DEV-Microservices-976857?style=flat&logo=dev.to&logoColor=white"> <img src="https://img.shields.io/badge/GitBook-Microservices-cf8f63?style=flat&logo=GitBook&logoColor=white"> <img src="https://img.shields.io/badge/Confluence-Microservices-dcb284?style=flat&logo=Confluence&logoColor=white">

<a href=""><img src="https://em-content.zobj.net/source/microsoft-teams/363/package_1f4e6.png" align="right" height="77"></a>

Em engenharia de software, uma arquitetura de **microsserviços** (microservices) é uma abordagem arquitetônica e organizacional do desenvolvimento de software na qual o software consiste em pequenos ou um conjunto de **serviços** independentes e com escopo limitado a uma única função comercial que se comunicam usando APIs bem definidas. Esses serviços pertencem a pequenas equipes autossuficientes. Os microsserviços são uma coleção de unidades menores que sempre entregam e implementam aplicativos grandes e complexos.

> Um **serviço** (service) é uma parte da nossa aplicação back-end isolada, contendo as regras de negócio, APIs e controle de dados.

**Um microsserviço** é um serviço web responsável por parte da lógica de domínio. Vários microsserviços são combinados para criar um aplicativo, e cada um representa uma funcionalidade para o domínio. Os microsserviços interagem uns com os outros por meio de APIs, como REST ou gRPC ou GraphQL, mas não têm conhecimento da atividade interna de outros serviços. Essa interação harmoniosa entre microsserviços é a arquitetura de microsserviços. Ele faz com que o software seja composto de múltiplos serviços de ligação solta que são independentes uns dos outros e implantados separadamente.

Os microsserviços surgiram como uma alternativa mais popular a SOA devido aos seus benefícios. Os microsserviços são mais compostos, permitindo que as equipes reutilizem a funcionalidade oferecida pelos pequenos pontos centrais de serviço. Os microsserviços são mais robustos e permitem um escalonamento vertical e horizontal mais dinâmico. Portanto, eles são um padrão de arquitetura orientado a serviços em que os aplicativos são construídos como uma coleção de várias unidades de serviço independentes menores. 

É uma abordagem de engenharia de software que se concentra na decomposição de um aplicativo em módulos de função única com interfaces bem definidas. Esses módulos podem ser implantados e operados de forma independente por pequenas equipes que possuem todo o ciclo de vida do serviço. O termo “micro” refere-se ao dimensionamento de um microsserviço que deve ser gerenciado por uma única equipe de desenvolvimento (5 a 10 desenvolvedores). Nesta metodologia, grandes aplicações são divididas nas menores unidades independentes.

> Pensando de forma minimalista e conceitualmente limpa, um microserviço é essencialmente um endpoint (ou um conjunto de endpoints) especializado e desacoplado, responsável por um domínio de dados ou funcionalidade específica, e que pode ser orquestrado dentro de uma arquitetura maior. Estes pequenos independentes se comunicam entre si com as APIs bem definidas. Esta abordagem torna o software escalável, mais rápido de desenvolver e atualizar de forma rápida, eficiente e fácil.

A <a href="https://www.instagram.com/valdircezarr/">arquitetura de microsserviços</a> é um padrão evoluído que mudou fundamentalmente a maneira como o código do lado do servidor é desenvolvido e gerenciado. Esse padrão de arquitetura envolve o design e o desenvolvimento do aplicativo como uma coleção de serviços fracamente acoplados que interagem em APIs leves e bem definidas para atender aos requisitos de negócios. O objetivo é ajudar as empresas de desenvolvimento de software a acelerar o processo de desenvolvimento, facilitando a entrega e o desenvolvimento contínuos.

Se falarmos sobre seu nível elementar, um microsserviço específico atua como um aplicativo em si mesmo que forma um aplicativo maior com outros microsserviços; Isso permite:

## [Microservices] Service mesh
<img src="https://img.shields.io/badge/Istio-Service_mesh-blue?style=flat&logo=Istio&logoColor=white"> <img src="https://img.shields.io/badge/Consul-Service_mesh-magenta?style=flat&logo=Consul&logoColor=white"> <img src="https://img.shields.io/badge/Linkerd-Service_mesh-limegreen?style=flat&logo=Linkerd&logoColor=white"> <img src="https://img.shields.io/badge/Kuma-Service_mesh-black?style=flat&logo=Kuma&logoColor=white">

<img height="77" src="https://user-images.githubusercontent.com/61624336/203901779-b9b35de6-2eeb-4b1b-ae76-b1600bb79e3d.png" align="right">

Um **Service mesh** (malha de serviço) é uma camada de infraestrutura configurável e de baixa latência projetada para lidar com um alto volume de comunicação entre processos baseada na rede entre serviços de infraestrutura de aplicativos usando interfaces de programação de aplicativos (APIs). 

Em um service mesh, cada instância do serviço é pareada com uma instância de um servidor de proxy reverso, chamando service proxy, sidecar proxy ou sidecar. A instância do serviço e o proxy sidecar compartilham um container, e o container é gerenciado por uma ferramenta de orquestração de containers como Kubernetes, Nomad, Docker Swarm ou DC/OS. O proxy de serviço é responsável pela comunicação com outras instâncias de serviço e podem suportar capacidades como descoberta de (instância de) serviço, balanceamento de carga, autenticação e autorização, comunicação segura e outras.

Serviços de malha, como Istio, Linkerd e Consul, são implementados como uma camada de infraestrutura entre os microsserviços, facilitando a comunicação e oferecendo um conjunto de funcionalidades padronizadas para lidar com os desafios complexos inerentes a ambientes distribuídos e baseados em microsserviços.

A malha de serviço geralmente é implementada fornecendo uma instância de proxy, chamada sidecar , para cada instância de serviço. Os Sidecars lidam com comunicações, monitoramentos e preocupações relacionadas à segurança entre serviços  na verdade, qualquer coisa que possa ser abstraída dos serviços individuais. Dessa forma, os desenvolvedores podem lidar com desenvolvimento, suporte e manutenção do código do aplicativo nos serviços; as equipes de operações podem manter a malha de serviço e executar o aplicativo.

Uma malha de serviços garante que a comunicação entre serviços de infraestrutura de aplicativos em contêiner e muitas vezes efêmeros seja rápida, confiável e segura. A malha fornece recursos críticos, incluindo descoberta de serviços, balanceamento de carga, criptografia, observabilidade, rastreabilidade, autenticação e autorização e suporte para o padrão de circuit braker (disjuntor).

Aqui vou dar ênfase em um service mesh especifico o grande **Istio** mas existem outros, como o **Consul** da Hashicorp que vale a pena olhar.

Podemos pensar em um service mesh como um campo de força inteligente e programável que envolve cada microserviço em uma arquitetura distribuída. Vamos explorar essa metáfora em detalhes, porque ela capta perfeitamente a essência do conceito. Imagine que cada microserviço é uma espaçonave ou uma base em um campo de batalha. Sozinha, ela é vulnerável. O service mesh é o _campo de força_ (force field) que a envolve, mas não é um escudo estático e burro. É um sistema de defesa ativo, inteligente e com consciência situacional.

Basicamente, são uma arquitetura de rede utilizada em ambientes de microsserviços para gerenciar a comunicação entre esses serviços de forma mais segura, confiável e controlada.

A principal função dos serviços de malha é oferecer um conjunto de capacidades para facilitar e controlar a comunicação entre os microsserviços em uma aplicação distribuída. Alguns dos principais objetivos e funcionalidades incluem:

<img height="277" align="right" src="https://github.com/user-attachments/assets/c21fb986-44d4-4747-8ace-776c5cccde04" />

- Descoberta de Serviços: Ajudam os microsserviços a descobrirem e se comunicarem entre si, independentemente de onde estão hospedados na rede.

- Roteamento e Balanceamento de Carga: Direcionam o tráfego entre os serviços de maneira inteligente, distribuindo as requisições de forma equilibrada para garantir um desempenho otimizado e evitar sobrecargas em um único serviço.

- Segurança na Comunicação: Implementam medidas de segurança, como criptografia de ponta a ponta e autenticação, para garantir a confidencialidade e integridade dos dados durante a comunicação entre os serviços.

- Monitoramento e Observabilidade: Oferecem ferramentas para monitorar o tráfego entre os serviços, coletando métricas e informações que podem ser utilizadas para análise, solução de problemas e otimização da rede.

- Controle de Tráfego e Políticas de Acesso: Permitem definir políticas de acesso, regras de autorização, limites de tráfego e outras políticas para controlar o comportamento da rede.

## [Microservices] Service Discovery
Embora a tendência do setor seja dividir seu aplicativo monolítico em microsserviços para segregar dados, código e interface, não é uma tarefa fácil de fazer. Especialmente se você não tiver nenhuma experiência no desenvolvimento de microsserviços e não estiver familiarizado com as práticas recomendadas e os padrões e princípios essenciais de design de microsserviços.

Gostando de Padrões de Design Orientados a Objetos, os Padrões de Microsserviços também são soluções testadas e comprovadas para problemas comuns que as pessoas encontraram ao desenvolver, implantar e dimensionar seus Microsserviços.

Por exemplo, o padrão SAGA resolve o problema de falhas de transação distribuída e o gateway de API facilita o código do lado do cliente e também atua como um controlador frontal e balanceador de carga para muitos de seus microsserviços, tornando-os mais fáceis de manter.

Você está lutando para acompanhar seu número crescente de microsserviços? Não se preocupe mais! O padrão **Service Discovery** (descoberta de serviço) está aqui para ajudá-lo a navegar no mundo complexo dos microsserviços com facilidade. Esse padrão permite que os serviços se encontrem dinamicamente, garantindo uma comunicação suave e reduzindo a necessidade de configuração manual. Padrão de descoberta de serviço: navegando no labirinto de microsserviços com facilidade

Por que o Service Discovery é crucial para sua arquitetura de microsserviços? À medida que seu sistema é dimensionado, o gerenciamento dos locais de serviço em constante mudança torna-se cada vez mais desafiador. Com o Service Discovery, os serviços podem se registrar e descobrir uns aos outros automaticamente, promovendo agilidade e flexibilidade em seu sistema.

> Dê uma olhada nos <a href="https://www.designgurus.io/course/grokking-microservices-design-patterns">Padrões de Design de Microsserviços da Grokking</a> para dominar esses padrões de design de microsserviços para projetar sistemas escalonáveis, resilientes e mais gerenciáveis.

A descoberta de serviço pode ser obtida por meio de duas abordagens principais: descoberta do lado do cliente e descoberta do lado do servidor. A descoberta do lado do cliente envolve o cliente consultando um registro de serviço para encontrar o local do serviço de destino, enquanto a descoberta do lado do servidor depende de um balanceador de carga para rotear solicitações para o serviço apropriado. Ferramentas como Netflix Eureka, Consul e Kubernetes oferecem soluções integradas de descoberta de serviços para atender às suas necessidades específicas.

O diagrama abaixo é uma arquitetura de microsserviços baseada em **Service Registry com Load Balancer**, também conhecida como **Service Discovery com Client-Side e/ou Server-Side Load Balancing**. Vou detalhar:

<img width="720" height="443" alt="image" src="https://github.com/user-attachments/assets/9832675c-c6f3-4ca4-ab8c-2179769ccd38" />

1. **Service Instances (A, B, C)**: cada serviço é independente, com sua própria API REST. Esses são os microsserviços reais.
2. **Registry Client**: cada instância de serviço se registra no **Service Registry** para que outras partes do sistema saibam onde encontrá-la.
3. **Service Registry**: é o componente central que mantém o mapeamento de quais instâncias estão ativas e seus endereços (IP + porta). Pode ser algo como **Eureka, Consul ou Zookeeper**.
4. **Load Balancer**: faz o balanceamento de requisições entre as instâncias disponíveis do serviço. Dependendo da implementação, pode ser **Server-Side** (o load balancer sabe das instâncias) ou **Client-Side** (o cliente consulta o registry e decide qual instância chamar).
5. **Request Flow**: quando uma requisição chega, ela passa pelo load balancer, que consulta o Service Registry para descobrir quais instâncias estão ativas e encaminha a requisição de forma balanceada.

**Resumo do tipo de arquitetura:**

* **Arquitetura de microsserviços com Service Discovery e Load Balancing**
* **Características principais:**

  * Desacoplamento total entre clientes e serviços.
  * Descoberta dinâmica de serviços (não precisa de endereços fixos).
  * Balanceamento de carga automático.
  * Alta escalabilidade e resiliência.

<img width="720" height="1142" alt="image" src="https://github.com/user-attachments/assets/ca37099f-ecb1-4055-aed8-32b814f1db16" />

Em poucas palavras, o padrão de descoberta de serviço desempenha um papel fundamental na manutenção de uma arquitetura de microsserviços robusta e adaptável. Ao implementar esse padrão, você pode gerenciar e dimensionar facilmente seus serviços sem suar a camisa. Você está preparado para conquistar o labirinto de microsserviços com o Service Discovery?

## [Microservices] Inter-Service Communication
Comunicação entre serviços em aplicações monolíticas: Em uma arquitetura monolítica, todos os componentes e módulos do aplicativo são totalmente integrados em uma única base de código e são executados no mesmo processo ou na mesma máquina. Como todos os componentes fazem parte do mesmo aplicativo, normalmente não há necessidade de comunicação entre serviços ou chamadas remotas para funções internas de negócios. A comunicação entre os componentes é obtida por meio de chamadas de método no nível da linguagem ou chamadas de função simples na mesma base de código

```java
// Monolithic application with internal method calls
public class MonolithicApp {
    public void performBusinessLogic() {
        // Call a method within the same application
        ComponentA.doSomething();
        ComponentB.processData();
    }
}

class ComponentA {
    public static void doSomething() {
        // Business logic for Component A
    }
}

class ComponentB {
    public static void processData() {
        // Business logic for Component B
    }
}
```

Neste exemplo monolítico, a classe chama diretamente métodos dentro e . Como todos os componentes fazem parte do mesmo aplicativo, não há necessidade de comunicação de rede e as chamadas de método são diretas.MonolithicAppComponentAComponentB

<img width="720" height="364" alt="image" src="https://github.com/user-attachments/assets/41b090e2-732a-4ce0-ad08-b85b9d0b08e6" />

## [Microservices] EDA - Event-Driven Architecture
<a href="http://tryrabbitmq.com/"><img src="https://img.shields.io/badge/RabbitMQ-16.17.0-orange?style=flat&logo=RabbitMQ&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/RabbitMQ-16.17.0-orange?style=flat&logo=Medium&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/Apache_Kafka-16.17.0-black?style=flat&logo=Apache-Kafka&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/Apache_Kafka-16.17.0-black?style=flat&logo=Apache-Kafka&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/Apache_Kafka-16.17.0-black?style=flat&logo=Apache-Kafka&logoColor=white"></a>

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/99011c9e-9092-45d4-9487-e3bdb7346352" align="right" height="377">

A **EDA - Event-driven architecture** (arquitetura de orientação a eventos) é um paradigma de design de software em que os componentes de um sistema são projetados para responder a eventos e mensagens, em vez de se comunicarem diretamente uns com os outros através de chamadas de função ou métodos. 

A arquitetura orientada a eventos é um padrão de design poderoso que pode fornecer muitos benefícios para sistemas modernos. Ao permitir que os componentes se comuniquem de forma assíncrona por meio de eventos, a arquitetura orientada a eventos pode permitir sistemas mais flexíveis, escaláveis e resilientes que podem lidar com as demandas de dados em tempo real e ambientes distribuídos.

Nessa arquitetura, os eventos são usados como meio de comunicação entre os diferentes componentes ou módulos do sistema. Esses eventos podem ser gerados por ações de usuários, sensores, outros sistemas, ou até mesmo pelo próprio sistema. Se você está cansado de lidar com a complexidade e a inflexibilidade das arquiteturas tradicionais de solicitação-resposta, talvez seja hora de considerar a arquitetura orientada a eventos.

Os microsserviços orientados a eventos são um padrão de design para a criação de sistemas de software escalonáveis e resilientes. Em vez da arquitetura monolítica tradicional, em que todos os componentes são fortemente acoplados e executados em uma sequência predefinida, os microsserviços orientados a eventos desacoplam componentes individuais e permitem que eles se comuniquem e colaborem por meio da troca de eventos.

Em uma arquitetura de microsserviços orientada a eventos, cada microsserviço é projetado para ser pequeno, modular e independente, e se concentra em uma funcionalidade ou funcionalidade de negócios específica. Esses microsserviços se comunicam entre si por meio de um sistema de mensagens, como o Apache Kafka, que atua como um hub central para a troca de eventos. Isso permite que os microsserviços sejam acoplados de forma flexível e permite que sejam desenvolvidos, implantados e dimensionados independentemente uns dos outros.

Um dos benefícios do uso de microsserviços orientados a eventos é que ele permite a criação de sistemas altamente escaláveis e resilientes. Porque cada microsserviço é

A arquitetura orientada a eventos facilita o manuseio de processos demorados, funcionalidades complexas e longo tempo de espera para os usuários processarem as solicitações. De plataformas de mídia social a sistemas de processamento de pagamentos, a arquitetura orientada a eventos está alimentando alguns dos aplicativos mais bem-sucedidos do mercado.

Você pode estar familiarizado com a arquitetura tradicional de solicitação-resposta (um cliente, normalmente um navegador da Web, envia uma solicitação de um recurso para um servidor e o servidor envia de volta uma resposta correspondente ao recurso), na qual os componentes se comunicam entre si fazendo solicitações explícitas e recebendo respostas. Os componentes são fracamente acoplados nesta arquitetura.

Em um sistema orientado a eventos, os componentes se comunicam entre si produzindo e consumindo eventos. Isso permite sistemas mais flexíveis e escaláveis, pois os componentes não precisam esperar por solicitações ou respostas explícitas.

Um **evento** (event) pode ser definido como uma mudança significativa do seu estado. Nessa arquitetura, os sistemas são construídos em torno da ideia de eventos. Os componentes do sistema podem produzir, consumir ou reagir a eventos. Quando um evento ocorre, os componentes interessados são notificados para tomar ações apropriadas. Essa arquitetura é comumente usada em sistemas de streaming em tempo real, como aplicativos de monitoramento e processamento de dados em tempo real.

> Os termos Event-Based e Event-Driven frequentemente são usados de maneira intercambiável, mas tecnicamente podem ter nuances diferentes dependendo do contexto em que são aplicados. No entanto, para a maioria das aplicações práticas e discussões sobre arquitetura de microsserviços, eles se referem ao mesmo padrão arquitetural. 

Um exemplo de arquitetura orientada a eventos é o **sistema de processamento de pagamentos** usado por comerciantes online. Quando um cliente faz uma compra, um evento é gerado e enviado para o sistema de processamento de pagamentos. O sistema de processamento de pagamentos processa o pagamento e envia um evento de confirmação de volta ao sistema do comerciante, que atualiza o status do pedido.

Vamos tentar entendê-lo de uma maneira mais simples com um exemplo. Digamos que você tenha um sistema que permite enviar vídeos para a plataforma deles. O sistema precisa lidar com as seguintes tarefas:

- Aceitar upload de vídeo do cliente
- Inspecionando o vídeo em busca de violações.
- Transcodificando o vídeo. (convertendo vídeo para outros formatos como MPEG, HLS etc, que oferece a melhor experiência de transmissão com base no seu dispositivo e largura de banda de rede.)
- Gerando uma miniatura.
- Codificando áudio para o vídeo.
- Adicione marcas d'água, se houver.
- Adicione metadados desse vídeo ao banco de dados.
- Carregando o vídeo para a nuvem ou para cdn.
- e muitos mais.

Em uma arquitetura tradicional de solicitação-resposta, essas tarefas podem ser implementadas da seguinte maneira:

- O usuário carrega um vídeo na plataforma.
- A plataforma envia uma solicitação ao sistema de processamento de vídeo para processar o vídeo.
- O sistema de processamento de vídeo primeiro passa o vídeo para a lista de verificação de inspeção e isso validará se o vídeo está violando algum direito ou algo assim.
- Em seguida, o vídeo será passado pelo serviço de transcodificação no qual o vídeo será convertido para diferentes formatos e tamanhos.
- O vídeo será usado para criar a miniatura.
- Em seguida, precisamos passar o vídeo pelo serviço de codificação de áudio para codificar o áudio.
- Depois que a codificação de áudio for concluída, precisamos adicionar uma sobreposição de imagem em cima do vídeo.
- Em seguida, precisamos enviar o vídeo para a nuvem para melhor acessibilidade para o usuário. idealmente CDN.
- Feito tudo isso, precisamos atualizar o banco de dados para os metadados e o conteúdo relacionado à imagem.
- Em seguida, poderemos retornar a resposta ao usuário dizendo que o upload do vídeo é um sucesso ou algo assim.

<img width="720" height="574" alt="image" src="https://github.com/user-attachments/assets/6edbeb13-c2a4-44ff-82fe-4ef68e4d1637" />

Nesse cenário, o site está fortemente acoplado ao sistema de processamento de vídeo e o sistema de processamento de vídeo está fortemente acoplado aos outros serviços responsáveis por lidar com operações como codificação, compactação, marca d'água etc. Se algum desses componentes falhar, todo o sistema poderá ser afetado. Além disso, se o sistema tiver um alto volume de uploads de vídeo, o sistema de processamento de vídeo poderá se tornar um gargalo.

> Esse tipo de arquitetura é comumente usado em muitos sistemas, mas pode ser menos flexível e escalável do que outras arquiteturas, como a arquitetura orientada a eventos.

Em uma arquitetura orientada a eventos, os componentes se comunicam entre si de forma assíncrona por meio de eventos, em vez de solicitações e respostas explícitas.

Agora, vamos considerar como esse cenário pode ser implementado usando a arquitetura orientada a eventos:

- O usuário carrega um vídeo na plataforma.
- A plataforma gera um evento de "upload de vídeo" e o envia para o sistema orientado a eventos.
- O sistema orientado a eventos encaminha o evento para o componente de inspeção de vídeo, que verificará se o vídeo não está violando nenhum direito. Assim que a inspeção de vídeo for concluída, ela gerará um evento de "processamento de vídeo".
- O sistema orientado a eventos roteia o "processamento de vídeo" para os componentes de transcodificação, miniatura, codificação de áudio, compactação e marca d'água.
- Como esses componentes são fracamente acoplados, eles podem funcionar de maneira assíncrona.
- Cada um desses componentes é dissociado um do outro, pois se comunicam por meio de eventos em vez de solicitações ou respostas diretas.
- O usuário pode enviar o vídeo e continuar com seus outros trabalhos, pois não precisa esperar que o servidor processe todas essas coisas. Esses processos estão sendo tratados de forma assíncrona.
- Assim que todos os componentes forem concluídos com suas respectivas manipulações para o vídeo, podemos notificar o usuário.

<img width="720" height="461" alt="image" src="https://github.com/user-attachments/assets/cf31f878-396c-49a8-9a67-72e7a2c7c719" />

Apresentando o agente de mensagens, eventos de pull de componentes do agente de mensagens, os componentes são desacoplados.

Nessa arquitetura orientada a eventos, o site é desacoplado do componente de processamento de vídeo e o componente de processamento de vídeo é desacoplado dos outros componentes. Isso permite mais flexibilidade e facilita a modificação ou substituição de componentes individuais sem afetar o sistema geral.

Introduzimos um agente de mensagens, o vídeo que precisa ser processado é enviado para o agente de mensagens, outros componentes funcionam como um consumidor que consome eventos desse agente de mensagens.

À medida que os componentes se comunicam de forma assíncrona por meio de eventos, o sistema pode escalar horizontalmente adicionando mais instâncias de um componente para lidar com um volume maior de pedidos.

Benefícios da arquitetura orientada a eventos:

- Acoplamento flexível: os componentes em um sistema orientado a eventos são desacoplados uns dos outros, pois se comunicam por meio de eventos em vez de solicitações ou respostas diretas. Isso facilita a modificação ou substituição de componentes individuais sem afetar o sistema geral.

- Escalabilidade: como os componentes em um sistema orientado a eventos não precisam esperar por solicitações ou respostas explícitas, o sistema pode escalar horizontalmente adicionando mais instâncias de um componente para lidar com um volume maior de eventos.

- Resiliência: em um sistema orientado a eventos, se um componente falhar, os eventos podem ser armazenados em buffer e repetidos assim que o componente for restaurado, permitindo que o sistema se recupere de falhas com mais facilidade.

Aqui estão alguns exemplos de arquitetura orientada a eventos no mundo real:

- Processamento de pagamentos: Quando um cliente faz uma compra em um comerciante online, um evento é gerado e enviado para o sistema de processamento de pagamentos. O sistema de processamento de pagamentos processa o pagamento e envia um evento de confirmação de volta ao sistema do comerciante, que atualiza o status do pedido.

- Plataforma de mídia social: os eventos são gerados sempre que um usuário publica uma mensagem, curte uma postagem ou executa qualquer outra ação em uma plataforma de mídia social. Esses eventos são usados para atualizar os feeds e notificações de outros usuários em tempo real.

- Gerenciamento de estoque: em um ambiente de depósito ou varejo, os eventos podem ser gerados sempre que um item é adicionado ou removido do estoque. Esses eventos podem disparar atualizações no sistema de gerenciamento de estoque e acionar o reabastecimento ou reabastecimento conforme necessário.

Aqui estão algumas coisas importantes a serem lembradas ao projetar uma arquitetura orientada a eventos:

- Identifique as fontes de eventos: A primeira etapa na criação de uma arquitetura orientada a eventos é identificar as fontes de eventos em seu sistema. Podem ser fontes externas, como ações do usuário ou leituras de sensores, ou fontes internas, como a conclusão de uma tarefa em segundo plano.

- Defina os eventos: Em seguida, você deve definir os eventos que serão usados para se comunicar entre os componentes do seu sistema. Isso inclui a estrutura e o conteúdo dos eventos, bem como o formato em que eles serão transmitidos (e.g. JSON mensagens por HTTP).

- Escolha um mecanismo de entrega de eventos: há várias opções para entregar eventos em um sistema controlado por eventos, incluindo filas de mensagens, sistemas de publicação/assinatura e barramentos de eventos. Você deve escolher o mecanismo de entrega que melhor se adapta às necessidades do seu sistema, considerando fatores como confiabilidade, escalabilidade e desempenho.

- Projete os consumidores de eventos: os consumidores de eventos são os componentes do sistema que reagem a eventos. Você deve projetar esses componentes para serem o mais desacoplados possível das origens dos eventos e para lidar com eventos de forma assíncrona.

- Implementar novas tentativas e tratamento de erros: Em um sistema orientado a eventos, é importante implementar novas tentativas e tratamento de erros para garantir que os eventos sejam entregues de forma confiável e que o sistema possa se recuperar de falhas. Isso pode incluir eventos de buffer e repetição da entrega em caso de falha ou implementação de transações de compensação para desfazer os efeitos de eventos com falha.

- Teste e monitore a arquitetura orientada a eventos: Como em qualquer sistema, é importante testar e monitorar minuciosamente uma arquitetura orientada a eventos para garantir que ela esteja funcionando conforme o esperado e para identificar e resolver quaisquer problemas que surjam.

A arquitetura orientada a eventos pode oferecer muitos benefícios, mas tem suas desvantagens. Aqui estão algumas desvantagens potenciais a serem consideradas:

- Complexidade: Os sistemas orientados a eventos podem ser mais complexos do que as arquiteturas tradicionais de solicitação-resposta, pois envolvem comunicação assíncrona e podem envolver vários componentes trabalhando juntos para produzir e consumir eventos. Isso pode tornar mais desafiador projetar, implementar e depurar sistemas orientados a eventos.

- Dependência de serviços de terceiros: os sistemas orientados a eventos podem depender de serviços de terceiros, como filas de mensagens ou barramentos de eventos, para transmitir eventos entre componentes. Isso pode introduzir dependências adicionais e possíveis pontos de falha.

- Dificuldade em testar e depurar: como os sistemas orientados a eventos envolvem comunicação assíncrona e podem envolver vários componentes trabalhando juntos, eles podem ser mais difíceis de testar e depurar do que os sistemas tradicionais de solicitação-resposta.

- Ordenação de eventos: em alguns casos, pode ser importante manter a ordem na qual os eventos são gerados e consumidos. Isso pode ser mais desafiador em um sistema controlado por eventos, pois os eventos podem ser transmitidos e consumidos de forma assíncrona.

- Falta de garantias transacionais: Em um sistema orientado a eventos, pode não haver o mesmo nível de garantias transacionais que em um sistema tradicional de solicitação-resposta. Isso pode tornar mais difícil garantir a consistência e a integridade dos dados no sistema.

Dito isto, os benefícios da arquitetura orientada a eventos muitas vezes podem superar essas desvantagens, especialmente em sistemas que exigem alta escalabilidade, resiliência ou flexibilidade.

Exemplo 2: Quando um consumidor adquire um imóvel, o estado dele se modifica de "à venda" para "vendido".

A arquitetura desse sistema pode tratar essa mudança de estado como um evento cuja ocorrência pode ser divulgada para outros aplicativos dentro da sua arquitetura.

De uma perspectiva formal, o que é produzido, publicado, propagado, detectado ou consumido é uma mensagem (geralmente assíncrona), chamada de **notificação de evento**, e não o próprio evento, que é a mudança de estado que acionou a emissão da mensagem. Isso se deve às arquiteturas orientadas a eventos, muitas vezes sendo projetadas sobre **arquiteturas orientadas a mensagens**, nas quais tal padrão de comunicação requer que uma das entradas seja somente texto (a mensagem), para diferenciar como cada comunicação deve ser tratada.

Um **sistema de mensagens** é um dos mecanismos mais comumente usados para troca de informações entre aplicações.

Ao escolher seu mecanismo de integração de aplicações, é importante ter em mente os princípios orientadores discutidos anteriormente.

No caso de bancos de dados compartilhados, por exemplo, alterações feitas por um aplicativo podem afetar diretamente outros aplicativos que estão usando as mesmas tabelas de banco de dados. Ambas as aplicações são fortemente acopladas.

- Você pode querer evitar isso nos casos em que tenha regras adicionais a serem aplicadas antes de aceitar as alterações no outro aplicativo.

- Da mesma forma, você deve pensar sobre todos esses princípios orientadores antes de finalizar formas de integração entre suas aplicações.

Um sistema de mensagens atua como um componente de integração entre vários aplicativos. Um sistema orientado a eventos normalmente consiste em:

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/ec869c7b-2639-4f30-b5d7-c349961d117a" height="377" align="right">

- **Emissores** (ou agentes): Os emissores têm a responsabilidade de detectar, reunir e transferir eventos. Um emissor de evento não conhece os consumidores, nem mesmo sabe se existe ou não um consumidor e, caso exista, não sabe como o evento será utilizado ou processado.

- **Consumidores** (ou coletores): Os coletores têm a responsabilidade de aplicar uma reação assim que um evento seja apresentado. A reação pode ou não ser totalmente fornecida pelo próprio coletor. Por exemplo, o coletor pode ter apenas a responsabilidade de filtrar, transformar e encaminhar o evento para outro componente ou pode fornecer uma reação independente a tal evento.

- **Canais de eventos**: Os canais de eventos são transmitidos dos emissores para consumidores. A implementação física dos canais pode ser baseada em componentes tradicionais, como middleware orientado à mensagem ou comunicação ponto a ponto.

Em um projeto de um sistema de integração entre aplicações, alguns fatores/princípios devem ser colocados em mente, tais como: fracamente acoplado, definições de interfaces comuns, latência e confiabilidade. Vamos compreender cada um deles a seguir:

- **FRACAMENTE ACOPLADO**: A interação entre as aplicações deve garantir uma dependência mínima entre elas. Isso garante que qualquer modificação em uma aplicação não irá afetar a outra. É diferente dos sistemas fortemente acoplados, nos quais uma aplicação é codificada com especificações predefinidas da outra aplicação, e qualquer mudança pode quebrar ou mudar suas funcionalidades com outras aplicações dependentes.

> Um sistema de mensagens atua como um componente de integração entre vários aplicativos. Tal integração invoca diferentes comportamentos das aplicações com base nas trocas de informações entre eles. Esse comportamento pode ser aplicado pelo projeto e pela implementação de aplicativos e sistemas que transmitem eventos entre componentes de software e serviços fracamente acoplados.

- **PADRÕES DE INTERFACES COMUNS**: Deve garantir um formato de dados comum acordado para troca de mensagens entre aplicativos. Isso não apenas ajuda a estabelecer padrões de troca de mensagens entre aplicativos, mas também garante que algumas das melhores práticas de troca de informações possam ser aplicadas facilmente. Por exemplo, você pode escolher usar o formato de dados **Avro** (muito usado em Big Data) para trocar mensagens. Isso pode ser definido como seu padrão de interface comum para troca de informações.

- **LATÊNCIA**: É o tempo que as mensagens levam para passar entre o remetente e o receptor. A maioria dos aplicativos deseja atingir uma baixa latência como um requisito crítico. Mesmo em um modo de comunicação assíncrono, a alta latência não é desejável, pois um atraso significativo no recebimento de mensagens pode causar perdas significativas para qualquer organização.

- **CONFIABILIDADE**: Garante que a indisponibilidade temporária dos aplicativos não afete as aplicações dependentes que precisam trocar informações. Em geral, quando o aplicativo de origem envia uma mensagem para o aplicativo remoto, este pode estar lento ou não disponível devido a alguma falha. A comunicação de mensagens assíncronas e confiáveis garante que a fonte da aplicação continue o seu trabalho, e garante que o aplicativo remoto retomará sua tarefa mais tarde. Uma vez compreendidas essas premissas iniciais, exploraremos alguns conceitos básicos de controle de mensageria.

- **FILA DE MENSAGENS**: Estruturas que também são referenciadas como canais. De uma forma bem simples, podemos definir como conectores que enviam/recebem mensagens entre as aplicações de forma oportuna e confiável.

> Em ciência da computação, uma fila de mensagens (MQ - Messaging Queue) é um componente de engenharia de software usado para a comunicação entre processos ou threads dum mesmo processo. O componente usa uma fila de mensagens.
>
> Filas de mensagens provêm um protocolo de comunicação assíncrona, de forma que o remetente e o destinatário da mensagem não precisam interagir ao mesmo tempo. As mensagens são enfileiradas e armazenadas até que o destinatário as processe. A maioria das filas de mensagens definem limites ao tamanho dos dados que podem ser transmitidos numa única mensagem. Aquelas que não possuem tal limite são chamadas caixas de mensagens.
>
> Faz sentido usar as filas de mensagens quando os interlocutores estão ligados através de redes de grande escala, em países diferentes, para as quais a probabilidade de desconexão não é desprezível.

  - **MENSAGENS (PACOTES DE DADOS)**: Uma mensagem é um pacote de dados que é transmitido por uma rede para uma fila de mensagens. 
    1. O aplicativo remetente divide os dados em pacotes de dados menores e os envolve como uma mensagem com informações de protocolo e cabeçalho.
    2. Em seguida, ele o envia para a fila de mensagens.
    3. De maneira semelhante, um aplicativo receptor recebe uma mensagem e extrai os dados do invólucro para processá-los posteriormente.

- **REMETENTE (PRODUTOR)**: Os aplicativos do remetente ou produtor são as fontes de dados que precisam ser enviados a um determinado destino. Eles estabelecem conexões com pontos de extremidade da fila de mensagens e enviam dados em pacotes de mensagens menores, que seguem padrões de interface comuns. Dependendo do tipo de sistema em uso, os aplicativos remetentes podem decidir enviar dados um a um ou em lote.

- **DESTINATÁRIO (CONSUMIDOR)**: São os destinatários das mensagens enviadas pelo aplicativo remetente.
  1. Eles extraem ou recebem, por meio de uma conexão persistente, dados de filas de mensagens.
  2. Em seguida, extraem dados desses pacotes de mensagens e os usam para processamento posterior.

- **PROTOCOLOS DE TRANSMISSÃO DE DADOS**: Determinam as regras para controle das trocas de mensagens entre aplicativos. Diferentes sistemas de filas usam diferentes protocolos de transmissão de dados. Alguns exemplos de tais protocolos de transmissão de dados são:

  - **AMQP** (Advance Message Queuing Protocol) é um protocolo de rede de código aberto projetado para a troca eficiente e confiável de mensagens entre aplicativos ou sistemas distribuídos. Ele é especialmente útil em cenários em que é necessária uma comunicação assíncrona e a transferência de mensagens entre componentes de software.
  
  - **STOMP** (Streaming Text Oriented Message Protocol) é um protocolo de mensagens voltado para a comunicação entre clientes e servidores de mensagens (message brokers). Ele é projetado para ser simples e orientado a texto, facilitando a implementação e a interoperabilidade entre diferentes sistemas.
  
  - **MQTT** (Message Queue Telemetry Protocol) é um protocolo de mensagens leve e eficiente projetado para comunicação entre dispositivos em redes de Internet das Coisas (IoT) e em ambientes de redes de sensores. Ele foi desenvolvido para ser simples, econômico em termos de largura de banda e adequado para dispositivos com recursos limitados, como sensores, microcontroladores e outros dispositivos IoT.
  
  - **HTTP** (Hypertext Transfer Protocol) 

- **MODO DE TRANSFERÊNCIA**: O modo de transferência em um sistema de mensagens pode ser entendido como a maneira pela qual os dados são transferidos de uma aplicação de origem para a aplicação receptora. Exemplo: Modos síncrono, assíncrono e em lote.

![527342228_1267838731798263_2909866205762398317_n](https://github.com/user-attachments/assets/5a759381-2886-47a2-868f-8393f007b337)

## [Microservices] Sidecar
<img height="577" align="right" src="https://github.com/user-attachments/assets/79738b6d-a379-45c2-9d46-32dc5afb4a64" />

Os padrões de design são soluções reutilizáveis para problemas comuns no design de software. Eles fornecem uma abordagem estruturada para resolver desafios arquitetônicos sem reinventar a roda a cada vez.

O padrão **sidecar** é um desses padrões de design que ganhou destaque na engenharia de software moderna. Em sua essência, o padrão sidecar combina um processo ou serviço secundário (o "sidecar") com um aplicativo primário para lidar com tarefas complementares. Essas tarefas incluem registro em log, monitoramento, proxy, segurança ou gerenciamento de configuração. O sidecar é executado junto com o aplicativo principal, compartilhando o mesmo host ou contêiner, mas permanece lógica e operacionalmente independente.

O padrão sidecar pode ser comparado a uma motocicleta com um sidecar. A motocicleta (o serviço principal) é o principal motorista, responsável pela funcionalidade principal, como transportar uma pessoa. O sidecar (o serviço auxiliar) transporta ferramentas ou passageiros adicionais, auxiliando o veículo principal sem interferir em sua operação.

Da mesma forma, em sistemas de software, o sidecar estende os recursos do aplicativo principal sem ser fortemente acoplado a ele.

Serviços de monitoramento, registro, configuração e rede são frequentemente exigidos por aplicações e serviços. Essas tarefas extras podem ser realizadas como componentes ou serviços distintos.

Um serviço de sidecar nem sempre faz parte da aplicação, mas está vinculado a ele. Ele segue o aplicativo principal para onde quer que vá. Sidecars são procedimentos ou serviços que são oferecidos junto com a aplicação principal. O sidecar de uma motocicleta é acoplado a uma motocicleta, e cada motocicleta pode ter seu próprio sidecar. Um serviço de sidecar, da mesma forma, reflete o destino de sua aplicação principal. Uma instância sidecar é implantada e hospedada junto com cada instância da aplicação.

<img width="705" height="335" alt="image" src="https://github.com/user-attachments/assets/e8e09de0-8b91-4f24-9bce-1c9334cedf31" />

Eles podem ser executados no mesmo processo que a aplicação se estiverem fortemente integrados, fazendo uso ótimo dos recursos compartilhados. Isso, no entanto, implica que eles não estão devidamente separados, e uma falha em um desses componentes pode afetar outros componentes ou toda a aplicação. Além disso, normalmente devem ser escritos no mesmo idioma do programa principal. Como resultado, o componente e a aplicação dependem muito um do outro.

## [Microservices] BFF - Backend for Frontend
<a href="https://blog.bitsrc.io/bff-pattern-backend-for-frontend-an-introduction-e4fa965128bf?source=post_page---author_recirc--df10edf0e8d0----1---------------------1744195f_55d3_428f_b6fa_370d3ddc78c4--------------"><img src="https://github.com/user-attachments/assets/8afda213-16a2-41b6-8379-8ddead4ac676" align="right" height="277"></a>

Conforme aumenta a complexidade dos produtos que desenvolvemos, mais provável é que aumente também a quantidade de “caras” que ele vai ter. Hoje é muito comum, por exemplo, um mesmo produto ter uma interface web, outra móvel e outra responsiva. Neste contexto, entendo que seja bastante tentador projetar uma única API de back-end para todas as interfaces, que seja reutilizável.

Entretanto, é claro que, como sempre, em um produto complexo uma solução simples não cai bem. As necessidades e restrições são bastante variáveis, e às vezes é necessária uma personalização. Para resolver este problema, é que entra em cena o _BFF_, que até pode ser considerado um _best friends forever_, mas significa na verdade _Back-end for Front-end_.

A Arquitetura **BFF - Backend for Frontend** é um padrão onde você cria um back-end específico para cada tipo de front-end (como web, mobile ou desktop). Em vez de ter um único back-end genérico que serve para todos, cada front-end tem seu próprio "mini-backend" adaptado às suas necessidades, reduzindo a complexidade no cliente e otimizando a performance.

Por exemplo, uma API BFF para um app mobile pode retornar dados já filtrados e otimizados para economia de banda, enquanto o BFF da versão web pode fornecer dados mais completos. Essa abordagem melhora a experiência do usuário, facilita manutenção e testes, e evita lógica excessiva no front-end.

A arquitetura BFF se encaixa muito bem com microserviços. Na verdade, ela é frequentemente usada em conjunto com microserviços para resolver um problema comum: a complexidade de consumir diretamente múltiplos serviços no front-end.

> [!Warning]
> Aviso: Os detalhes deste post foram extraídos do Blog de Engenharia do SoundCloud. Todo o crédito pelos detalhes técnicos pertence à equipe de engenharia do SoundCloud. Os links para os artigos originais estão presentes na seção de referências no final do post. Tentamos analisar os detalhes e fornecer nossa opinião sobre eles. Se você encontrar alguma imprecisão ou omissão, deixe um comentário e faremos o possível para corrigi-las.

Assim como na vida real, os melhores amigos também podem ser salvadores quando se trata de projetos de software.

O SoundCloud descobriu isso quando quis evoluir sua arquitetura de serviço para lidar com milhões de solicitações por hora.

Caso você não saiba, o SoundCloud é um site online para ouvir música gratuitamente. Eles têm mais de 320 milhões de faixas musicais e a maior comunidade online do mundo de artistas, bandas, DJs e criadores de áudio.

Inicialmente, o aplicativo web do SoundCloud seguia o que eles chamavam de abordagem "comer a própria ração". Uma única API monolítica atendia aos requisitos de aplicativos oficiais e integrações de terceiros.

Naturalmente, com o crescimento do SoundCloud, essa abordagem tornou-se insuficiente para suas necessidades de escalabilidade operacional e organizacional, resultando em uma migração da arquitetura monolítica para microsserviços.

No entanto, isso se mostrou mais fácil na teoria do que na prática. Com a criação de novos microsserviços, os clientes que dependiam do monolito passaram a ter que acessar múltiplos serviços para obter os dados necessários. Isso dificultou o desenvolvimento para os clientes, incluindo aplicativos de terceiros que utilizavam o SoundCloud.

Como essa situação era insustentável, o SoundCloud precisou criar uma maneira de facilitar o desenvolvimento para os aplicativos clientes, mantendo a arquitetura de microsserviços subjacente. Neste artigo, veremos como eles alcançaram esses objetivos com BFFs (Browser Forwarders), Serviços de Valor Agregado e Gateways de Domínio.

**BFFs no SoundCloud**: O termo BFF significa Backends-for-Frontends (Backends para Frontends). Em termos mais simples, pense em um BFF como um gateway de API dedicado para cada dispositivo ou tipo de interface que interage com seu aplicativo.

O diagrama abaixo mostra uma visão geral do BFF:

<img width="1600" height="971" alt="image" src="https://github.com/user-attachments/assets/96f99b89-ca2b-497d-9237-8086ba4ae353" />

<img src="https://github.com/user-attachments/assets/348dad2b-072f-4207-ac8e-0f823d637261" align="right" height="477">

Em um sistema de microserviços, cada serviço é especializado em uma funcionalidade (como autenticação, pagamentos, produtos etc.), mas o front-end precisaria orquestrar várias chamadas, lidar com autenticação, formatação, e mais. O BFF entra nesse ponto como uma camada de orquestração entre os microserviços e o front-end.

Ele agrega, adapta e transforma os dados de vários serviços para entregar ao front-end exatamente o que ele precisa, sem que o front precise entender toda a estrutura dos serviços internos. Isso melhora a performance, simplifica o front-end e ajuda a manter separação de responsabilidades.

Discutimos o API Gateway. Essa abordagem é boa se tivermos um único cliente na web ou no celular. Se nosso aplicativo for usado por vários clientes, como web, dispositivos móveis, IoT, etc., não é uma boa ideia usar um único API Gateway para todos os tipos de clientes. O processo ficará complicado rapidamente e poderá inchar o serviço API Gateway, tornando-o um único serviço Monolith.

A melhor abordagem para esse tipo de cenário é usar um API Gateway separado para cada tipo de cliente, esse padrão de arquitetura é chamado de padrão Backend for FrontEnd (BFF) e se tornou uma palavra da moda.

A equipe de engenharia do SoundCloud opera dezenas de BFFs (Broadcast Frameworks), cada um atendendo a um tipo específico de cliente. Por exemplo, um BFF chamado API Móvel atende clientes Android e iOS. Há também um BFF de API Web que lida com a interface web e os widgets. Além disso, existem BFFs dedicados para APIs públicas e de parceiros.

Todo o tráfego externo que chega ao SoundCloud passa por um dos BFFs. Esses BFFs também lidam com diversas funcionalidades, como:

<img src="https://github.com/user-attachments/assets/dea5743c-855c-43e0-9fb9-210fa03addd1" align="right" height="277">

- Limitação de taxa
- Autenticação
- Sanitização de cabeçalho
- Controle de cache

O padrão BFF é um paradigma arquitetônico, uma variante do padrão de API Gateway e compreende vários back-ends projetados para atender às demandas de aplicativos front-end específicos, como desktop, navegador e aplicativos móveis nativos, dispositivos IoT etc.

<img width="1600" height="1025" alt="image" src="https://github.com/user-attachments/assets/d8c4bbe6-81bf-4b02-bea0-3eb2ba6fb35a" />

Para facilitar o compartilhamento de lógica comum entre todos os BFFs (Broadcast Frameworks for Frontiers), todos eles utilizam uma biblioteca interna que fornece recursos avançados. Quaisquer alterações nessa biblioteca são implementadas automaticamente em questão de horas.

O SoundCloud segue a filosofia de desenvolvimento de código-fonte interno para esses BFFs.

De acordo com essa filosofia, equipes individuais podem contribuir para a base de código do BFF, e uma equipe central revisa cada alteração com base nos princípios discutidos no Coletivo. Esse Coletivo, organizado por um Líder de Plataforma, se reúne regularmente para discutir problemas e compartilhar conhecimento.

**Vantagens do BFF**: Os BFFs oferecem diversas vantagens. Vejamos algumas das principais.

1 - Autonomia: A autonomia é talvez o maior valor agregado ao usar um BFF.

APIs separadas por tipo de cliente significam que podemos otimizar a API para o que for mais conveniente para um determinado tipo de cliente.

Por exemplo, no caso do SoundCloud, os clientes móveis preferiam respostas maiores com um número maior de entidades incorporadas como forma de minimizar o número de solicitações. Em contraste, o front-end web prefere respostas mais granulares.

Os BFFs atendem a essas demandas variáveis ​​para cada tipo de cliente.

2 - Resiliência e Menor Risco: Os BFFs também reduzem o risco geral de indisponibilidade do aplicativo.

Embora uma implantação malsucedida possa derrubar um BFF inteiro em uma zona de disponibilidade, isso não derruba toda a plataforma, o que era uma possibilidade com a abordagem de API monolítica.

Veja o diagrama abaixo que representa um cenário em que a indisponibilidade do BFF móvel não significa que o BFF web também ficará indisponível.

<img width="1600" height="971" alt="image" src="https://github.com/user-attachments/assets/3c221b20-bb25-432f-a908-4282744dfa00" />
