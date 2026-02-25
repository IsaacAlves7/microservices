> Versículo chave: "Consagre ao Senhor tudo o que você faz, e os seus planos serão bem-sucedidos." - Provérbios 16:3

- https://substack.com/redirect/8e94e755-da70-4871-a52c-c1f3bc65ab95?j=eyJ1IjoiMmRpcmZwIn0.DgQpD9vnxeDXnbOGqr5r4QICWGtxf2wFAnKNG8yY6Aw
- https://substack.com/redirect/55568165-cc89-4e78-a706-d535205faa44?j=eyJ1IjoiMmRpcmZwIn0.DgQpD9vnxeDXnbOGqr5r4QICWGtxf2wFAnKNG8yY6Aw

# 📦 Microservices 
<a href="https://github.com/IsaacAlves7/qa"><img src="https://img.shields.io/badge/QA-Microservices-5B4638?style=flat&logo=GitHub&logoColor=white"></a> <a href="https://python.plainenglish.io/top-11-tools-for-microservices-backend-development-in-2023-3d9cdd61ef10"><img src="https://img.shields.io/badge/Medium-Microservices-5B4638?style=flat&logo=Medium&logoColor=white"></a> <img src="https://img.shields.io/badge/DEV-Microservices-976857?style=flat&logo=dev.to&logoColor=white"> <img src="https://img.shields.io/badge/GitBook-Microservices-cf8f63?style=flat&logo=GitBook&logoColor=white"> <img src="https://img.shields.io/badge/Confluence-Microservices-dcb284?style=flat&logo=Confluence&logoColor=white">

<a href="https://github.com/IsaacAlves7/microservices"><img src="https://em-content.zobj.net/source/microsoft-teams/363/package_1f4e6.png" align="right" height="77"></a>

Em engenharia de software, uma arquitetura de **microsserviços** (microservices) é uma abordagem arquitetônica e organizacional do desenvolvimento de software na qual o software consiste em pequenos ou um conjunto de **serviços** independentes e com escopo limitado a uma única função comercial que se comunicam usando APIs bem definidas. Esses serviços pertencem a pequenas equipes autossuficientes. Os microsserviços são uma coleção de unidades menores que sempre entregam e implementam aplicativos grandes e complexos.

> Um **serviço** (service) é uma parte da nossa aplicação back-end isolada, contendo as regras de negócio, APIs e controle de dados.

Os microserviços representam uma mudança de paradigma na arquitetura de software, dividindo as aplicações em pequenos serviços implantáveis de forma independente. Essa abordagem oferece flexibilidade incomparável na escalabilidade e manutenção dos componentes do sistema, permitindo que as organizações desenvolvam e evoluam diferentes partes de suas aplicações de forma independente.

Com base em nossa discussão anterior sobre arquiteturas de 3 níveis, que podem ser implementadas usando abordagens monolíticas ou microserviços, este artigo explora os conceitos e insights essenciais dos microsserviços. Nosso objetivo é fornecer uma compreensão abrangente desse paradigma contemporâneo de design de sistemas, equipando você com conhecimentos cruciais para a arquitetura moderna de software e preparando para se destacar nas próximas entrevistas.

**Um microsserviço** é um serviço web responsável por parte da lógica de domínio. Vários microsserviços são combinados para criar um aplicativo, e cada um representa uma funcionalidade para o domínio. Os microsserviços interagem uns com os outros por meio de APIs, como REST ou gRPC ou GraphQL, mas não têm conhecimento da atividade interna de outros serviços. Essa interação harmoniosa entre microsserviços é a arquitetura de microsserviços. Ele faz com que o software seja composto de múltiplos serviços de ligação solta que são independentes uns dos outros e implantados separadamente.

Os microsserviços surgiram como uma alternativa mais popular a SOA devido aos seus benefícios. Os microsserviços são mais compostos, permitindo que as equipes reutilizem a funcionalidade oferecida pelos pequenos pontos centrais de serviço. Os microsserviços são mais robustos e permitem um escalonamento vertical e horizontal mais dinâmico. Portanto, eles são um padrão de arquitetura orientado a serviços em que os aplicativos são construídos como uma coleção de várias unidades de serviço independentes menores. 

É uma abordagem de engenharia de software que se concentra na decomposição de um aplicativo em módulos de função única com interfaces bem definidas. Esses módulos podem ser implantados e operados de forma independente por pequenas equipes que possuem todo o ciclo de vida do serviço. O termo “micro” refere-se ao dimensionamento de um microsserviço que deve ser gerenciado por uma única equipe de desenvolvimento (5 a 10 desenvolvedores). Nesta metodologia, grandes aplicações são divididas nas menores unidades independentes.

> Pensando de forma minimalista e conceitualmente limpa, um microserviço é essencialmente um endpoint (ou um conjunto de endpoints) especializado e desacoplado, responsável por um domínio de dados ou funcionalidade específica, e que pode ser orquestrado dentro de uma arquitetura maior. Estes pequenos independentes se comunicam entre si com as APIs bem definidas. Esta abordagem torna o software escalável, mais rápido de desenvolver e atualizar de forma rápida, eficiente e fácil.

A <a href="https://www.instagram.com/valdircezarr/">arquitetura de microsserviços</a> é um padrão evoluído que mudou fundamentalmente a maneira como o código do lado do servidor é desenvolvido e gerenciado. Esse padrão de arquitetura envolve o design e o desenvolvimento do aplicativo como uma coleção de serviços fracamente acoplados que interagem em APIs leves e bem definidas para atender aos requisitos de negócios. O objetivo é ajudar as empresas de desenvolvimento de software a acelerar o processo de desenvolvimento, facilitando a entrega e o desenvolvimento contínuos.

Se falarmos sobre seu nível elementar, um microsserviço específico atua como um aplicativo em si mesmo que forma um aplicativo maior com outros microsserviços; Isso permite:

<img src="https://github.com/user-attachments/assets/a7c5794e-03b6-4b1a-86c1-a5091c1bee8a" align="right" height="177">

- Desenvolvimento mais fácil e rápido
- Manutenibilidade
- Escalabilidade

Essencialmente, isso permite que você gerencie e mantenha um aplicativo com mais eficiência. Há, no entanto, uma complexidade específica inerente a esse padrão, que pode ser mitigada com o uso de certas práticas recomendadas.

Todos sabemos que o design de microsserviços tem um impacto direto na resiliência da rede das arquiteturas modernas. Quando as empresas decidem criar usando microsserviços, é importante desenvolvê-los de forma eficiente e eficaz para que possam operar na rede, sem causar excesso de latência, consumo de largura de banda e perda de pacotes.

Então, discutiremos as práticas recomendadas básicas de microsserviços que você deve considerar se quiser obter um ecossistema de microsserviços eficiente e desprovido de complexidades arquitetônicas extremas. 

**Adotar o princípio da responsabilidade única**: O Princípio da Responsabilidade Única (SOLID) é o conceito de que qualquer objeto único em POO deve ser feito para uma função específica. Basicamente, faz parte dos princípios de programação apresentados por Robert Martin. Assim como no código, uma classe deve ter apenas um motivo para mudar, tornando o software mais sustentável, escalável e fácil de entender. Para adotar o SRP no desenvolvimento de software, você deve garantir que cada classe ou módulo tenha uma responsabilidade bem definida e que não esteja tentando fazer muitas coisas. Você também deve manter seus módulos desacoplados e usar interfaces claras e concisas para se comunicar entre eles. Para resumir isso, temos uma citação interessante:

> "Reúna as coisas que mudam pelo mesmo motivo e separe as coisas que mudam por motivos diferentes." — O'Reilly

Podemos dizer que este é um dos melhores e mais essenciais princípios para construir um bom projeto de arquitetura, pois significa que um microsserviço, módulo, classe, subsistema ou função não deve ter vários motivos para mudar. Vamos entender este Princípio com um exemplo:

Um portal de comércio eletrônico pode ter uma arquitetura de microsserviços como esta:

<img width="720" height="417" alt="image" src="https://github.com/user-attachments/assets/c6bf1f1e-051e-4c74-a36a-d0c510999ae7" />

Aqui, todos os serviços (por exemplo, `Serviço de Listagem de Produtos`, `Serviço de Pedidos`, `Atendimento ao Cliente`, `Serviço de Pagamento`, `Serviço de Carrinho`, `Serviço de Lista de Desejos`, etc.) têm responsabilidades únicas. Isso significa que é importante certificar-se de que você não está integrando um serviço com outro quando não for absolutamente necessário, pois torna a arquitetura mais complicada de manter e testar.

**Construa equipes com responsabilidades claras**: Para desenvolver a arquitetura de microsserviços, precisamos construir equipes que tenham responsabilidades claras. Isso pode ser feito de várias maneiras, como equipes baseadas em funções, equipes multifuncionais, etc. Nessa arquitetura, cada microsserviço funciona como um aplicativo independente. Portanto, cada equipe deve ser versátil o suficiente para lidar com suas operações.

Vamos entender isso com um exemplo: Uma organização pode ter equipes baseadas em funções, como desenvolvedores de UI/UX, desenvolvedores front-end, desenvolvedores back-end, administradores de banco de dados, QAs, desenvolvedores de middleware, etc., que trabalham isoladamente, mas interagem diariamente por meio de reuniões – pessoalmente ou usando várias ferramentas de comunicação como JIRA, Slack e assim por diante.

Quando pensamos em manutenção, às vezes pequenos bugs ou às vezes até grandes bugs também podem ocorrer no sistema. Portanto, o SCRUM pode ser uma solução possível. Ajuda cada membro da equipe a encurtar o tempo de inconsciência. Mas como as equipes são organizadas com base nas funções, a integração de uma atualização em um sprint pode se tornar uma tarefa complicada. Por exemplo, se os desenvolvedores de UI/UX não obtiverem nenhuma informação dos caras do servidor sobre as alterações em uma API, a nova API não será útil.

Então, qual é a solução?

**Crie equipes multifuncionais com responsabilidades claras, para ajudar a orquestrar o trabalho entre as equipes**: Uma equipe multifuncional responsável por toda a funcionalidade de microsserviços pode ser um grande benefício para o seu projeto. Essa equipe deve consistir em membros de todas as equipes baseadas em funções e é responsável por orquestrar as várias partes do aplicativo, ou seja, interface do usuário, desenvolvimento, banco de dados e até mesmo controle de qualidade. 

Se houver duas versões do aplicativo, ou seja, web e mobile, os desenvolvedores de ambas as equipes devem estar presentes nessa equipe. O principal benefício desse tipo de equipe é que fica fácil resolver bugs, desenvolver novos recursos e implantá-los no ambiente de produção.

![e](https://github.com/user-attachments/assets/ca7b964a-d5fe-4104-8437-ff376e160ba8)

Use as ferramentas e estruturas certas: A essa altura, você provavelmente já projetou seus microsserviços para implantá-los de forma independente, agora você deve perceber o valor ideal desses microsserviços. E para fazer isso, você precisa automatizar o gerenciamento de compilação e implantação usando um bom conjunto de ferramentas de DevOps.

Usar as ferramentas, estruturas e bibliotecas certas ajudará muito na implementação de uma arquitetura de microsserviços. Se você planeja fazer isso em Java, considere o Spring Boot Project. Escolher as ferramentas e estruturas certas leva muito tempo e esforço, então aqui está uma lista de ferramentas e tecnologias comprovadas para o trabalho:

<img src="https://github.com/user-attachments/assets/2d955a04-5dac-439a-8a8c-592b1ad0e334" align="right" height="677">

- Jenkins e Bamboo para automação de implantação
- Docker para conteinerização
- Postman para teste de API
- Kubernetes para orquestração e implantação de contêineres
- Logstash para monitoramento
- DevSecOps para gerenciar todo o processo do ciclo de vida de desenvolvimento de software
- GitHub para gerenciamento de código-fonte e controle de versão
- Serviço de fila simples da Amazon para mensagens
- SonarQube para verificar a qualidade e segurança do código
- Ansible para gerenciar sua configuração
- Jira para rastreamento de problemas e gerenciamento de projetos
- Manter a comunicação assíncrona entre microsserviços

**Dois tipos de comunicação ocorrem entre microsserviços: Síncrono e Assíncrono**. Vamos entender isso com um exemplo: Para uma plataforma de comércio eletrônico, a comunicação síncrona significa que o usuário deverá "permanecer na linha" e avançar por uma série de etapas (selecionar itens, adicionar endereço de entrega, detalhes de pagamento, verificação do pedido), resultando na notificação do cliente "Obrigado pelo seu pedido! Estamos entregando na próxima semana".

Existem várias comunicações assíncronas que também ocorrem quando a notificação do cliente é processada e que fazem parte do estágio de "atendimento" do pedido, como: notificação de armazém, atualização de estoque, etc.

No caso de comunicação síncrona, um serviço torna-se dependente de outro serviço. Às vezes, torna-se um processo demorado concluir toda a tarefa usando a comunicação síncrona entre vários microsserviços.

Por outro lado, as comunicações assíncronas não dependem umas das outras. Assim, cada serviço pode levar seu tempo para concluir sua tarefa. Portanto, deve-se tentar maximizar a comunicação assíncrona entre microsserviços sempre que possível. Ele reduz a dependência e aumenta a eficiência geral de um aplicativo.

Você pode ver um exemplo disso abaixo:

<img width="720" height="417" alt="image" src="https://github.com/user-attachments/assets/c12e82e2-0727-4d12-bdaf-90c241acc92b" />

**Adote o modelo DevSecOps e proteja microserviços**: A segurança é muito importante nessa arquitetura. À medida que a arquitetura de microserviços evoluiu no desenvolvimento de aplicações nativas em nuvem, as práticas DevSecOps são cada vez mais utilizadas para garantir integração contínua e entrega contínua com medidas de segurança reforçadas. Uma build de aplicação usando microserviços pode ser dividida nos seguintes tipos de código:

1. Código de aplicação (lógica central)
2. Código de serviço de aplicação (conexões de rede, estabelecimento de sessões, etc.)
3. Infraestrutura (recursos de armazenamento de dados, rede, plataformas, etc.)
4. Monitoramento (observabilidade contínua da aplicação)

DevSecOps consiste em três conceitos: desenvolvimento, segurança e operações, e provou ser um paradigma facilitador para tipos de código com primitivas como integração contínua, entrega contínua e pipelines de implantação contínua. Esses pipelines são fluxos de trabalho para usar o código-fonte dos desenvolvedores para desenvolver, testar, implantar e muitas outras operações que são suportadas por ferramentas automatizadas com mecanismos de feedback. Além disso, faz com que as equipes de desenvolvimento entreguem código melhor e mais seguro mais rapidamente. As práticas DevSecOps em arquitetura de microserviços oferecem inúmeros benefícios, tais como:

- Alta garantia de segurança
- Redução da vulnerabilidade do código
- Melhoria da qualidade do produto
- Aumento da produtividade
- Aumento da velocidade das operações
- Entregar softwares melhores e de maior qualidade mais rapidamente

![unnamed](https://github.com/user-attachments/assets/b63080fa-2cb5-4184-8a0c-4d14744d6691)

**Use um armazenamento de dados separado para cada microserviço**: Uma prática importante é garantir que haja um banco de dados separado para armazenar dados sempre que possível, em vez de ter o mesmo banco de dados para múltiplos microserviços, como em uma arquitetura monolítica. No entanto, uma análise mais aprofundada pode indicar que um microserviço funciona apenas com um subconjunto de tabelas de banco de dados, enquanto, por outro lado, outro microserviço só funciona com um subconjunto totalmente novo de tabelas. E se ambos os subconjuntos de dados forem ortogonais, isso seria um caso para separar o banco de dados em serviços separados. Portanto, certifique-se de ter um armazenamento de dados separado para seus microserviços, a fim de reduzir a latência e melhorar a segurança. Isso já foi mencionado muitas vezes, mas é importante enfatizar que os microserviços devem depender o mínimo possível uns dos outros.

Um dos principais atributos da arquitetura de microserviços é que os dados de cada serviço são privados, como acontece, por exemplo, com o padrão Banco de Dados por Serviço.

<img width="720" height="375" alt="image" src="https://github.com/user-attachments/assets/dcc7b633-1f80-4fef-8091-4f5f5a4a01fb" />

Também podemos usar um servidor de banco de dados compartilhado que pode ser usado por múltiplos serviços com separação lógica de seus dados.

Implante cada microserviço separadamente
Se você está implantando cada microserviço separadamente, certamente vai economizar muito tempo coordenando com várias equipes enquanto mantém ou atualiza os esforços. Além disso, se um ou mais microserviços tiverem os mesmos recursos, recomendamos que você use uma infraestrutura dedicada para isolar cada microserviço de falhas e evitar uma queda completa.

Alguns dos padrões mais comuns e populares para implantação de microserviços são:

1. Múltiplas instâncias de serviço por host
2. Instância de serviço por contêiner
3. Instância de serviço único por host
4. Instância de serviço por VM
5. Orquestração de microserviços

A orquestração dos seus microserviços é um dos fatores mais influentes para alcançar sucesso tanto no processo quanto nas ferramentas. Você pode usar o Docker para rodar containers em uma VM, mas ele não oferece o mesmo nível de resiliência que uma plataforma de orquestração de containers oferece. Essa decisão pode muito bem afetar negativamente seu tempo de atividade ao tentar adotar uma arquitetura de microserviços.

<img src="https://github.com/user-attachments/assets/ec3b7c8e-29c2-4361-a6d3-d7bc17599bce" align="right" height="177">

Aqui estão algumas das plataformas de orquestração que já foram comprovadas: Essas plataformas podem ser úteis para gerenciar o provisionamento e implantação de contêineres, balanceamento de carga, escalabilidade, preocupações com comunicação em rede, etc.

- K8s (Kubernetes)
- AKS (Azure Kubernetes Services)
- ECS (Serviços de Contêineres Elásticos da Amazon)
- Azure Container Apps

Use um sistema de monitoramento eficaz: A arquitetura de microserviços ajuda você a realizar uma enorme escalabilidade de milhares de serviços modulares e oferece potencial para maior velocidade e métodos organizados de monitoramento. É importante, no entanto, revisar todos os seus microserviços e verificar regularmente se eles estão funcionando como desejado e utilizando eficientemente os recursos disponíveis. Dependendo dessas observações, você pode tomar as atitudes apropriadas caso as expectativas não estejam sendo atendidas.

Vamos analisar uma situação de exemplo e imaginar que você aplicou um padrão de arquitetura de microserviços que não tem capacidade para lidar com requisições, mas que ainda estão rodando. Por exemplo, se ele ficar sem conexões de banco de dados, o sistema de monitoramento deve ser capaz de gerar um alerta sempre que uma instância falhar e as requisições devem ser roteadas para instâncias de serviço em funcionamento.

Monitorar microserviços e manter essas estatísticas explicadas com precisão ajudará você a melhorar a tomada de decisões e manter seus microserviços disponíveis quando necessário.

Vamos dar uma olhada em alguns exemplos de ferramentas de monitoramento de microserviços.

- AWS CloudWatch: um serviço de monitoramento, observabilidade e gerenciamento que coleta e visualiza logs em tempo real e fornece insights acionáveis para aplicações e recursos de infraestrutura da AWS, híbridos e locais.

- Jaeger: software projetado para monitorar e solucionar problemas complexos em um ambiente de microserviços.

- Datagod: uma plataforma de observabilidade, segurança e análise para aplicações em escala de nuvem que oferece uma solução abrangente para bancos de dados, serviços e ferramentas usando uma plataforma de análise de dados baseada em SaaS.

- Graphite: como o nome sugere, é um software de código aberto que monitora e grava graficamente dados numéricos de séries temporais e fornece insights aprofundados sobre o sistema subjacente.

- Prometheus: uma ferramenta de software livre e de código aberto que oferece soluções de monitoramento e modificação.

<img src="https://user-images.githubusercontent.com/61624336/209388964-cc8c82aa-206e-4643-93ca-153a129d2334.svg" height="77" align="right">

Outro ponto bastante importante, em um contexto de microsserviços, é sobre um **domínio** (domain) que refere-se a uma parte específica ou a um conjunto de funcionalidades de um sistema maior que é dividido em microsserviços, os domínios podem ser considerados como o núcleo de um microsserviço em uma arquitetura baseada nessa divisão. Em termos de design de microsserviços, a ideia é organizar serviços em torno de áreas específicas de funcionalidade ou de um contexto de negócios. 

Essas áreas específicas são comumente referidas como domínios. Cada microsserviço é responsável por lidar com um domínio específico do negócio ou uma parte bem definida da aplicação. Os microsserviços são projetados para serem autônomos e independentes, e a ideia é que cada um deles se concentre em um domínio delimitado. Por exemplo, em um sistema de e-commerce, pode haver microsserviços separados para lidar com a gestão de produtos, carrinho de compras, processamento de pedidos, autenticação de usuários, etc. 

Cada um desses microsserviços abordaria um domínio específico do sistema. Ao dividir um sistema em microsserviços baseados em domínios, há vantagens como:

- Escalabilidade e Desempenho: Cada microsserviço pode ser escalado independentemente, focando nos domínios mais exigidos.

- Manutenção e Evolução: Mudanças em um domínio específico podem ser feitas sem afetar outros microsserviços, facilitando a manutenção e evolução do sistema.

- Desenvolvimento Ágil: Equipes podem se concentrar em microsserviços específicos, acelerando o desenvolvimento e permitindo que cada equipe tenha autonomia sobre o seu domínio.

A **lógica de domínio** é uma parte fundamental do desenvolvimento de software, onde reside a essência das regras de negócio e o comportamento específico de um determinado domínio ou área de conhecimento. Ela encapsula as regras, restrições e operações que governam o funcionamento e as relações dentro desse domínio. Lembrando que em um sistema de software, o domínio refere-se à área de negócio ou problema que o software está sendo desenvolvido para resolver. Por exemplo, em um sistema bancário, o domínio pode incluir conceitos como contas, transações, clientes, etc.

A lógica de domínio trata dessas entidades e das operações que podem ser realizadas sobre elas. Ela não está ligada diretamente à implementação técnica, como a interface do usuário ou o armazenamento de dados, mas sim à representação das regras e processos que definem o comportamento do sistema.

Por exemplo, no contexto de um sistema de reservas de voos, a lógica de domínio pode incluir regras sobre disponibilidade de assentos, restrições de datas, políticas de cancelamento e assim por diante.

A separação da lógica de domínio é um princípio fundamental no design de software, como na arquitetura em camadas ou no uso de padrões como o Modelo de Domínio, onde a lógica de domínio é isolada e mantida separada das outras partes do sistema. Isso facilita a manutenção, a compreensão e a evolução do software, uma vez que as mudanças no domínio podem ser feitas sem afetar desnecessariamente outras partes do sistema.

É possível implementar microsserviços em aplicativos desktop, web e móveis. A arquitetura de microsserviços é uma abordagem na qual um aplicativo é construído como um conjunto de serviços pequenos e independentes, cada um focado em realizar uma função específica. Para aplicativos desktop e móveis, os microsserviços podem ser implementados de maneira semelhante aos aplicativos web. Os serviços podem ser desenvolvidos separadamente e podem se comunicar por meio de APIs (Interfaces de Programação de Aplicativos), permitindo que diferentes partes do aplicativo interajam entre si de forma independente. 

Você pode utilizar programação com sockets também em microsserviços, embora não seja a abordagem mais comum. A programação com sockets permite uma comunicação direta e bidirecional entre os serviços, o que pode ser vantajoso em algumas situações específicas. No entanto, é importante considerar os prós e contras dessa abordagem em comparação com os métodos mais comuns de comunicação entre microsserviços, como HTTP/REST, gRPC e mensageria. Você pode desenvolver um sistema de compartilhamento de arquivos P2P usando sockets em uma arquitetura de microsserviços que é uma abordagem viável e pode trazer várias vantagens em termos de escalabilidade, flexibilidade e manutenção, e é crucial garantir a robustez e a segurança do sistema. Implementar medidas de autenticação, autorização e criptografia de dados é essencial para proteger os dados dos usuários e manter a integridade do sistema. Além disso, monitorar e gerenciar a comunicação entre os peers é fundamental para assegurar a eficiência e a escalabilidade da rede P2P.

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/185da4d4-c3de-49f5-bfdd-d06a0582f63c" align="right" height="177">

Por exemplo, em um aplicativo de e-commerce (sistema de vendas), pode haver um microsserviço para gerenciar o catálogo de produtos, outro para processar pagamentos, outro para gerenciar usuários e assim por diante. Cada um desses serviços pode ser desenvolvido separadamente e ser consumido pelo aplicativo desktop ou móvel por meio de chamadas de API. No entanto, é importante considerar alguns desafios ao implementar microsserviços em aplicativos desktop e móveis, como a latência da rede em dispositivos móveis, o consumo de recursos, a sincronização de dados offline e a segurança na comunicação entre os serviços. Com uma arquitetura bem planejada e estruturada, é viável implementar microsserviços em aplicativos desktop e móveis, aproveitando os benefícios de escalabilidade, manutenção simplificada e flexibilidade no desenvolvimento e atualização de diferentes partes do aplicativo.

A definição clara de limites de domínio é essencial para o sucesso dos microsserviços. Isso envolve identificar fronteiras bem definidas entre os diferentes domínios, para que cada microsserviço possa ser desenvolvido, mantido e escalado de forma independente. A comunicação entre os microsserviços geralmente é realizada através de APIs, independente do tipo arquitetural delas, permitindo que eles interajam uns com os outros para cumprir processos mais complexos ou fluxos de trabalho do sistema maior.

Nem sempre um domínio é diretamente equivalente a um microsserviço, embora essa seja uma maneira comum de organizar a arquitetura de microsserviços. Em muitos casos, um microsserviço pode abranger mais de um domínio, ou pode haver múltiplos microsserviços lidando com um único domínio. A ideia principal é que cada microsserviço seja especializado em uma área específica do negócio, mas a definição exata dos limites de um microsserviço pode variar dependendo do contexto e da complexidade do sistema.

Por exemplo, em um sistema de comércio eletrônico, pode haver um microsserviço responsável pela gestão de pedidos, que abrange vários domínios, como processamento de pagamentos, verificação de disponibilidade de produtos, gerenciamento de estoque, etc. Este microsserviço pode abranger múltiplos domínios, mas ainda está focado em uma área específica do negócio: o fluxo de pedidos.

Por outro lado, pode haver um domínio como o de autenticação e gerenciamento de usuários, que é abordado por vários microsserviços. Um microsserviço pode ser responsável pela autenticação, outro pelo gerenciamento de perfis de usuários e outro pelo controle de acesso.

A chave é encontrar um equilíbrio entre a granularidade dos microsserviços e a clareza das responsabilidades de cada um. A divisão deve permitir que os microsserviços sejam suficientemente independentes para serem desenvolvidos, implantados e mantidos de maneira ágil, mas também devem colaborar de forma eficiente para atender às necessidades do sistema como um todo.

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/59cecdee-0e6a-4d8c-a115-6dd18d979a8f" height="777"></td>
		<td><img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/c5d3b0dd-3df3-4eac-878a-a86803221771" height="777"></td>
		<td><img src="https://github.com/user-attachments/assets/90283b3a-8d82-4e72-8829-81fe65396b0f" height="777"></td>
	</tr>
</table>

A arquitetura de microsserviços, também conhecida como "microsserviços", é a abordagem de criação de aplicativos como uma série de serviços com implementação independente e desenvolvimento descentralizado e autônomo. Esses serviços são pouco integrados, implementáveis com independência e fáceis de manter. Enquanto o aplicativo monolítico, estrutura centralizada, é criado como unidade indivisível, os microsserviços dividem essa unidade em uma coleção de unidades independentes que contribuem para o todo. Os microsserviços são parte integral do DevOps, pois são a base para práticas de entrega contínua que permitem que equipes se adaptem com rapidez aos requisitos do usuário.

Uma arquitetura de microsserviços é um tipo de sistema distribuído, pois decompõe um aplicativo em componentes ou “serviços” diferentes. Por exemplo, uma arquitetura de microsserviços pode ter serviços que correspondem a recursos de negócios (pagamentos, usuários, produtos etc.) em que cada componente correspondente lida com a lógica empresarial para essa responsabilidade. O sistema vai ter várias cópias redundantes dos serviços para que não haja um ponto central de falha para um serviço.

Com a arquitetura de microsserviços, desenvolvedores podem se organizar em equipes menores especializadas em serviços diferentes, com pilhas distintas e implementações dissociadas. Por exemplo, o Jira é formado por diversos microsserviços, e cada um representa uma funcionalidade específica, como pesquisa de itens, visualização de informações sobre o item, comentários, transições de item e muito mais.

<img src="https://user-images.githubusercontent.com/61624336/232251177-abafc647-65f7-4fd4-ad93-213395659fa2.png" align="right" height="307">

Então, baseado em um contexto histórico, uma forma de desenvolver uma aplicação é colocar todas as funcionalidades em um único "lugar". Ou seja, a aplicação roda em uma única instância (ou servidor) que possui todas as funcionalidades. Isso talvez seja a forma mais simples de criar uma aplicação (também a mais natural), mas quando a base de código cresce, alguns problemas podem aparecer. Por exemplo, qualquer atualização ou `bug fix` necessita parar todo o sistema, buildar o sistema todo e subir novamente. Isso pode ficar demorado e lento. Em geral, quanto maior a base de código, mais difícil será para manter ela mesmo com uma boa cobertura de testes e as desvantagens não param por ai. Outro problema é se alguma funcionalidade possuir um gargalo no desempenho o sistema todo será afetado. Não é raro de ver sistemas onde relatórios só devem ser gerados à noite para não afetar o desempenho de outras funcionalidades. Outro problema comum é com os ciclos de testes e builds demorados (falta de agilidade no desenvolvimento), problemas no monitoramento da aplicação ou falta de escalabilidade. Enfim, o sistema se torna um legado pesado, onde nenhum desenvolvedor gostaria de colocar a mão no fogo.

Então, a ideia é fugir desse tipo de arquitetura monolítica (com os padrões arquiteturais MVC, MVVP, PVC, MVP) monstruosa e dividir ela em pequenos pedaços. Cada pedaço possui uma funcionalidade bem definida e roda como se fosse um "mini sistema" isolado. Ou seja, em vez de termos uma única aplicação back-end enorme, teremos várias instâncias menores que dividem e coordenam o trabalho. Essas instâncias são chamadas de Microserviços (Microservices).

Agora fica mais fácil monitorar cada serviço específico, atualizá-lo ou escalá-lo pois a base de código é muito menor, e assim o deploy e o teste serão mais rápidos. Podemos agora achar soluções específicas para esse serviço sem precisar alterar os demais. Outra vantagem é que um desenvolvedor novo não precisa conhecer o sistema todo para alterar uma funcionalidade, basta ele focar na funcionalidade desse microsserviço.

> Importante também é que um microsserviço seja acessível remotamente, normalmente usando o protocolo HTTP trocando mensagens JSON ou XML, mas nada impede que outro protocolo seja usado. Um microsserviço pode usar outros serviços para coordenar o trabalho.

Repare que isso é uma outra abordagem arquitetural bem diferente do monolítico e por isso também é chamado de arquitetura de microsserviços.

Por fim, uma arquitetura de Microserviços tem um grau de complexidade muito alta se comparada com uma arquitetura monolítica. Aliás, há aqueles profissionais que indicam partir para uma arquitetura monolítica primeiro e mudar para uma baseada em microsserviços depois, quando estritamente necessário.

Repare que a UI, ou seja nossa View ou aplicação front-end, fica dividida para cada microservice (nossas APIs) contendo as regras de negócio e acesso a camada de dados, e nossos microserviços ficam divididos ou se relacionando com os outros a fim de realizar uma tarefa necessária no nosso back-end e atuando em banco de dados próprios para os microsserviços específicos.

Os microservices podem ser trabalhados com patterns (padrões) em seu desenvolvimento, tais como:

<img src="https://github.com/user-attachments/assets/506e2fcd-3f04-4d9a-a13a-fa306801ab85" align="right" height="477">

- **API Gateway pattern**: Esse padrão envolve ter um único ponto de entrada para todas as solicitações do cliente, que encaminha essas solicitações para o microsserviço apropriado. Isso simplifica a comunicação com os clientes e permite que o gateway lide com funções como autenticação, autorização e transformação de dados.

- **Circuit Breaker pattern**: Este padrão é utilizado para lidar com falhas em uma arquitetura de microsserviços. Quando um microsserviço falha ou deixa de responder, o disjuntor dispara e redireciona as solicitações para um serviço de fallback.

- **Retry pattern**: Automaticamente tenta novamente as operações (requests) que falharam para prover as chances de sucesso.

- **Service Registry pattern**: Este padrão é usado para rastrear todos os serviços em uma arquitetura de microsserviços. O registro atua como um diretório central para descoberta de serviço.

- **Mesh Service pattern**: esse padrão envolve a adição de uma camada de infraestrutura entre microsserviços para lidar com preocupações transversais, como descoberta de serviço, balanceamento de carga e segurança.

- **Event-Driven Architecture pattern**: esse padrão envolve o uso de eventos para comunicação entre microsserviços. Cada microsserviço pode publicar eventos e assinar eventos publicados por outros microsserviços.

- **Saga pattern**: Este padrão é usado para gerenciar transações que abrangem vários microsserviços. Envolve dividir a transação em etapas individuais menores e usar ações de compensação para desfazer as etapas concluídas se ocorrer um erro.

- **Bulkhead pattern**: Este padrão é utilizado para isolar falhas em uma arquitetura de microsserviços. Cada microsserviço é colocado em um contêiner separado, portanto, se um microsserviço falhar, ele não afetará outros microsserviços.

- **Sidecar pattern**: esse padrão envolve a implantação de um contêiner separado ao lado de cada microsserviço para lidar com preocupações transversais, como registro, monitoramento e segurança.

- **CQRS pattern**: Esse padrão envolve a separação dos modelos de leitura e gravação em uma arquitetura de microsserviços. O modelo de leitura é otimizado para consultar dados, enquanto o modelo de gravação é otimizado para atualizar dados.

- **Strangler pattern**: esse padrão envolve a substituição gradual de um aplicativo monolítico por microsserviços, adicionando gradualmente novos microsserviços e removendo a funcionalidade do monólito.

- **Shared Database pattern**: esse padrão é praticamente uma base de dados compartilhada, ela é muito comum no processo pós migração de arquiteturas monolíticas para microsserviços. Onde os microsserviços vão sendo criados e vão ficando independentes, mas a base de dados ainda continua sendo compartilhada nesse serviço.

- **Database Per Service pattern**: esse padrão é chamado de banco de dados por serviço, onde cada serviço geralmente possui seu próprio banco de dados, o que ajuda a evitar acoplamento entre serviços e permite que cada serviço escolha o banco de dados mais adequado às suas necessidades.

- **Test Automation patten**: Automatizar testes, incluindo testes de unidade, testes de integração e testes de aceitação, para garantir a qualidade e a confiabilidade dos microsserviços.

<img src="https://github.com/user-attachments/assets/5d535c27-fda8-46eb-b138-29b027d651b6" align="right" height="577">

Ao desenvolver microsserviços, precisamos seguir as seguintes boas práticas:

1. Utilizar armazenamento de dados separado para cada microsserviço

2. Manter o código em um nível de maturidade semelhante

3. Realizar builds separados para cada microsserviço

4. Atribuir a cada microsserviço uma única responsabilidade

5. Implantar em contêineres

6. Projetar serviços sem estado

7. Adotar o design orientado a domínio (DDD)

8. Projetar micro front-ends

9. Orquestrar microsserviços

Lembre-se de que a escolha dos padrões arquiteturais depende dos requisitos específicos do projeto e das necessidades de negócios. Não existe uma única abordagem correta para a arquitetura de microsserviços, e você pode combinar vários desses padrões de acordo com suas necessidades. O importante é manter os princípios de isolamento, independência e coesão ao projetar e implementar microsserviços.

Exemplo: Microservices Communication - Implementando duas APIs e realizando comunicações síncronas e assíncronas via chamadas HTTP por meio de API REST e fila de mensagens com RabbitMQ. Por fim, iremos subir toda a aplicação no Docker com docker-compose, e iremos disponibilizar também no Heroku. Cada microsserviço vai cuidar de uma parte específica dentro do sistema.

Na prática, iremos simular um pequeno <a href="#">sistema de vendas</a>:

1. Teremos uma API isolada em Node.js para nos autenticar que através do nome do usuário e a senha ele vai gerar um token de acesso e nisso ele será usado em todas as aplicações e todos os endpoints,
2. Outra API Node.js será responsável por registrar vendas,
3. API em Spring responsável por cuidar do estoque de produtos.
4. Toda vez que uma venda for realizada na aplicação de vendas em Node.js, será enviada uma mensagem da API de vendas para a API de produtos para que o estoque seja atualizado.
5. Para a realização de cada venda, será necessário requisitar para a API de produtos os dados dos IDs dos produtos que constam no carrinho de compras.
6. Ao receber uma mensagem de venda para atualizarmos o estoque, retornaremos uma mensagem para a aplicação de vendas informando se foi tudo ok ou não, para atualizá-la para `CANCELADA` ou `CONCLUÍDA`.

O conceito chave dessa aplicação é entender como funciona os microserviços, onde cada serviço cuida de uma parte pequena da aplicação, onde estamos descentralizando os serviços da API que seria de uma aplicação monolítica para uma aplicação em microsserviços.

O interessante é que vamos requisitar em uma comunicação síncrona por isso quando a gente tiver mensagem vai ser uma comunicação assíncrona a gente vai utilizar repetindo aquilo que vai ser isso a gente vai mandar uma mensagem a outra aplicação não vai escutar isso na hora a gente vai mandar para o repetir e vai ter. Isso vai cair numa fila.

Vai ter alguma outra aplicação que vai estar ouvindo essa fila em algum momento. Não precisa ser naquele exato instante que a gente publicou e quando ela ouvir ela vai processar essa mensagem.

Então beleza vamos supor que nossa aplicação caiu ela está fora por motivos de falta de alguma atualização gente que teve que dar um build lá em produção. Então a gente publicou uma mensagem e se ela estiver fora não vai impactar no nosso processamento da informação.

A aplicação vai estar fora a beleza mas em algum momento ela vai voltar a ficar operante e quando ela voltar a ficar operante ela vai processar essa mensagem e vai dar sequência no fluxo para realização de cada venda vai ser necessário requisitar então os produtos porque como a gente vendia só usar em dias a gente vai buscar todos os produtos informados no carrinho de compras e vai salvar eles da venda salvou a venda vai ficar com pendente.

A gente vai publicar a mensagem para pedir produtos e lá ele vai receber os produtos que a gente está tentando vender e a quantidade.

Então ele vai atualizar esse estoque caso vamos supor que a gente é formular o produto. Ele tem só lá no produto ele tem esse tipo dois itens só em estoque e a gente mandou fazer uma venda com cinco. A gente não vai conseguir atualizar essa venda para concluir ela vai ter que ser cancelada porque a gente não tem esse estoque disponível. Ou então vamos supor que a gente tem dois anos de estoque e a gente quer vender só um.

A gente vai embeleza a gente vai atualizar esse estoque para 1 e a gente vai finalizar essa venda a gente vai devolver uma mensagem para fazer uma nova publicação como concluída para a área de vendas.

Então assim a gente vai ter um método para publicar e para ele escutar mensagens um vice e um senador ou então publisher chegou subscrever tanto nas duas APIs de venda de produtos porque a gente vai implementar a lógica de ouvir as filas e de publicar nas filas tanto no Japão quanto no novo vocês conseguem ter uma noção de como faz em cada uma dessas tecnologias.

E essa aqui é uma imagem que eu criei um diagrama especificando como é que vai ser a nossa arquitetura aqui no quadrado principal e a aplicação em si. A aplicação de Java naqueles produtos é a aplicação de jazz que é de vendas. Elas vão se comunicar de maneira síncrona via chamadas HTTP através de uma API REST. E a gente vai ter uma token JWT protegendo essas chamadas.

Esse toque vai ser chamado por essa aplicação mas porque ele está num quadro de separado porque ela não vai ter interação alguma com essas aplicações. Ela só vai gerar em stock mas nada elas não vão se comunicar em momento algum nem envia via mensagem e nem envia chamada Oeste e também eu coloquei que servidor Red time que o que ele vai ser um serviço de mensageiro.

A gente vai subir um contêiner Docker. Então a gente faz com que Os dois que têm uma faixa de bidirecional por que ele vai enviar e escutar. Ele também vai enviar e vai escutar tanto a venda quanto produtos irão enviar ou escutar mensagens para esse servidor.

A gente vai ter um bom banco de dados em mongoDB para o próprio e de vendas. 

A gente vai ter um banco de dados imposto de Goiás que ele próprio de produto e a gente vai ter um pouco das dados que SQL para pedir de autenticação. Esse último quadrado aqui em cima de toque com poucos a gente vai a gente tem todos os contêineres.

A gente tem um total de sete contêineres. A gente vai ter então dois contentes do posto de Goiás que é um para aplicação de autenticação e aplicação de produtos. Vamos repetir aqui porque são dois são dois deles então um do Acre também uma antena para aplicação de produtos ou uma aplicação de autenticação de vendas do Banco de Gutemberg.

E sempre o time caiu e a gente vai subir tudo isso com o Dakar pulso a ideia que a gente dê apenas um Docker Compose e ele consiga subir todo todas aqui e já ter o sistema pronto para gente utilizá-la. O utilizador vai fazendo chamadas pelo Postman coisas do tipo.

A arquitetura de microsserviços é a bala de prata? O diagrama abaixo mostra por que os jogos em tempo real e os aplicativos de negociação de baixa latência não devem usar a arquitetura de microsserviço.

<table>
	<tr>
		<td><img height="577" src="https://github.com/user-attachments/assets/c14d1c83-b66c-447a-a993-015bfa4f2a50" /></td>
		<td><img height="577" src="https://github.com/user-attachments/assets/bac174a0-22f1-404d-895d-8b6f29e2c527" /></td>
	</tr>
</table>

Existem alguns recursos comuns a esses aplicativos, que os fazem escolher a arquitetura monolítica:

- Esses aplicativos são muito sensíveis à latência. Para jogos em tempo real, a latência deve estar no nível de milissegundos; Para negociação de baixa latência, a latência deve estar no nível de microssegundos. Não podemos separar os serviços em processos diferentes porque a latência da rede é insuportável.

- A arquitetura de microsserviços geralmente é sem estado e os estados são mantidos no banco de dados. Os jogos em tempo real e a negociação de baixa latência precisam armazenar os estados na memória para atualizações rápidas. Por exemplo, quando um personagem é ferido em um jogo, não queremos ver a atualização 3 segundos depois. Esse tipo de experiência do usuário pode matar um jogo.

- Os jogos em tempo real e a negociação de baixa latência precisam se comunicar com o servidor em alta frequência, e as solicitações precisam ir para a mesma instância em execução. Portanto, conexões de soquete da web e roteamento fixo são necessários.

Portanto, a arquitetura de microsserviços é projetada para resolver problemas para determinados domínios. Precisamos pensar no "porquê" ao projetar aplicativos.

👉 Para você: você já se deparou com situações semelhantes no trabalho quando teve que escolher uma arquitetura diferente de microsserviço?

<img width="720" height="378" alt="image" src="https://github.com/user-attachments/assets/4eddd12f-070c-4835-b1c7-5585db5b4932" />

Quando falamos de aplicações monolíticas, dissemos que a comunicação em aplicações monolíticas é uma comunicação entre processos. Isso significa que ele está trabalhando em um único processo que invoca um para o outro usando chamadas de método. Basta criar uma classe e chamar o método dentro do módulo de destino. Todos executando o mesmo processo.

Essa comunicação é muito simples, mas ao mesmo tempo os componentes são altamente acoplados uns aos outros e difíceis de separar e escalar de forma independente.

Use um sistema de monitoramento eficaz: A arquitetura de microserviços ajuda você a realizar uma enorme escalabilidade de milhares de serviços modulares e oferece potencial para maior velocidade e métodos organizados de monitoramento. É importante, no entanto, revisar todos os seus microserviços e verificar regularmente se eles estão funcionando como desejado e utilizando eficientemente os recursos disponíveis. Dependendo dessas observações, você pode tomar as atitudes apropriadas caso as expectativas não estejam sendo atendidas.

Essa comunicação é muito simples, mas ao mesmo tempo os componentes são altamente acoplados uns aos outros e difíceis de separar e escalar de forma independente.

Construir software escalável exige que um engenheiro/arquiteto de software escolha a arquitetura certa, especialmente ao construir software/aplicações empresariais.

Arquitetura monolítica geralmente é a primeira escolha em mente para a maioria dos engenheiros porque é fácil e não precisa lidar com a complexidade do sistema distribuído, já que toda uma aplicação está no mesmo enorme código quando lida com entrega ágil de software; A aplicação monolith pode não ser a escolha certa porque, quando fazer pequenas alterações no código exige que implantemos uma aplicação inteira, o que pode ser demorado, outra coisa é que nem podemos escalar componentes/serviços individuais.

Se houver um erro em qualquer módulo/funcionalidade/serviço, isso pode afetar a disponibilidade de toda a aplicação e é por isso que a <a href="https://medium.com/javarevisited/do-you-know-about-microservices-and-their-design-patterns-e8d7c8193dfe">Microservice Architecture</a> vem ao resgate.

Aqui estão os 10 padrões de microserviços que os engenheiros de software devem conhecer:

![633988640_1671001741014720_1873344397966094120_n](https://github.com/user-attachments/assets/453bef11-af5a-451a-9a02-19effeb2c8dd)

![Screenshot_20241022-230512_Instagram](https://github.com/user-attachments/assets/8b432d31-3848-4996-a1a5-92921fec1404)

![FB_IMG_1733228987280](https://github.com/user-attachments/assets/caf7b934-fde2-489c-affe-ce7e16241678)

![FB_IMG_1718629521831](https://github.com/user-attachments/assets/23486dd3-edb0-4b98-845b-3b6ac62c43db)

- API Gateway: É o ponto de entrada para acessar qualquer microserviço e podemos implementar aqui questões transversais como Segurança, Limite de Taxa e Balanceamento de Carga. Podemos usar o Spring Cloud Zuul ou o Spring Cloud Gateway para implementar isso.

- Service Discovery: Permitir que os serviços se encontrem por meio de um nome em vez de um IP. Por que não propriedade intelectual? Porque o IP frequentemente muda em tempo de execução devido à frequência com que os containers são girados e destruídos. Podemos usar o serviço Spring Cloud Eureka ou Kubernetes para implementar isso.

- Circuit breaker: Esse padrão é muito útil ao lidar com erros transitórios. Por exemplo, quando o serviço a chama o serviço b e o serviço b está indisponível (timeout), ele pode retornar um resultado de cache como resposta padrão ou um recurso de retenção para fazer uma solicitação a outro serviço auxiliar para obter o resultado e permitir que o serviço b recupere sem tentar fazer mais requisições para ele. Podemos usar Hystrix ou Resilient4J para implementar isso.

- Bulkhead: Esse padrão ajuda a lidar com a tolerância a falhas relacionada ao pool de threads, dividindo o pool de threads com base no número de serviços que precisavam ser chamados. Por exemplo, definimos um pool de 50 threads no serviço A e o serviço A fará requisições para os serviços B e C. Assim, o serviço A deve dividir o pool de 50 threads em 2 (25 para o serviço B, outros 25 para o serviço C), assim, se o serviço C não estiver disponível ou demorar mais para processar a solicitação, isso não afete a chamada do serviço B porque ele tem seu próprio pool de threads para realizar o trabalho. Podemos usar o Resilient4J para implementar isso.

- CQRS: poderíamos separar Command(write) e Query(read), o que significa que poderíamos projetar uma tabela de banco de dados otimizando para escrita e leitura de forma diferente para escalabilidade.

- Event Driven Pattern: Esse padrão permite um acoplamento frouxo entre serviços, o que significa que os serviços não precisam se conhecer para se comunicar. O protocolo de comunicação geralmente ocorre por meio de eventos usando Mensagens Queue, como AMQP (RabbitMQ) ou Apache Kafka.

- Saga: Como sabemos, lidar com sistemas distribuídos é difícil, especialmente quando se trata de transações distribuídas; O commit de 2 fases era a melhor opção, mas devido à sua natureza de bloqueio pessimista, dificulta escalar, por isso os padrões Saga entram em cena. Existem maneiras de implementar o padrão Saga, que são Orquestração e Coreografia.

- Strangler Pattern: Esta é uma forma de decompor uma aplicação monólita em microsserviços, extraindo gradualmente cada recurso do aplicativo monolítico em microsserviços individuais e permitindo que a aplicação monolítica chame esses novos microsserviços. Ao criar novos recursos, comece criando um novo microserviço em vez de criar esse novo recurso dentro do aplicativo monolito. A extração também pode incluir a criação de um novo banco de dados para esses novos serviços.

- Sidecar: Provavelmente um dos padrões mais legais de conhecer. Por quê? porque é uma forma de conectar serviços de negócios transversais como um sidecar ao serviço empresarial real. Normalmente, isso é feito implantando um serviço de sidecar no mesmo pod do serviço empresarial propriamente dito. Caso de uso: comunicação segura, entre serviço e serviço, implementação de logging ou métrica. Podemos usar o proxy do Envoy como sidecar.

- BFF: Também conhecido como Backend para Frontend. Implementar microserviços para cada plataforma permite mais personalização/otimização com base em cada plataforma. Por exemplo, um aplicativo móvel pode não precisar de fotos ou vídeos de grande porte como aplicativos web, mas lembre-se de que o serviço pode ser redundante.

Em um mundo onde produtos digitais precisam escalar globalmente, responder instantaneamente e lidar com milhares de usuários simultâneos — a comunicação tradicional síncrona de solicitação e resposta atinge seus limites.

Sistemas distribuídos modernos exigem padrões de comunicação assíncronos que reduzam a dependência, aumentem a resiliência e permitam que as equipes distribuam recursos de forma independente.

![FB_IMG_1727375403456](https://github.com/user-attachments/assets/4cafc8ec-3a3d-4943-8782-4049347483aa)

Se você está construindo SaaS nativo da nuvem, microserviços de alto desempenho ou automação corporativa — esses três padrões são suas armas essenciais:

- 👉 Event Bus
- 👉 CQRS
- 👉 Saga

**Component-based** é uma abordagem de arquitetura de software onde os sistemas são construídos a partir de unidades modulares e reutilizáveis chamadas componentes. Cada componente é uma entidade funcional independente, encapsulando dados, lógica de negócio e comportamento, podendo ser desenvolvido, testado e mantido de forma isolada. O principal objetivo do component-based é promover reutilização, manutenção facilitada, escalabilidade e separação de preocupações. Em vez de criar sistemas como blocos monolíticos de código interdependente, o component-based permite montar aplicações como se fossem conjuntos de peças de Lego, onde cada peça realiza uma função específica e pode ser substituída ou atualizada sem impactar o todo, desde que sua interface permaneça a mesma.

Na prática, os componentes possuem interfaces bem definidas e comunicam-se entre si de forma controlada, muitas vezes por meio de eventos, injeção de dependência ou contratos formais de dados. Isso os torna altamente portáveis e adaptáveis a diferentes contextos. No front-end, esse conceito é amplamente adotado em frameworks como React, Angular e Vue, onde cada parte da interface — como botões, formulários ou tabelas — é um componente reutilizável. No back-end, esse paradigma também pode ser aplicado através de serviços encapsulados ou bibliotecas modulares que se integram em uma arquitetura maior. Em ambientes mais complexos, os componentes podem evoluir para microcomponentes ou micro frontends, refletindo a mesma filosofia de modularidade.

Além disso, o desenvolvimento baseado em componentes favorece a testabilidade e o versionamento granular, pois cada unidade pode ser testada isoladamente e evoluída de forma segura. Também incentiva a colaboração entre equipes, permitindo que diferentes grupos trabalhem em diferentes componentes sem conflitos, o que é crucial em projetos grandes e distribuídos. No entanto, adotar component-based exige disciplina em design, pois é necessário definir interfaces estáveis, evitar acoplamentos desnecessários e gerenciar bem a comunicação entre os módulos. Quando bem aplicado, o component-based resulta em sistemas mais flexíveis, organizados e fáceis de escalar, permitindo evoluções constantes sem comprometer a estrutura já existente.

**Controller-Responder** é um padrão arquitetural frequentemente utilizado em aplicações web que seguem a arquitetura MVC (Model-View-Controller), onde o objetivo é separar ainda mais as responsabilidades dentro do fluxo de uma requisição HTTP. Ele propõe que o Controller atue como um intermediador entre a lógica de aplicação e a entrega da resposta, enquanto o Responder seja responsável exclusivamente por construir e formatar a resposta que será enviada ao cliente, seja ela uma página HTML, um JSON, um XML ou qualquer outro tipo de representação. Esse padrão ajuda a reduzir o acoplamento entre lógica de controle e formatação de resposta, melhorando a organização, legibilidade e manutenção do código.

A principal ideia é que o Controller manipula o caso de uso: recebe a requisição, valida, chama os serviços ou casos de uso, obtém o resultado e, em vez de ele próprio montar a resposta final, delega essa tarefa ao Responder. O Responder, por sua vez, é especializado em transformar os dados de saída do domínio ou do caso de uso em uma resposta apropriada para o protocolo e formato desejado. Por exemplo, enquanto o Controller pode apenas saber que um usuário foi autenticado com sucesso, é o Responder quem decide como essa informação será apresentada, estruturando a resposta HTTP com os dados corretos, cabeçalhos, códigos de status e formatação.

Esse padrão é muito útil em sistemas que lidam com múltiplos formatos de resposta ou que exigem clareza entre as etapas da aplicação. Também contribui para testes mais precisos, pois separa a lógica de negócios (que pode ser testada em nível de controller e serviço) da apresentação (testada via responder). Em síntese, o Controller-Responder promove um controle mais claro e segmentado sobre o fluxo de uma requisição e permite que cada parte do sistema seja responsável por uma única coisa: o controller decide o que aconteceu, o responder decide como mostrar isso.

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/33fbe46b-9d77-49ea-b5be-e2b09160517b">

**Broker** (Pub/Sub) é um padrão arquitetural e também um conceito amplamente utilizado em sistemas distribuídos, onde sua principal função é atuar como um intermediário entre componentes que produzem dados (produtores) e componentes que consomem dados (consumidores). 

Em vez de os produtores e consumidores se comunicarem diretamente, o broker recebe, organiza, encaminha ou até transforma as mensagens trocadas entre eles. Esse modelo é especialmente útil para desacoplar os elementos do sistema, garantindo que eles não dependam um do outro diretamente para operar, o que traz flexibilidade, escalabilidade e resiliência à arquitetura. Na prática, o broker funciona como uma central de mensagens ou eventos, um ponto de encontro onde os dados são enviados e de onde outros serviços podem consumi-los no tempo e da forma que preferirem.

Essa abordagem é muito comum em arquiteturas baseadas em eventos, como em sistemas que utilizam filas de mensagens (message queues) ou publicadores/assinantes (pub/sub). Um broker pode ser representado por tecnologias como RabbitMQ, Apache Kafka, ActiveMQ, Redis Streams ou MQTT, cada uma adequada a contextos e volumes diferentes. Por exemplo, num sistema de e-commerce, quando um pedido é realizado, o serviço de pedidos envia uma mensagem para o broker. Esse evento pode ser consumido simultaneamente por diferentes sistemas, como o de faturamento, o de estoque e o de envio, sem que o serviço de pedidos precise se preocupar em notificar cada um diretamente. O broker garante a entrega, o roteamento e, em alguns casos, até a persistência dessas mensagens, assegurando que nada se perca, mesmo em falhas temporárias dos consumidores.

Além disso, o uso de brokers contribui para a criação de sistemas assíncronos, o que melhora o desempenho e evita que um serviço precise esperar pela resposta de outro para continuar operando. Isso é essencial em ambientes de microserviços, onde os componentes são independentes e a comunicação entre eles precisa ser eficiente, confiável e tolerante a falhas. Em resumo, o broker é uma peça central que media a comunicação entre partes diferentes de um sistema, permitindo desacoplamento, tolerância a falhas e escalabilidade, além de tornar os sistemas mais organizados e preparados para lidar com alta carga de eventos e dados.

<img src="https://github.com/user-attachments/assets/65701460-5b34-4c05-a153-25d1b65525e8" align="right" height="377">

O **MQTT** é um protocolo de mensageria incrivelmente leve e simples, projetado especificamente para cenários onde a eficiência é crítica, como dispositivos IoT com recursos limitados, conexões de baixa largura de banda ou redes instáveis. Desenvolvido inicialmente pela IBM na década de 1990 para monitorar oleodutos via satélite, ele opera sobre TCP/IP e segue um modelo de publicação/assinatura extremamente elegante.

Sua arquitetura envolve três componentes principais: os **publicadores** que enviam mensagens, os **assinantes** que recebem mensagens de tópicos específicos, e o **broker** que atua como um corretor central, filtrando e distribuindo todas as mensagens. A beleza do MQTT está em sua simplicidade: os clientes não precisam saber uns dos outros, apenas se conectam ao broker e se comunicam através de tópicos hierárquicos como "casa/sala/temperatura". O protocolo oferece três níveis de qualidade de serviço que permitem equilibrar entre confiabilidade e overhead, desde o "fire and forget" até a confirmação de entrega completa, além de recursos importantes como a mensagem de última vontade que notifica outros clientes se um dispositivo se desconectar abruptamente.

Já o AMQP é um protocolo de camada de aplicação mais robusto e completo, projetado para ser um padrão aberto para sistemas de mensageria empresarial. Enquanto o MQTT é minimalista por design, o AMQP oferece um conjunto rico de recursos para cenários complexos de negócios. Sua arquitetura é mais sofisticada, baseada em um modelo de filas, exchanges e bindings que permitem roteamento flexível de mensagens através de diferentes padrões como publish/subscribe, ponto a ponto e request/reply.

As diferenças fundamentais entre eles começam com seus **objetivos de design**: MQTT foi criado para dispositivos embarcados e IoT, enquanto AMQP foi desenvolvido para sistemas empresariais como bancos e sistemas financeiros. Em termos de **modelo de mensageria**, MQTT usa publish/subscribe baseado em tópicos através de um broker central, enquanto AMQP oferece um modelo mais flexível com exchanges que roteiam mensagens para filas baseado em regras definidas por bindings. O **tamanho do cabeçalho** ilustra bem essa diferença filosófica - MQTT tem apenas 2 bytes de overhead por mensagem, enquanto AMQP tem overhead significativamente maior devido à sua riqueza de recursos.

Quando consideramos **confiabilidade e garantias de entrega**, MQTT oferece três níveis de QoS básicos, enquanto AMQP fornece garantias transacionais completas com confirmações e persistência robusta. Na **descoberta de serviços**, MQTT depende completamente do broker para roteamento baseado em tópicos, enquanto AMQP permite roteamento inteligente baseado em cabeçalhos de mensagem, parâmetros de rota e outras propriedades.

![518211933_1249050527010417_7374330936779393934_n](https://github.com/user-attachments/assets/84a867cc-18b9-4ed1-8b3b-6e8a3353338c)

Essas diferenças se traduzem em casos de uso bastante distintos. O MQTT brilha em aplicações IoT como sensores remotos, dispositivos vestíveis, automação residencial e telemetria de veículos, onde a simplicidade e eficiência são prioritárias. O AMQP é ideal para sistemas empresariais como integração de sistemas legados, processamento de transações financeiras, orquestração de serviços em microsserviços e sistemas onde o roteamento complexo e as garantias de entrega são essenciais.

A escolha entre eles não é questão de qual é melhor, mas qual é mais apropriado para o contexto específico. MQTT oferece a elegância da simplicidade para dispositivos com restrições, enquanto AMQP fornece o poder e a flexibilidade para sistemas empresariais complexos que exigem roteamento sofisticado e garantias robustas de entrega.

<table>
 <tr>
  <td><img height="177" src="https://github.com/user-attachments/assets/c1f16147-9329-4bac-9d8f-cf49c31d2927" /></td>
  <td><img height="177" src="https://github.com/user-attachments/assets/9b534d8b-d236-451f-a327-0be7b244cea3" /></td>
 </tr>
</table>

O padrão **Pub/Sub** é um paradigma de comunicação assíncrona onde os emissores de mensagens, chamados de **publicadores** (Pub - publishers), não enviam dados diretamente para receptores específicos. Em vez disso, eles categorizam as mensagens em **tópicos** (ou *channels*), sem sequer conhecer a identidade ou a quantidade dos possíveis receptores. Os receptores, por sua vez, chamados de **assinantes** (Sub - subscribes), expressam interesse em um ou mais tópicos e recebem apenas as mensagens que são relevantes para eles, sem precisar saber de qual publicador vieram. Esse desacoplamento total entre publicador e assinante — tanto no tempo (não precisam estar ativos simultaneamente) quanto no espaço (não precisam se conhecer) — é a principal virtude do padrão, tornando-o ideal para sistemas escaláveis, dinâmicos e distribuídos.

A aplicação do Pub/Sub no **MQTT** é a sua razão de ser original. O protocolo foi concebido em torno desse modelo. No MQTT, o coração do sistema é o **broker**, um servidor central que gere todos os tópicos. Um publicador envia uma mensagem para o broker, especificando um tópico com estrutura hierárquica, como `casa/sala/iluminacao`. Os assinantes, para receberem essas mensagens, enviam ao broker uma mensagem `SUBSCRIBE` informando o tópico de interesse (é possível usar o caractere curinga `#` para assinar uma hierarquia inteira). A partir desse momento, o broker atua como um serviço de correio inteligente: toda vez que uma mensagem for publicada naquele tópico, ele a encaminhará a todos os assinantes inscritos. A implementação é simples e direta: basta que os dispositivos se conectem ao broker usando uma biblioteca cliente MQTT e comecem a publicar ou assinar nos tópicos desejados. A leveza do protocolo faz com que essa operação seja extremamente eficiente, mesmo para milhares de dispositivos conectados.

A aplicação no **AMQP** é igualmente poderosa, mas segue uma lógica mais rica e flexível. O AMQP implementa o Pub/Sub através de um de seus componentes de roteamento: a **Exchange**. Especificamente, a **Fanout Exchange** e a **Topic Exchange** são os mecanismos clássicos para esse padrão. Na Fanout Exchange, a regra é simples: toda mensagem que chega é replicada e enviada para **todas as filas** que estiverem vinculadas a ela, sem qualquer filtro. É o Pub/Sub mais puro e amplo. Já a Topic Exchange oferece um controle mais refinado: as mensagens são roteadas para filas específicas com base em uma chave de roteamento e em padrões de correspondência definidos no vínculo (o *binding*). Por exemplo, uma fila pode se vincular a uma exchange usando a chave `sensor.temperatura.*` e receberá todas as mensagens cuja chave de roteamento combine com esse padrão, como `sensor.temperatura.cozinha` e `sensor.temperatura.quarto`. Para aplicar o Pub/Sub no AMQP, o publicador envia a mensagem para uma Exchange do tipo Fanout ou Topic. Os assinantes, por sua vez, criam suas próprias filas (geralmente exclusivas e temporárias) e as vinculam a essa Exchange, com a chave de roteamento desejada. O broker (como o RabbitMQ) então se encarrega do roteamento inteligente.

A diferença fundamental na aplicação prática está na **filosofia de uso**. O MQTT, com seus tópicos hierárquicos e broker centralizado, é incrivelmente simples e intuitivo para cenários de IoT e telemetria, onde o foco é a disseminação eficiente de dados. O AMQP, com seu modelo baseado em Exchanges e Filas, oferece um controle muito mais granular sobre o fluxo de mensagens, permitindo padrões complexos de roteamento, persistência e garantias de entrega que são essenciais em sistemas empresariais. Em resumo, enquanto o MQTT oferece um "sistema de tópicos" pronto para uso, o AMQP fornece os "tijolos de construção" para que você mesmo monte seu próprio sistema de Pub/Sub com o nível de sofisticação exigido pela aplicação.

**Space-based** architecture é um estilo arquitetural voltado principalmente para aplicações altamente escaláveis e resilientes, especialmente aquelas que enfrentam cargas de trabalho imprevisíveis ou picos de acesso intensos. A ideia central do modelo space-based é eliminar gargalos comuns de acesso e processamento centralizado — como ocorre em bancos de dados relacionais tradicionais — distribuindo o estado da aplicação em memória através de múltiplos nós (clusters) que compartilham um "espaço de dados" (data grid), de onde vem o termo "space". Essa abordagem busca minimizar a contenção por recursos compartilhados, permitindo que os nós operem de forma mais autônoma, mantendo o estado da aplicação localmente, replicando-o conforme necessário.

No space-based, a aplicação é dividida em unidades chamadas de “processing units” (unidades de processamento), cada uma contendo a lógica de negócio, dados relevantes e, às vezes, o mecanismo de persistência local. Essas unidades são implantadas de forma redundante em diferentes servidores, e o sistema gerencia automaticamente o balanceamento de carga e a tolerância a falhas. Os dados e as tarefas de processamento são mantidos em um espaço distribuído em memória, como um cache altamente disponível, evitando assim o uso intensivo de banco de dados em tempo real. Isso é especialmente eficaz em sistemas como e-commerces durante Black Friday, sistemas bancários com transações simultâneas, ou qualquer cenário com grande volume de leitura e escrita concorrente.

Essa arquitetura é inspirada no conceito de tuple space (espaço de tuplas), popularizado pelo modelo Linda de programação paralela, onde elementos podem ser inseridos, buscados ou removidos de um espaço compartilhado, de forma assíncrona e desacoplada. Ao utilizar esse espaço como uma camada de abstração entre os componentes do sistema, o space-based promove o desacoplamento, a escalabilidade horizontal e a alta disponibilidade. A persistência eventual em bancos de dados pode ser usada para backup ou consistência de longo prazo, mas não interfere no desempenho em tempo real.

Em suma, space-based architecture é uma abordagem orientada à memória, com foco em escalabilidade e resiliência, onde os dados e processos circulam por um espaço distribuído e compartilhado entre os nós da aplicação. Ela é ideal para aplicações que não podem depender de uma única fonte de verdade centralizada e precisam operar sob alta concorrência e baixa latência.

**Rule-based**, ou sistema baseado em regras, é uma abordagem na qual o comportamento de um sistema é determinado por um conjunto explícito de regras lógicas e condicionais, geralmente escritas na forma de “se... então...” (if... then...). Esse tipo de sistema atua avaliando constantemente as regras definidas em sua base de conhecimento para tomar decisões, executar ações ou inferir novos dados a partir de informações fornecidas como entrada. É um paradigma fortemente utilizado em inteligência artificial simbólica, sistemas especialistas, motores de decisão e automações de negócios. Em vez de escrever um fluxo rígido de controle de programação, o desenvolvedor ou especialista define um conjunto de condições e consequências, e o motor de regras se encarrega de aplicar essas instruções de acordo com os dados e o contexto.

O grande diferencial de sistemas rule-based é a sua flexibilidade e facilidade de modificação. Como o comportamento é guiado por regras separadas da lógica de aplicação principal, é possível adaptar e expandir o sistema alterando ou adicionando novas regras, sem a necessidade de reescrever o código central. Essa característica os torna úteis em domínios onde o conhecimento muda com frequência ou onde especialistas não técnicos precisam alterar a lógica, como em sistemas jurídicos, financeiros, diagnósticos médicos ou motores de recomendação. Motores como Drools, no ecossistema Java, são exemplos típicos de implementação desse conceito, permitindo que o sistema reaja dinamicamente às entradas conforme as regras são disparadas.

No entanto, sistemas baseados em regras também apresentam desafios, principalmente à medida que a complexidade aumenta. Quando há muitas regras interdependentes, pode se tornar difícil prever os efeitos colaterais de uma nova regra ou compreender completamente o comportamento do sistema. Além disso, sistemas rule-based não lidam bem com incerteza ou ambiguidade, como modelos probabilísticos fariam. Mesmo assim, sua transparência e explicabilidade os tornam ideais para contextos em que decisões precisam ser justificáveis e auditáveis. Portanto, rule-based é uma abordagem lógica e determinística, onde o conhecimento do domínio é traduzido em regras explícitas e aplicadas sistematicamente para produzir decisões, diagnósticos ou ações.

Evolução da Arquitetura da API da Netflix: A arquitetura da API da Netflix passou por 4 estágios principais:

- Monolith
- Direct access
- Gateway aggregation layer
- Federated gateway

![FB_IMG_1722531344115](https://github.com/user-attachments/assets/d2ea7a2a-93a2-4fc0-a032-e6f13c302c0b)
![FB_IMG_1722461479416](https://github.com/user-attachments/assets/e5e8b6fe-9a02-483e-b210-8750cffba180)
![FB_IMG_1722096754127](https://github.com/user-attachments/assets/fd5e6c9b-f1fe-4519-9e80-a07810d8ea8e)
![FB_IMG_1721753552315](https://github.com/user-attachments/assets/ae5f9263-a440-4cc5-9e1a-159ac125c398)
![FB_IMG_1721753534122](https://github.com/user-attachments/assets/d72c5509-4909-4fa7-84c4-110914b82030)

## [Microservices] Sistemas reativos
<img src="https://img.shields.io/badge/Spring_Boot-3.10.7-gold?style=flat&logo=Spring&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-gold?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/RabbitMQ-16.17.0-gold?style=flat&logo=RabbitMQ&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-16.17.0-gold?style=flat&logo=PostgreSQL&logoColor=white"> <img src="https://img.shields.io/badge/MongoDB-16.17.0-gold?style=flat&logo=MongoDB&logoColor=white"> <img src="https://img.shields.io/badge/Docker-16.17.0-gold?style=flat&logo=Docker&logoColor=white">

<img height="77" align="right" src="https://github.com/user-attachments/assets/b0a85aed-004e-41d8-aad6-8cd4919b2b77" />

Com cada vez mais conexões, mais dados e usuários mais exigentes, manter a responsividade de um sistema de microsserviços tem se tornado uma tarefa dolorosa. Por sorte, isso não precisa ser assim. É para amenizar essa dor que existem os *sistemas reativos*. Sistemas criados como reativos são muito mais flexíveis, desacoplados e escaláveis, o que os torna mais fáceis para desenvolver e mais abertos a mudanças. 

Os **sistemas reativos** são um design de software, eles são projetados para serem mais responsivos, resilientes, elásticos e orientados por mensagens. Esse paradigma de design é especialmente relevante para sistemas distribuídos e modernos, onde a escalabilidade e a capacidade de lidar com falhas são cruciais. O contexto descrito está relacionado ao paradigma de programação reativa. Estamos destacando os desafios de manter a responsividade e a eficiência em sistemas de microsserviços diante do aumento de conexões, volume de dados e demandas dos usuários, e apresenta os sistemas reativos como uma solução para esses problemas.

A **programação reativa** é um estilo de design de software que foca em responder a eventos de forma assíncrona e não bloqueante. No caso de sistemas distribuídos e modernos, como os de microsserviços, a programação reativa é extremamente útil.

> [!Warning]
> Programação reativa e sistemas reativos não denotam a mesma coisa, embora muita gente use como se fossem sinônimos — e é exatamente aí que nasce a confusão. A relação entre os dois é de meio e fim, não de equivalência. Programação reativa pode ajudar a construir sistemas reativos, mas não garante que você terá um sistema reativo. Dá perfeitamente para ter código reativo rodando dentro de um monólito frágil, acoplado, que cai inteiro se um serviço externo falhar. E também é possível ter um sistema reativo bem arquitetado usando técnicas assíncronas que não seguem estritamente bibliotecas de programação reativa.

As organizações que trabalham em diferentes ramos estão independentemente descobrindo padrões para criar sistemas semelhantes. Esses sistemas são mais robustos, mais resilientes, mais flexíveis e melhor posicionados para sustentar as demandas modernas.

Essas transformações estão acontecendo porque os requisitos de sistemas mudaram drasticamente nos últimos anos. Há apenas alguns anos, uma grande aplicação tinha dezenas de servidores, tempo de resposta na casa dos segundos, horas de indisponibilidade para manutenção e gigabytes de dados. Aplicações atuais são entregues em todos os lugares, desde aplicativos móveis até aplicações na nuvem com clusters rodando milhares de processadores multi-core. Geralmente os usuários esperam respostas em milissegundos e 100% de disponibilidade. Dados são mensurados em petabytes. As demandas de hoje simplesmente não são mais atendidas pelas arquiteturas do passado.

Nós acreditamos que é preciso haver uma abordagem consistente para arquitetura de sistemas, e acreditamos que todos os aspectos necessários já são reconhecidos individualmente: nós queremos sistemas Responsivos, Resilientes, Elásticos e Orientados a Mensagens. Nós chamamos isso de <a href="https://www.reactiveprinciples.org/index.html">Sistemas Reativos</a>.

Sistemas criados como Reativos são muito mais flexíveis, desacoplados e escaláveis. Isso os torna mais fáceis para desenvolver e mais abertos a mudanças. São significativamente mais tolerantes a falhas e quando elas ocorrem são tratadas com elegância ao invés de desastre. Sistemas Reativos são altamente responsivos, dando aos usuários um efetivo feedback interativo.

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/d1e1a2cf-323a-444f-817d-f01edd890686" align="right" height="177">

> [!Important]
> No livro <a href="https://www.casadocodigo.com.br/products/livro-sistemas-reativos">Sistemas reativos: Não confundir com sistemas radioativos</a>, Guilherme Moraes aborda a aplicação da perspectiva reativa no desenvolvimento para garantir que seus sistemas sejam mais resilientes, elásticos e responsivos. Você passará por conceitos complexos da Arquitetura de Software e sistemas distribuídos, mas em uma aprendizagem envolvente com doses cavalares de humor e descontração, estabelecendo relações práticas com muito do que você já faz em seu dia a dia. E, meio sem perceber, você ampliará sua perspectiva sobre software e nunca mais reagirá da mesma maneira ao escutar a seguinte pergunta: "A gente já chegou?".

Sistemas Reativos são:

<div align="center"><img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/280a334e-ea32-428e-af93-9171f9d5217d" height="277"></div><br />

- **Responsivos**: O sistema responde em um tempo razoável, se possível. Responsividade é a pedra fundamental da usabilidade e da utilidade, mas, mais do que isso, responsividade significa que problemas podem ser detectados rapidamente e tratados com a máxima eficácia. Sistemas responsivos têm como objetivo prover tempos de resposta curtos e consistentes, estabelecendo margens de tolerância confiáveis que garantem uma qualidade de serviço consistente. Esse comportamento consistente, por sua vez, simplifica tratamentos de erro, reforça a confiança do usuário final e incentiva interações futuras.

- **Resilientes**: O sistema continua responsivo em caso de falha. Isso aplica-se não apenas para sistemas de alta disponibilidade e missão crítica  qualquer sistema que não é resiliente ficará indisponível após uma falha. Resiliência é obtida por meio de replicação, contenção, isolamento e delegação. Falhas são contidas dentro de cada componente, isolando-os uns dos outros e, portanto, garantindo que partes do sistema podem falhar e se recuperar sem comprometer o sistema como um todo. A recuperação de cada componente é delegada a outro componente (externo) e alta disponibilidade é garantida por replicação, quando necessária. Os clientes de cada componente não são sobrecarregados com a responsabilidade do tratamento de falhas.

<img src="https://github.com/user-attachments/assets/62b63ffa-8db1-4620-9442-2d589e95147b" align="right" height="177">

- **Elásticos**: O sistema continua responsivo mesmo sob variações de carga de demanda. Sistemas Reativos podem reagir a mudanças na taxa de solicitações por meio do aumento ou diminuição dos recursos alocados para lidar com essas entradas. Isso requer uma arquitetura que não tenha pontos de contenção ou gargalos, o que permite dividir ou replicar componentes e distribuir a demanda entre eles. Sistemas Reativos suportam algoritmos de escalonagem preditivos e Reativos porque geram métricas de desempenho relevantes e em tempo real. Assim, conseguem elasticidade com baixo custo em hardware e plataformas de software padrões.

- **Orientados a Mensagens**: Sistemas Reativos baseiam-se em transferência de mensagens assíncronas para estabelecer fronteiras entre os componentes e garantir baixo acoplamento, isolamento, transparência na localização. Essas fronteiras também provêem meios para delegar o tratamento de erros na forma de mensagens. Utilizar explicitamente a transferência de mensagens permite o gerenciamento de carga, elasticidade e controle de fluxo, por meio da modelagem e monitoramento das filas no sistema e aplicação de contrapressão quando necessária. Roteamento de mensagens com transparência na localização como o meio de comunicação torna possível o gerenciamento de falhas da mesma maneira seja em um cluster ou em um único host. Comunicação não bloqueante permite que os destinatários consumam recursos apenas enquanto estão ativos, o que leva a uma menor sobrecarga no sistema.

<img src="https://github.com/user-attachments/assets/bdc78ab5-276b-452f-ae88-f937dfc84960" align="right" height="177">

Grandes sistemas são compostos por sistemas menores e, portanto, dependem das propriedades Reativas de seus componentes. Isso significa que Sistemas Reativos aplicam princípios arquiteturais que fazem com que essas propriedades sejam utilizadas em todos os níveis da escala, de modo que os componentes sejam combináveis entre si. Os maiores sistemas do mundo são construídos sobre arquiteturas que baseiam-se nessas propriedades e servem as necessidades de bilhões de pessoas diariamente. Está na hora de aplicar esses princípios conscientemente do início ao invés de redescobrí-los todas as vezes que implementamos um novo sistema.

## [Microservices] AG - API Gateway
<a href=""><img src="https://img.shields.io/badge/Kong-24.0.1-003459?style=flat&logo=Kong&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Nginx-24.0.1-limegreen?style=flat&logo=Nginx&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Terraform-24.0.1-844FBA?style=flat&logo=Terraform&logoColor=white"></a> <a href="https://ngrok.com/docs/universal-gateway/examples/microservices-gateway?utm_campaign=september_2025_newsletter_content_a&utm_medium=newsletter&_hsenc=p2ANqtz-8WI06tvfCxMZimoOpNdlTDF3plxzsopr8WcnqMdKL16obTxSLnCVtUcT8AtzopCEiAC30cf9XxtiZ3gHj--Hwxhj08TR7_n0COA3XGLtE5Am4BKO0&_hsmi=381970286&utm_content=homepage&utm_source=email
"><img src="https://img.shields.io/badge/Docker-24.0.1-2496ED?style=flat&logo=Docker&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Istio-24.0.1-2496ED?style=flat&logo=Istio&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Amazon_Web_Services-AGW-FF4F8B?style=flat&logo=amazonapigateway&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/.NET-Ocelot-indigo?style=flat&logo=.NET&logoColor=white"></a>

<a href="https://youtu.be/Uu32ggF-DWg"><img src="https://github.com/user-attachments/assets/8a11f9f6-3095-46f5-bdf0-0541bcf5119a" height="77" align="right"></a>

Um **API Gateway** é um componente essencial em arquiteturas modernas, especialmente em sistemas baseados em microserviços. Ele atua como um intermediário entre clientes e um conjunto de serviços backend, gerenciando todas as solicitações que entram no sistema. Sua principal função é receber, rotear, transformar e controlar as solicitações de API, além de retornar respostas apropriadas aos clientes.

Você está cansado de gerenciar vários pontos de entrada para seus microsserviços? O padrão API Gateway está aqui para salvar o dia! Atuando como um único ponto de entrada para todas as solicitações do cliente, o API Gateway simplifica o acesso aos seus microsserviços, oferecendo comunicação perfeita entre clientes e serviços.

Gateways de API são componentes essenciais em arquiteturas de software modernas, especialmente em sistemas baseados em microsserviços. Padrão de API gateway: seu balcão único para microsserviços.

Eles atuam como um único ponto de entrada para todas as requisições de API, fornecendo uma interface unificada para acessar diversos serviços e dados. Ao desacoplar aplicações clientes dos microserviços backend, os API Gateways simplificam o gerenciamento de APIs e melhoram o desempenho geral e a segurança do sistema.

Gateways de API ajudam a aprimorar a experiência do desenvolvedor enquanto constroem sistemas escaláveis e manuteníveis. As organizações podem alcançar melhor controle sobre seu cenário de APIs utilizando APIs Gateways.

À medida que a complexidade dos sistemas de software continua a crescer, os Gateways de API desempenharão um papel cada vez mais importante ao possibilitar uma comunicação e integração eficazes entre serviços e clientes.

Vamos falar sobre Padrões de Design da arquitetura de Microsserviços, que é o padrão de **Agregação de Gateway** (Gateway Aggregation Pattern). Como você sabe, aprendemos práticas e padrões e os adicionamos à nossa caixa de ferramentas de design. E usaremos esses padrões e práticas ao projetar a arquitetura de microsserviços.

Em sistemas distribuídos, sem um API Gateway, os clientes teriam que se comunicar diretamente com cada microserviço, o que aumentaria a complexidade, exigiria lógica adicional para lidar com autenticação, balanceamento de carga e agregação de dados, além de expor os serviços internos diretamente à internet. O API Gateway resolve esses problemas centralizando essas responsabilidades.

Você precisa aprender onde e quando aplicar o padrão de agregação de gateway na arquitetura de microsserviços com o design de um sistema de aplicativos de comércio eletrônico com os seguintes princípios KISS, YAGNI, SoC e SOLID.

O API Gateway é um servidor que lida com muitas funcionalidades em um único local para os clientes interagirem. Ele também funciona como um proxy reverso entre seus aplicativos cliente e a arquitetura de microsserviços de back-end.

O padrão de agregação de gateway é semelhante ao roteamento de gateway, mas além disso, oferece agregação de serviços. Basicamente, o padrão de agregação de gateway oferece o uso de um serviço de gateway que fornece para agregar várias solicitações internas a microsserviços internos com a exposição de uma única solicitação ao cliente.

Por que você deve se preocupar com o API Gateway? Primeiro, ajuda a agregar respostas de vários microsserviços, reduzindo o número de viagens de ida e volta entre clientes e serviços. Isso resulta em melhor desempenho e experiência do usuário. Em segundo lugar, ele permite que você implemente preocupações transversais, como autenticação, registro e limitação de taxa em um único local, promovendo consistência e reduzindo a redundância.

Imagine a conveniência de ter um hub central que cuida de todas essas responsabilidades! De acordo com um estudo da RapidAPI, 68% dos desenvolvedores que adotaram o API Gateway relataram segurança aprimorada e gerenciamento simplificado de seus microsserviços.

Algumas soluções populares do API Gateway incluem Amazon API Gateway, Kong e Azure API Management. Essas ferramentas fornecem uma variedade de recursos, como cache, limitação e monitoramento, para ajudá-lo a gerenciar seus microsserviços com eficiência.

O diagrama abaixo mostra os detalhes:

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/e37ee7bf-898b-4330-8c19-6e64e2a68278"></td>
		<td><img src="https://github.com/user-attachments/assets/87fefd9b-435b-48c8-a89d-eac83e7bd959"></td>
		<td><img src="https://github.com/user-attachments/assets/62bebf76-1aca-4dd9-b71a-3e33adaa4e7d"></td>
	</tr>
</table>

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/86d63816-3755-4a13-845d-24218313551c"></td>
		<td><img src="https://github.com/user-attachments/assets/9f70ea59-cd9f-4c93-af85-1738b9009a83"></td>
		<td><img src="https://github.com/user-attachments/assets/a153616b-7058-40f7-8514-f7422708c78c"></td>
		<td><img src="https://github.com/user-attachments/assets/ebf0d996-77fa-426a-9095-2692d92050a2"></td>
		<td><img src="https://github.com/user-attachments/assets/4b929edf-c4a7-4393-92d7-108b8556d1f5"></td>
	</tr>
</table>

- Passo 1 - O cliente envia uma requisição HTTP para o gateway da API.

- Passo 2 - O gateway da API analisa e valida os atributos na requisição HTTP.

- Passo 3 - O gateway API realiza verificações de lista de permissões/listas de recusas.

- Passo 4 - O gateway da API se comunica com um provedor de identidade para autenticação e autorização.

- Passo 5 - As regras de limite de taxa são aplicadas ao pedido. Se o valor estiver acima do limite, o pedido é rejeitado.

- Passos 6 e 7 - Agora que a solicitação passou pelas verificações básicas, o gateway da API encontra o serviço relevante para encaminhar por meio de correspondência de caminhos.

- Passo 8 - O gateway da API transforma a solicitação no protocolo apropriado e a envia para microserviços de backend.

- Passos 9-12: O gateway API pode lidar com erros corretamente e lida com falhas se o erro demorar mais para ser recuperado (quebra de circuito). Também pode aproveitar a pilha ELK (Elastic-Logstash-Kibana) para registro e monitoramento. Às vezes armazenamos dados em cache no gateway da API.

Esse padrão deve ser usado se o aplicativo cliente tiver que invocar vários microsserviços de back-end diferentes para executar sua lógica. Vamos olhar para a imagem:

<table>
	<tr>
		<td><a href="https://medium.com/design-microservices-architecture-with-patterns/microservices-architecture-for-enterprise-large-scaled-application-825436c9a78a"><img height="377" src="https://github.com/user-attachments/assets/6049c51f-5d11-46cd-bb90-ae1e2e6aea27" /></a></td>
		<td><img height="377" src="https://github.com/user-attachments/assets/aa05f06e-1b18-4f1c-b16f-9515f356a74b" /></td>
	</tr>
</table>

Se não pudermos colocar a caixa de agregação aqui, o cliente envia solicitações para cada serviço. Cada serviço processa a solicitação e envia a resposta de volta ao aplicativo (2,3,4,5,6).

Portanto, isso causará problemas de rede e latência. E não é bom gerenciar serviços de acesso direto do cliente e não é bom invocar a responsabilidade de serviço para o cliente.

Para resolver esses problemas, podemos usar um gateway para reduzir a conversa entre o cliente e os microsserviços internos. O gateway recebe solicitações de clientes e envia solicitações para os vários serviços de back-end e, em seguida, agrega os resultados e os envia de volta ao cliente solicitante.

Esse padrão pode reduzir o número de solicitações que o aplicativo faz aos serviços de back-end e melhorar o desempenho do aplicativo em redes de alta latência.

Veja a imagem 2 que a comunicação da interface do usuário e da MS é direta e parece difícil gerenciar as comunicações. Agora devemos nos concentrar nas comunicações de microsserviços com a aplicação do padrão API GW e a evolução dessas arquiteturas passo a passo.

Pode haver vários clientes que chamam as APIs do servidor, e o API Gateway é o componente que roteia solicitações para o microsserviço relevante e, em seguida, obtém a resposta e a envia ao cliente. Ele lida com todos os recursos transversais, como segurança, registro, cache, etc., em um único lugar, em vez de implementarmos essas funcionalidades em todos os microsserviços. Além disso, ele pode consolidar e agregar os dados na agregação de vários microsserviços usando um único endpoint para os clientes se comunicarem.

Antes da evolução da arquitetura de microsserviços, a maioria dos sistemas usava um padrão Monolith e podíamos até lidar com as preocupações transversais em um ou dois servidores. Mas com microsserviços, não podemos nos dar ao luxo de lidar com preocupações transversais em cada um dos microsserviços, o que tornará as coisas mais lentas com um volume de memória maior, degradando o desempenho do sistema.

As principais funcionalidades de um API Gateway incluem:

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/4e8e1f10-ad97-4b15-b570-36eeee8967ac"></td>
		<td><img src="https://github.com/user-attachments/assets/be3e0ab6-fd21-4d5a-9a52-03b094a1d828" /></td>
	</tr>
</table>

1. **Roteamento de solicitações**: Ele direciona solicitações para o serviço backend apropriado com base no caminho, método HTTP ou outros critérios.
   
2. **Autenticação e autorização**: Pode validar tokens de acesso, certificados ou outras credenciais antes de encaminhar solicitações aos serviços backend.

3. **Transformação de dados**: Permite manipular solicitações e respostas, como converter formatos (JSON para XML, por exemplo) ou adicionar/remover campos.

4. **Agregação de respostas**: Para solicitações que requerem dados de múltiplos serviços, o API Gateway pode consolidar essas respostas antes de retornar ao cliente.

5. **Limitação de taxa e controle de acesso**: Garante que o sistema não seja sobrecarregado, implementando políticas de limite de solicitações por usuário ou IP.

6. **Monitoramento e métricas**: Coleta dados de uso e desempenho para fornecer insights sobre o funcionamento das APIs.

7. **Segurança e proteção**: Oferece proteção contra ataques comuns, como DDoS e injeções maliciosas, ao atuar como uma camada de firewall para APIs.

Um exemplo prático é em uma aplicação de e-commerce: o API Gateway pode expor uma única API para os clientes acessarem, enquanto internamente roteia solicitações para microserviços como autenticação, catálogo de produtos, carrinho de compras e pagamentos.

Ferramentas populares para implementação de API Gateways incluem **Kong**, **NGINX**, **AWS API Gateway**, **Apigee**, **Traefik** e **Istio** (quando usado em conjunto com service meshes). Em resumo, o API Gateway é uma peça fundamental para simplificar a gestão, aumentar a segurança e otimizar a performance de APIs em arquiteturas modernas.

Vamos aprender a projetar a arquitetura de microsserviços usando padrões de design, princípios e as melhores práticas. Começaremos projetando microsserviços monolíticos a orientados a eventos passo a passo e juntos, usando os padrões e técnicas de design de arquitetura corretos. Você pode optar por mensageria, cache, balanceamento de carga, juntamente com arquiteturas de software como modulares, tudo isso pode ser customizável de acordo com a complexidade do seu sistema, verifique com atenção os requisitos e a complexidade.

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/b8353aaa-159e-49b7-a479-0590ed21b6fd"></td>
		<td><img src="https://github.com/user-attachments/assets/525e8f5b-cf1b-4b50-8c53-ea7a3ca95dca"></td>
	</tr>
</table>

Em resumo, o padrão API Gateway é um componente essencial de uma arquitetura de microsserviços bem-sucedida. Ao adotar esse padrão, você pode garantir comunicação simplificada, segurança aprimorada e gerenciamento simplificado de seus serviços. Você está pronto para desbloquear o verdadeiro potencial dos microsserviços com o padrão API Gateway? Bora pro código!

Os sistemas de software modernos raramente vivem isolados. A maioria dos aplicativos hoje é costurada a partir de dezenas, às vezes centenas, de serviços implantados de forma independente, cada um lidando com uma peça do quebra-cabeça. Isso ajuda a criar unidades menores de responsabilidade e acoplamento flexível. No entanto, a flexibilidade vem com um novo tipo de complexidade, especialmente em torno de como esses serviços se comunicam.

Em um monólito, a função em processo chama os componentes de costura. Em um mundo baseado em serviços, tudo fala pela rede. De repente, as preocupações que antes eram tratadas dentro do aplicativo, como novas tentativas, autenticação, limitação de taxa, criptografia e observabilidade, tornam-se preocupações distribuídas. E as preocupações distribuídas são mais difíceis de acertar.

Para gerenciar essa complexidade, as equipes de engenharia normalmente usam um dos dois padrões: o gateway de API ou o service mesh.

Ambos visam tornar a comunicação entre serviços mais gerenciável, segura e observável. Mas eles fazem isso de maneiras muito diferentes e por razões diferentes. A confusão geralmente começa quando essas ferramentas são tratadas como intercambiáveis ou quando suas funções são reduzidas a uma simples direção de tráfego: "Os gateways de API são para tráfego norte-sul, as malhas de serviço são para leste-oeste". Esse atalho simplifica demais ambos e prepara as equipes para uso indevido ou sobrecarga desnecessária.

Analisamos os gateways de API e o Service Mesh em detalhes, juntamente com suas principais diferenças e metas de uso:

![unnamed](https://github.com/user-attachments/assets/d793f585-620c-432a-a105-826a1c2c6538)

Observe o diagrama abaixo: Essa imagem representa uma **arquitetura de microsserviços com API Gateway** um padrão bastante comum em sistemas distribuídos modernos, especialmente em plataformas de mobilidade (como Uber, 99, ou Lyft). Tecnicamente, o tipo exato é conhecido como **API Gateway Pattern** dentro do estilo **Service-Oriented Microservices Architecture**.

<img width="815" height="832" alt="6c506745-529e-483f-942a-f95b4deca71b" src="https://github.com/user-attachments/assets/e39f07af-a647-45a2-8082-ff5cec4f6a30" />

Veja a análise completa:

- Cada **módulo hexagonal verde** (Passenger Management, Driver Management, Trip Management, Billing, Payments, Notification) é um **microsserviço independente**, com sua própria **REST API**, banco de dados e domínio funcional.
- O **API Gateway** centraliza o acesso externo — ou seja, o app móvel e as interfaces web não se conectam diretamente a cada serviço, mas sim ao gateway, que roteia requisições, aplica autenticação, logging, rate limiting, etc.
- Os **adapters externos** (Stripe Adapter, Twilio Adapter, SendGrid Adapter) mostram **integrações com serviços externos**, aqui o padrão de integração é o **adapter pattern**, acoplado a serviços de pagamento, SMS e e-mail.
- Essa topologia também sugere o uso de **Service Mesh** (como Istio ou Linkerd), já que há comunicação cruzada direta entre microsserviços (REST API interna).

Conceitualmente, isso é uma **arquitetura de microsserviços com gateway unificado e comunicação síncrona via REST**, uma variação moderna do **Backend for Frontend (BFF)** quando há múltiplos front-ends (Passenger Web UI, Driver Web UI, Mobile App).

Se você fosse nomear essa arquitetura tecnicamente em um documento de design ou currículo, a forma mais correta seria:

> **Arquitetura de Microsserviços com API Gateway Pattern e integração externa via Adapters (REST-based Service Mesh).**

Em termos práticos, é uma arquitetura distribuída e escalável, com alta coesão entre domínios (DDD) e baixo acoplamento entre serviços.

Essa arquitetura pode (e quase sempre deve) envolver **Service Discovery**, mesmo que isso não esteja explícito no diagrama. Explicando tecnicamente: o **Service Discovery** (como o que o Netflix OSS, Consul ou Eureka implementam) é um componente fundamental em sistemas de **microsserviços dinâmicos**, porque cada serviço pode estar em múltiplas instâncias, distribuídas em diferentes hosts, containers ou pods (em Kubernetes, por exemplo).

No diagrama, o *API Gateway* funciona como ponto de entrada, mas para conseguir rotear requisições corretamente, ele precisa saber onde cada serviço está rodando. É aí que entra o **Service Discovery**: ele mantém um **catálogo de endpoints ativos** e suas localizações (geralmente em formato de registros DNS dinâmicos ou endpoints HTTP).

A relação entre os dois é a seguinte:
- O **API Gateway** consulta o **Service Discovery** para saber onde estão os microsserviços que ele precisa chamar.
- Os **microsserviços** registram-se automaticamente no **Service Discovery** quando sobem (registro dinâmico) e removem-se quando caem (deregistro).
- Outros microsserviços também consultam o **Service Discovery** quando precisam se comunicar entre si.

Na prática, se o diagrama fosse expandido, veríamos o **Service Discovery** (como Consul, Eureka, etc.) entre o Gateway e os serviços, gerenciando o roteamento interno. Essa arquitetura não é apenas **API Gateway Pattern**, mas uma **arquitetura de microsserviços com API Gateway e Service Discovery** — o que a torna altamente resiliente e escalável.

Se fosse descrever com rigor de senior:

> “Essa arquitetura implementa um modelo de microsserviços com API Gateway, comunicação síncrona via REST e resolução dinâmica de endpoints por meio de Service Discovery, garantindo balanceamento, disponibilidade e desacoplamento entre serviços.”

https://medium.com/tinder/how-we-built-the-tinder-api-gateway-831c6ca5ceca

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/0eeee857-d322-458d-8702-89de320bcf35"></td>
		<td><img src="https://github.com/user-attachments/assets/2f7c18d7-b68a-4fed-870a-68b0bea3109a"></td>
	</tr>
</table>

How Tinder’s API Gateway Handles A Billion Swipes Per Day:

> [!Warning]
> Aviso: Os detalhes deste post foram derivados dos artigos compartilhados online pela equipe de engenharia do Tinder. Todo o crédito pelos detalhes técnicos vai para a equipe de engenharia do Tinder. Os links para os artigos e fontes originais estão presentes na seção de referências ao final do post. Tentamos analisar os detalhes e dar nossa opinião sobre eles. Se você encontrar alguma imprecisão ou omissão, por favor, deixe um comentário e faremos o possível para corrigi-las.

Gateways de API estão na linha de frente de qualquer aplicação em grande escala. Eles expõem os serviços ao mundo externo, garantem segurança e moldam como os clientes interagem com o backend. A maioria das equipes começa com soluções prontas para uso como AWS API Gateway, Apigee ou Kong. E para muitos casos de uso, essas ferramentas funcionam bem, mas em alguns momentos podem não ser suficientes.

O Tinder chegou a esse ponto por volta de 2020.

Ao longo dos anos, o Tinder cresceu para mais de 500 microserviços. Esses serviços se comunicam internamente via malha de serviços, mas APIs voltadas para o exterior, que lidam com tudo, desde recomendações até correspondências e pagamentos, precisavam de um ponto de entrada unificado, seguro e amigável para desenvolvedores. Gateways prontos a oferecer poder, mas não precisão. Eles impuseram restrições à configuração, introduziram complexidade na implantação e careciam de integração profunda com a pilha de nuvem do Tinder.

Também havia um problema de velocidade. Equipes de produto enviam atualizações frequentes para serviços backend e clientes móveis. O portal precisava acompanhar. Cada atraso na exposição de uma nova rota ou comportamento de ajuste na borda retardava a entrega de recursos.

Depois veio a preocupação maior: a segurança. O Tinder opera globalmente. Tráfego real de usuários chega de mais de 190 países. O mesmo vale para o tráfego ruim, incluindo bots, scrapers e tentativas de abuso. O portal se tornou um ponto crítico de estrangulamento. Ele precisava impor controles rigorosos, detectar anomalias e aplicar filtros protetores sem desacelerar o tráfego legítimo.

A equipe de engenharia precisava de mais do que um gateway de API. Era necessário um framework que pudesse escalar com a organização, integrar profundamente com ferramentas internas e permitir que as equipes avançassem rápido sem comprometer a segurança.

Foi aqui que nasceu o TAG (Tinder API Gateway).

Desafios antes do TAG: Antes do TAG, a lógica do gateway no Tinder era um mosaico de soluções de terceiros. Diferentes equipes de aplicação adotaram diferentes produtos de gateway de API, cada um com sua própria pilha tecnológica, modelo operacional e limitações. O que funcionava bem para um time virou um gargalo para outro.

Essa configuração fragmentada introduziu atrito real:

- Stacks tecnológicos incompatíveis dificultavam o compartilhamento de código ou configuração.
- Componentes reutilizáveis não podiam se propagar entre equipes, levando à duplicação e desvio.
- O comportamento do gerenciamento de sessões variava entre gateways, criando bugs sutis e experiências de usuário inconsistentes.
- A sobrecarga operacional aumentou. Cada portal tinha suas peculiaridades, ciclo de atualização e custo de manutenção.
- A velocidade de implantação diminuiu. As equipes passaram mais tempo aprendendo, depurando e contornando limitações do gateway do que enviando recursos.

Aqui está um vislumbre da complexidade do gerenciamento de sessões entre APIs no Tinder antes do TAG.

<img width="1100" height="559" alt="image" src="https://github.com/user-attachments/assets/9e5aa464-e976-4bd5-b784-2866efa60e9e" />

Ao mesmo tempo, recursos centrais simplesmente estavam ausentes ou difíceis de implementar em gateways existentes. Alguns exemplos foram os seguintes:

Não há uma maneira limpa de criar gateways por aplicação que pudessem escalar de forma independente.

Suporte limitado para fluxos de trabalho nativos do Kubernetes, que o Tinder já havia adotado em outros lugares.

Os formatos de configuração eram pesados ou inflexíveis, retardando as equipes que tentavam expor ou modificar rotas.

Construir middleware personalizado, como filtros para detecção de bots ou aplicação de esquema de requisições, era ou sem suporte ou difícil de manter.

Transformar pedidos e respostas na borda exigia escrever boilerplate ou adotar plugins frágeis.

Esses não eram casos extremos. Eram necessidades diárias em um produto de rápida escala global.

A necessidade era clara: uma estrutura interna única que permitisse a qualquer equipe do Tinder construir e operar um gateway de API seguro e de alto desempenho com atritos mínimos.

Limitações das Soluções Existentes: Antes de construir o TAG, a equipe avaliou várias soluções populares de gateway de API, incluindo AWS API Gateway, Apigee, Kong, Tyk, KrakenD e Express Gateway.

Cada uma dessas plataformas tinha seus pontos fortes, mas nenhuma se alinhava bem com as demandas operacionais e arquitetônicas do Tinder.

Várias questões centrais surgiram durante a avaliação:

Integração fraca com o Envoy, que serve como a espinha dorsal da malha interna de serviço do Tinder.

A sobrecarga de configuração era alta. Configurar até mesmo rotas ou transformações básicas envolvia arquivos de configuração detalhados, sistemas de plugins desconhecidos ou scripts personalizados.

Curvas de aprendizado íngremes retardaram o onboarding e a depuração. As equipes precisavam aprender o interior de cada gateway em vez de focar em entregar recursos.

O suporte ruim para as linguagens e ferramentas preferidas do Tinder significava mais código de colagem e menos reutilização. O atrito aumentou rapidamente.

A extensibilidade era limitada. Adicionar filtros personalizados ou middleware frequentemente significava forkar o gateway, escrever plugins não suportados ou lidar com hooks de ciclo de vida frágeis.

O que é TAG? TAG, abreviação de Tinder API Gateway, é um framework baseado em JVM construído sobre o Spring Cloud Gateway.

Não é um produto plug-and-play nem uma única instância de gateway compartilhada. É um kit de ferramentas para construir gateways. Cada equipe de aplicação pode usá-lo para criar sua própria instância de gateway de API, adaptada às suas rotas, filtros e necessidades de tráfego específicas. Veja o diagrama abaixo para referência:

<img width="1100" height="641" alt="image" src="https://github.com/user-attachments/assets/c11c240d-6398-4464-a0a2-fe122f173f93" />

No seu cerne, o TAG transforma a configuração em infraestrutura. As equipes definem suas rotas, regras de segurança e comportamento de middleware usando arquivos simples YAML ou JSON. O TAG cuida do resto ligando tudo nos bastidores usando o motor reativo da Spring.

Esse design desbloqueia três resultados críticos:

Fluxos de trabalho mais rápidos para desenvolvedores, já que a maioria das mudanças não exige código, apenas configuração.

Limites de segurança mais fortes, porque as equipes possuem e isolam suas instâncias de gateway.

Melhor reutilização, por meio de filtros compartilhados e padrões comuns de middleware.

Do ponto de vista do desenvolvedor, a experiência é a seguinte:

Defina rotas em um arquivo de configuração.

Aplique filtros embutidos como setPath, rewriteResponse ou addHeader.

Reutilize filtros globais para questões compartilhadas, como autenticação ou métricas.

Inclua filtros personalizados onde for necessário validação, transformação ou controle específico.

Fluxo de Boot do TAG: A maioria dos gateways de API sofre quando a configuração cresce. As rotas levam tempo para carregar. Filtros adicionam complexidade. Alguns sistemas até analisam a configuração em tempo real, introduzindo latência no momento da solicitação. O TAG evita isso completamente fazendo o trabalho pesado na inicialização.

Construído sobre o Spring Cloud Gateway, o TAG estende o ciclo de vida padrão com componentes personalizados que processam toda a configuração antes que o tráfego comece a fluir. O resultado é um motor de roteamento totalmente preparado, pronto desde a primeira solicitação.

Veja como funciona o boot flow:

O Gateway Watcher inicia o processo, sinalizando que é hora de carregar as definições de rota.

O Gateway Config Parser lê a configuração YAML específica do ambiente e valida a estrutura. Isso inclui caminhos de rota, predicados, filtros e vinculações de serviços backend.

O Gerenciador de Gateway monta um mapeamento dos IDs de rota para seus filtros associados (pré-construídos, personalizados e globais).

O Gateway Route Locator pega esse mapeamento e vincula os predicados de cada rota, filtrando-os para o motor interno de roteamento do Spring Cloud Gateway.

A tabela completa de roteamento é carregada na memória, então, quando o TAG começa a receber tráfego, não há necessidade de análise ou avaliação de configuração em tempo de execução.

<img width="1100" height="754" alt="unnamed" src="https://github.com/user-attachments/assets/bd030964-3903-41a2-8d41-488149b16da5" />

Esse projeto garante que a lógica de roteamento seja executada com sobrecarga mínima. Todas as decisões já foram tomadas. Cada rota, predicado e filtro é compilado no grafo de tempo de execução.

A troca é simples e deliberada: se algo estiver configurado incorretamente, o gateway falha rapidamente na inicialização em vez de falhar lentamente durante o tráfego de produção. Ele impõe a correção cedo e protege o desempenho em tempo de execução.

Ciclo de Vida de Solicitação no TAG
Quando uma solicitação atinge um gateway alimentado por TAG, ela passa por um pipeline bem definido de filtros, transformações e consultas antes de chegar ao backend. Esse fluxo é um caminho de execução consistente que dá controle às equipes em cada etapa.

Veja o diagrama abaixo:

<img width="1100" height="696" alt="unnamed" src="https://github.com/user-attachments/assets/5e5adc5c-5b2f-462c-a302-3808e41d053c" />

Veja como o TAG lida com uma solicitação recebida do início ao fim:

Busca Reversa de IP Geo (RGIL)
O primeiro passo é a geolocalização. O TAG aplica um filtro global que mapeia o endereço IP do cliente para um código de país ISO de três letras. Este teste leve alimenta:

Limitação de taxa específica por país

Banimento de pedidos geo-conscientes

Comportamento regional de características

O filtro roda antes de qualquer correspondência de rota, garantindo que até caminhos inválidos ou bloqueados possam ser parados antecipadamente.

Varredura de Solicitação e Resposta
O TAG captura esquemas de requisição e resposta, não cargas completas. Isso acontece por meio de um filtro global e assíncrono que publica eventos na Amazon MSK (Kafka).

O fluxo de dados possibilita:

1. Geração automática de esquemas para documentação de API

2. Detecção de bots, baseada em padrões e formato de requisição

3. Ferramentas de detecção de anomalias que analisam a estrutura do tráfego em tempo real

4. O filtro funciona fora da thread principal, evitando impacto na latência da requisição.

Gerenciamento de Sessões: Um filtro global centralizado lida com a validação e atualizações das sessões, garantindo que a lógica da sessão permaneça consistente em todos os gateways e serviços.

Não há desvio por sessão por serviço ou lógica duplicada.

Correspondência de Predicados: Uma vez concluídos os filtros preliminares, o TAG corresponde ao caminho da requisição a uma rota configurada usando o mecanismo de predicados do Spring Cloud Gateway.

Se nenhuma correspondência for encontrada, o pedido é rejeitado antecipadamente.

Descoberta de Serviços (Service Discovery): Com a rota identificada, o TAG usa a malha de serviço do Envoy para resolver o serviço backend correto. Essa abordagem desacopla o roteamento de IPs fixos ou listas de serviço estáticas.

Pré-Filtros: Antes de encaminhar a solicitação, o TAG aplica quaisquer pré-filtros definidos para essa rota. Esses podem incluir:

Roteamento ponderado entre diferentes versões do backend.

Conversão de HTTP para gRPC, quando os clientes frontend falam HTTP, mas o backend fala gRPC.

Filtros personalizados, como cortar cabeçalhos ou validar campos de requisição.

Os pré-filtros rodam em uma sequência definida, determinada pela configuração.

Pós-Filtros: Após a resposta do serviço de backend, o TAG processa a saída por meio de filtros pós-post. Esses frequentemente incluem:

Registro ou enriquecimento de erros

Modificação de cabeçalhos ou mascaramento de campos sensíveis

Transformações de resposta para normalização de formas

Novamente, a ordem de execução é configurável.

Resposta Final
Uma vez que todos os filtros pós-filtros estejam concluídos, a resposta final é enviada de volta ao cliente. Sem surpresas, sem efeitos colaterais.

Todo filtro (pré, pós, global ou personalizado) segue uma ordem de execução rigorosa. Desenvolvedores podem:

Insira lógica personalizada em qualquer etapa.

Compartilhe filtros entre rotas.

Defina a prioridade exata de execução.

Essa previsibilidade é o que torna o TAG sustentável sob carga.

Conclusão
O TAG se tornou o framework padrão de gateway de API em todo o Tinder. Em vez de depender de uma única instância centralizada de gateway, cada equipe de aplicação implanta sua instância TAG com configurações específicas de cada aplicação. Esse modelo dá autonomia às equipes enquanto preserva a consistência em como as rotas são definidas, o tráfego é filtrado e a segurança é aplicada.

Cada instância de TAG escala de forma independente, facilitando a adaptação a mudanças nos padrões de tráfego, lançamentos de recursos ou prioridades de negócios. A TAG agora alimenta tanto o tráfego B2C quanto B2B, não só para o Tinder, mas também para outras marcas do Match Group como Hinge, OkCupid, PlentyOfFish e Ship.

Veja a visualização abaixo para essa capacidade.

![unnamed](https://github.com/user-attachments/assets/4f9a2d0b-922c-40dd-bb6b-5f5e2c3380b1)

O design do TAG desbloqueia várias vantagens de longo prazo:

A lógica de sessão e autenticação é padronizada, eliminando inconsistências entre equipes e serviços.

O suporte a plugins personalizados permite experimentação rápida e ajustes finos no comportamento na borda.

Sem lock-in de fornecedores, o Tinder controla seu caminho evolutivo sem esperar atualizações do roadmap de terceiros.

O Route-as-Config (RAC) permite que as equipes enviem mudanças mais rápido sem precisar escrever código ou esperar pelas equipes centrais.

Além do uso atual em produção, o TAG estabelece a base para futuras iniciativas que exigem visibilidade e controle na camada da API.
A lição aqui não é que toda empresa precisa construir um gateway personalizado. A lição é que, em certa escala, flexibilidade, consistência e desempenho não podem ser resolvidos apenas com ferramentas prontas. O TAG funciona porque é profundamente moldado por como o Tinder constrói, implanta e defende seu software, sem comprometer a velocidade do desenvolvimento ou a clareza operacional.

## [Microservices] CQRS - Command-query responsability segregation
<img src="https://img.shields.io/badge/Spring_Boot-3.10.7-gold?style=flat&logo=Spring&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-gold?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/RabbitMQ-16.17.0-gold?style=flat&logo=RabbitMQ&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-16.17.0-gold?style=flat&logo=PostgreSQL&logoColor=white"> <img src="https://img.shields.io/badge/Apache_Cassandra-16.1-gold?style=flat&logo=Apache-Cassandra&logoColor=white"> <img src="https://img.shields.io/badge/MongoDB-16.17.0-gold?style=flat&logo=MongoDB&logoColor=white"> <img src="https://img.shields.io/badge/Docker-16.17.0-gold?style=flat&logo=Docker&logoColor=white">

<img src="https://github.com/user-attachments/assets/ae249146-7dec-47c3-86a1-beb52b42c23e" height="277" align="right">

O **CQRS (Command-Query Responsibility Segregation)** é um padrão arquitetural que separa as operações de escrita **comandos** (`command`) das operações de leitura **consultas** (`query`) em um sistema, atribuindo responsabilidades distintas para cada uma delas. Em vez de usar o mesmo modelo de dados e lógica para lidar tanto com as atualizações quanto com as consultas, o <a href="https://medium.com/@edin.sahbaz/a-demo-on-clean-architecture-with-cqrs-and-repository-pattern-in-net-web-api-986838191e74?source=email-afeafff77325-1697176799007-digest.reader--986838191e74----6-98------------------21db751b_aa12_4c21_9185_c81d1d5c1508-1">CQRS</a> propõe que esses dois aspectos sejam tratados de maneira independente, o que permite otimizações específicas para cada cenário. 

CQRS significa Segregação de Responsabilidade por Comando e Consulta, um padrão que isola processos de leitura e atualização de armazenamento de dados. A implementação do CQRS na sua aplicação pode melhorar seu desempenho, escalabilidade e segurança. A flexibilidade obtida ao migrar para o CQRS permite que um sistema evolua de forma mais eficaz ao longo do tempo e impede que instruções de atualização desencadeem conflitos de fusão no nível do domínio.

Modelos separados de consulta e atualização facilitam o design e a implementação. embora o código CQRS não possa ser gerado automaticamente a partir de um esquema de banco de dados usando técnicas de andaime, como ferramentas O/RM (embora você possa adicionar seu código personalizado sobre o código gerado).

Você pode dividir fisicamente os dados de leitura e gravação para maior isolamento. Nesse caso, o banco de dados de leitura pode utilizar seu próprio esquema de dados otimizado para consultas. Ele pode, por exemplo, armazenar uma visualização materializada dos dados para evitar junções complexas ou mapeamentos O/RM. Pode até empregar um tipo diferente de armazenamento de dados. 

Por exemplo, o banco de dados de escrita pode ser relacional, e o banco de dados de leitura pode ser um banco de dados de documentos.

No contexto de comandos, o foco está em realizar mudanças no estado da aplicação. Essas operações geralmente envolvem regras de negócios que precisam ser validadas antes que os dados sejam modificados. Por outro lado, as consultas têm como objetivo apenas recuperar e exibir dados, sem causar impacto no estado do sistema. Essa separação pode resultar em um design mais simples e eficiente, pois permite que cada lado seja modelado e implementado de acordo com suas necessidades específicas.

O CQRS é um dos padrões importantes ao consultar entre microsserviços. Podemos usar o padrão de design CQRS para evitar consultas complexas para se livrar de junções ineficientes. CQRS significa Segregação de Responsabilidade de Comando e Consulta. Basicamente, esse padrão separa as operações de leitura e atualização de um banco de dados.

Normalmente, em aplicações monolíticas, na maioria das vezes temos 1 banco de dados e esse banco de dados deve responder tanto às operações de consulta quanto de atualização. Isso significa que um banco de dados está trabalhando para consultas de junção complexas e também executa operações CRUD. Mas se o aplicativo for mais complexo, essa consulta e as operações crud também serão uma situação não gerenciável.

No exemplo de leitura de banco de dados, se seu aplicativo exigiu alguma consulta que precisa unir mais de 10 tabelas, isso bloqueará o banco de dados devido à latência da computação da consulta. Além disso, se dermos um exemplo de gravação de banco de dados, ao realizar operações crud, precisaríamos fazer validações complexas e processar lógicas de negócios longas, portanto, isso causará o bloqueio das operações do banco de dados.

Além disso, o CQRS se integra bem a outras abordagens, como Event Sourcing, onde as mudanças de estado são representadas por eventos. Nesse caso, os comandos geram eventos que podem ser armazenados e usados para reconstruir o estado atual do sistema, enquanto as consultas podem acessar modelos de leitura otimizados que foram derivados desses eventos.

O CQRS é especialmente útil em sistemas complexos, onde as operações de leitura e escrita têm diferentes requisitos de desempenho, escalabilidade ou segurança. Ele também facilita a evolução do sistema, pois a separação de responsabilidades torna mais fácil introduzir novas funcionalidades ou modificar as existentes sem impacto significativo em outras partes do código. No entanto, sua implementação pode aumentar a complexidade inicial, e é importante avaliar se os benefícios justificam o esforço em projetos de menor escala ou simplicidade.

Aplicar estilos e padrões arquiteturais adequados em nossos componentes de software demonstram maturidade em sua base de construção. A decisão correta demanda esforço de maneira a prosperar, e sem dúvida, a escolha certa torna-se um grande ponto de partida para o sucesso de nossa aplicação, naturalmente facilitando adoção posterior de outros padrões/conceitos que estejam preparados para enfrentarmos as dificuldades relacionadas às aplicações distribuídas.

Independente do padrão de implementação adotado em nossas API’s/componentes, seja RESTful/CRUD/EDA (event-driven architecture), naturezas de comunicação síncronas/assíncronas, quando utilizada a Arquitetura de Microsserviços o padrão CQRS poderá agregar benefícios como veremos a seguir. Além disso, aplicado juntamente a outros conceitos complementares (Event Sourcing, DDD) atribuem a nossas aplicações um diferencial competitivo quando abraçamos os principais desafios pertencentes aos sistemas distribuídos.

<img width="720" height="397" alt="image" src="https://github.com/user-attachments/assets/eeea5a97-7dfb-471d-9206-09f1b140b6cd" />

Portanto, a leitura e a gravação do banco de dados têm abordagens diferentes para que possamos definir estratégias diferentes para lidar com essa operação. Para isso, o CQRS oferece o uso de princípios de "separação de preocupações" e banco de dados de leitura separado e o banco de dados de gravação com 2 bancos de dados. Dessa forma, podemos até usar diferentes bancos de dados para ler e gravar tipos de banco de dados, como usar no-sql para leitura e usar banco de dados relacional para operações crud.

Outra consideração é que devemos entender os comportamentos de caso de uso de nosso aplicativo, se nosso aplicativo estiver principalmente lendo casos de uso e não escrevendo tanto, podemos dizer que nosso aplicativo é um aplicativo de incentivo de leitura. Portanto, devemos projetar nossa arquitetura de acordo com nossos requisitos de leitura, concentrando-se em bancos de dados de leitura.

Portanto, podemos dizer que o CQRS separa leituras e gravações em diferentes bancos de dados, Comandos executa dados de atualização, Consultas executa dados de leitura.

Os comandos devem ser ações com operações baseadas em tarefas, como "adicionar item ao carrinho de compras" ou "pedido de check-out". Portanto, os comandos podem ser manipulados com sistemas de agentes de mensagens que fornecem comandos de processamento de maneira assíncrona.

Consultas nunca é modificar o banco de dados. As consultas sempre retornam os dados JSON com objetos DTO. Dessa forma, podemos isolar os Comandos e Consultas.

Para isolar Comandos e Consultas, suas melhores práticas para separar o banco de dados de leitura e gravação com 2 bancos de dados fisicamente. Dessa forma, se nosso aplicativo for de leitura intensiva, o que significa ler mais do que escrever, podemos definir um esquema de dados personalizado para otimizar as consultas.

O padrão de exibição materializado é um bom exemplo para implementar bancos de dados de leitura. Porque desta forma podemos evitar junções e mapeamentos complexos com dados pré-definidos e refinados para operações de consulta.

<img width="700" height="388" alt="image" src="https://github.com/user-attachments/assets/f72ef3dd-acfb-4276-bf90-7311651b8ed0" />

Por esse isolamento, podemos até usar diferentes bancos de dados para ler e gravar tipos de banco de dados, como usar banco de dados de documentos no-sql para leitura e usar banco de dados relacional para operações crud.

Exemplo: Arquitetura de banco de dados do Instagram - Isso é tão popular na arquitetura de microsserviços que também me permite dar um exemplo da arquitetura do Instagram. O Instagram basicamente usa dois sistemas de banco de dados, um é o banco de dados relacional PostgreSQL e o outro é o banco de dados no-sql - Cassandra.

<img width="720" height="692" alt="image" src="https://github.com/user-attachments/assets/ab4b021d-2557-46d1-93c7-dd53f643d77d" />

Isso significa que o Instagram usa o banco de dados Cassandra no-sql para histórias de usuários que são dados de incentivo de leitura. E usando o banco de dados PostgreSQL relacional para atualização da biografia de informações do usuário. Este é um dos exemplos de abordagens do CRQS.

Como sincronizar bancos de dados com CQRS? Mas quando separamos os bancos de dados de leitura e gravação em 2 bancos de dados diferentes, a principal consideração é sincronizar esses dois bancos de dados de maneira adequada.

Portanto, devemos sincronizar esses 2 bancos de dados e manter a sincronização sempre.

Isso pode ser resolvido usando a Arquitetura Orientada a Eventos. De acordo com a Arquitetura Orientada a Eventos, quando algo é atualizado no banco de dados de gravação, ele publicará um evento de atualização com o uso de sistemas de agente de mensagens e isso consumirá pelo banco de dados de leitura e sincronizará os dados de acordo com as alterações mais recentes.

Mas essa solução cria um problema de consistência, porque, como implementamos a comunicação assíncrona com agentes de mensagens, os dados não seriam refletidos imediatamente.

<img width="720" height="456" alt="image" src="https://github.com/user-attachments/assets/f590654a-1943-4f1b-9cae-c5435847e514" />

Isso operará o princípio da "consistência eventual". O banco de dados de leitura eventualmente sincroniza com o banco de dados de gravação e pode levar algum tempo para atualizar o banco de dados de leitura no processo assíncrono. Discutiremos a consistência eventual nas próximas seções.

Portanto, se voltarmos aos nossos bancos de dados de leitura e gravação no padrão CQRS, ao iniciar seu design, você pode obter o banco de dados de leitura de réplicas do banco de dados de gravação. Dessa forma, podemos usar diferentes réplicas somente leitura com a aplicação do padrão de exibição materializado que pode aumentar significativamente o desempenho da consulta.

Além disso, quando separamos bancos de dados de leitura e gravação, isso significa que podemos escalá-los de forma independente. Isso significa que, se nosso aplicativo for de incentivo de leitura, quero dizer, se for muito mais consulta que grava, do que podemos escalar apenas lendo bancos de dados muito rápido.

O CQRS vem com comandos de separação e bancos de dados de consulta. Portanto, isso exigia sincronizar os dois bancos de dados com a oferta de arquiteturas orientadas a eventos. E com arquiteturas controladas por eventos, existem alguns novos padrões e práticas que devem ser considerados ao aplicar o CQRS.

O padrão de Fornecimento de Eventos é o primeiro padrão que devemos considerar para usar com o CQRS. Principalmente o CQRS está usando com "Padrão de Fornecimento de Eventos" em Arquiteturas Controladas por Eventos. Portanto, depois de aprendermos o CQRS, devemos aprender o "padrão de fornecimento de eventos", porque o CQRS e o "padrão de fornecimento de eventos" são as melhores práticas para usar os dois.

Projetar a arquitetura — CQRS, fornecimento de eventos, consistência eventual, exibição materializada

Vamos projetar nossa arquitetura de comércio eletrônico com a aplicação do padrão CQRS:

<img width="700" height="338" alt="image" src="https://github.com/user-attachments/assets/6eae286e-09c6-48f5-bb59-96b1858c3963" />

Agora podemos projetar nossos bancos de dados de microsserviços de pedidos

Vou dividir 2 bancos de dados para ordenar microsserviços 1 para o banco de dados de gravação para questões relacionais 2 para o banco de dados de leitura para consultar preocupações.

Então, quando o usuário criar ou atualizar um pedido, usarei o banco de dados de gravação relacional e, quando o pedido de consulta do usuário ou o histórico de pedidos, usarei o banco de dados de leitura no-sql. e torná-los consistentes ao sincronizar 2 bancos de dados com o uso do sistema de agente de mensagens com a aplicação do padrão de publicação/assinatura.

Agora podemos considerar a pilha de tecnologia desses bancos de dados, vou usar o SQL Server para o banco de dados de escrita relacional e o Cassandra para o banco de dados de leitura no-sql. É claro que usaremos o Kafka para sincronizar esses 2 bancos de dados com as trocas de tópicos pub / sub Kafka.

Portanto, devemos evoluir nossa arquitetura com a aplicação de outros padrões de dados de microsserviços para acomodar adaptações de negócios, tempo de lançamento no mercado mais rápido e lidar com solicitações maiores.

https://medium.com/@martinstm/cqrs-pattern-c-a6632693d3e1

## [Microservices] SAGA
<a href="https://medium.com/@joudwawad/microservices-pattern-distributed-transactions-saga-92b5e933cea1"><img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"></a> <img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/DEV-Saga-blue?style=flat&logo=dev.to&logoColor=white"> <img src="https://img.shields.io/badge/GitBook-Saga-blue?style=flat&logo=GitBook&logoColor=white"> <img src="https://img.shields.io/badge/Confluence-Saga-blue?style=flat&logo=Confluence&logoColor=white">

<img src="https://github.com/user-attachments/assets/54637f6c-1d52-43e8-bfbd-f59840a423b8" align="right" height="77">

O padrão **Saga** (Saga Pattern) foi originalmente proposto pelos cientistas da computação Hector Gracia Molina e Kenneth Salem, é uma abordagem para gerenciar transações distribuídas em uma arquitetura de microsserviços. Em sistemas distribuídos, uma **transação** (transaction) pode envolver múltiplos microsserviços, o que torna o uso de transações tradicionais (como as que utilizam o protocolo de commit em duas fases) impraticável devido à complexidade e ao impacto na performance. 

O padrão <a href="https://medium.com/swlh/microservices-architecture-what-is-saga-pattern-and-how-important-is-it-55f56cfedd6b">Saga</a> oferece uma maneira de garantir a consistência dos dados e a execução das transações em tais sistemas. O padrão Saga é frequentemente associado ao conceito de Long-Running Transactions (LRTs). SAGA pode ser descrito como uma sequência de transações que podem ser intercaladas com outras transações.

> [!Warning]
> **Problema**: Microserviços têm suas próprias vantagens e desvantagens. Uma dessas desvantagens é gerenciar transações distribuídas. Digamos que sua transação abrange 4 microserviços diferentes. Como garantir que sua transação seja confirmada com sucesso com todas as 4 tarefas ou fracasse se alguma das tarefas não for concluída (as concluídas forem revertidas)? O Spring Boot fornece a `@Transactional` de anotação para gerenciar transações. Mas isso funciona apenas dentro de um único método e dentro de um único projeto.

> [!Tip]
> **Solução**: Existe um padrão de design que resolve o problema com transações distribuídas em microserviços e ele surgiu exatamente porque o modelo clássico de transações distribuídas — o famoso Two-Phase Commit (2PC) — simplesmente não escala bem nem combina com os princípios de microserviços. O padrão que resolve esse problema de forma pragmática é o Saga Pattern, e ele parte de uma mudança mental importante: em vez de tentar garantir atomicidade global forte, ele assume que falhas vão acontecer e modela explicitamente como o sistema deve se recuperar delas.

O Spring Boot fornece a `@Transactional` de anotação para gerenciar transações. Mas isso funciona apenas dentro de um único método e dentro de um único projeto.

Nos aprofundamos no intrincado mundo das transações distribuídas através das lentes do padrão SAGA, uma estratégia fundamental para gerenciar a consistência de dados em arquiteturas de microsserviços descentralizadas. Com o brilho dos microsserviços, o SAGA é quase a solução ideal quando se trata de transações distribuídas, entender como lidar efetivamente com transações que abrangem vários serviços torna-se crucial. Esta discussão visa não apenas esclarecer os princípios fundamentais dos SAGAs, mas também fornecer insights práticos sobre sua aplicação estratégica, garantindo interações robustas e sem erros dentro de seus serviços.

Uma compreensão fundamental dos microsserviços é essencial para compreender totalmente as nuances das SAGAs. Recomenda-se que os leitores tenham familiaridade com os vários mecanismos de comunicação empregados em arquiteturas de microsserviços. Para aqueles que buscam aprofundar seus conhecimentos, convido você a ler meu post detalhado no blog, <a href="https://medium.com/@joudwawad/a-guide-to-communication-styles-in-microservices-architecture-9a8ae4bc21b2">"Um Guia para Estilos de Comunicação na Arquitetura de Microsserviços"</a>, que oferece uma análise aprofundada sobre esse assunto.

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/be0e8414-d158-4c2e-bd18-65718528780d">

Da arquitetura monolítica à arquitetura de microsserviços, quase todas as solicitações tratadas por um aplicativo empresarial são executadas em uma transação de <a href="https://blog.dataengineerthings.org/breaking-apart-legacy-databases-a-personal-guide-to-microservices-data-migration-f0b18fa412fd">banco de dados</a>. Os desenvolvedores de aplicativos corporativos usam estruturas e bibliotecas que simplificam o gerenciamento de transações. Algumas estruturas e bibliotecas fornecem uma API programática para iniciar, confirmar e reverter transações explicitamente. Outras estruturas, como a estrutura Spring, fornecem um mecanismo declarativo.

O Spring fornece uma anotação `@Transactional` que organiza as invocações de método a serem executadas automaticamente em uma transação. Como resultado, é simples escrever lógica de negócios transacional.

> [!Warning]
> Deixei nosso backend Java 50x mais rápido substituindo essa anotação, veja como uma anotação aparentemente inocente da primavera estava silenciosamente matando o desempenho abaixo.

Nosso backend era lento. Não é "esperar um arquivo para baixar". Quero dizer, vovó atravessando a rua com um andaril. Cada pedido se arrastava como se tivesse acabado de correr uma maratona de chinelos.

O uso da CPU estava suspeitosamente alto, os logs GC pareciam um ECG, e os tempos de resposta... Bem, digamos que os usuários não ficaram satisfeitos.

Eu já tinha feito a dança de sempre: perfilar, otimizar consultas, ajustar as bandeiras da JVM, rezar para os deuses do GC. Nada funcionou...

E então — durante mais uma sessão de perfil — encontrei o culpado. Não era uma consulta de banco de dados. Não foi uma grande serialização em JSON. Nem era um código ruim. Era o `@Transactional`, sim, aquela inocente anotação da primavera.

**A Cena do Crime**: `@Transactional` é como fita adesiva. Fácil de colocar. Mantém tudo unido. Mas comece a usá-la em todos os lugares, e de repente você já construiu toda a casa com fita adesiva. E fita adesiva não é aço.

Nossa equipe havia espalhado todos os métodos de serviço `@Transactional`

> Porque, sabe, "só por precaução." Como colocar um impermeável no deserto—suado, desnecessário e, eventualmente, com cheiro ruim.

O problema? Todo `@Transactional` abre um proxy, intercepta chamadas, inicia uma transação (mesmo para operações somente leitura) e funciona bem com o `PlatformTransactionManager` subjacente. 

Isso não é de graça, na verdade, quando seu app está lidando com milhares de solicitações por segundo, esse "gratuito" começa a parecer uma assinatura premium da Netflix que você nunca quis.

**O Momento Ahá-Ha**: Durante o perfil, percebi que 40% do tempo de execução estava sendo consumido pela sobrecarga de transações — para métodos que nem sequer modificavam o banco de dados.

Imagine pagar um pedágio toda vez que passar pela ponte sem nem atravessá-la.

Então decidi tentar algo radical: remover dos métodos somente leitura `@Transactional`.

**O Substituto**: Em vez de bater cegamente em todos os lugares, eu: `@Transactional`

1. Marcou apenas operações de escrita como `@Transactional`

2. Para operações com muita leitura, removi completamente ou usei:

```java
@Transactional(readOnly = true)
```

3. Melhor ainda, para alguns caminhos críticos de desempenho, abandonei completamente o gerenciamento de transações do Spring e deixei os métodos do repositório cuidarem do que precisavam.

**Os Resultados**: O impacto? Como trocar uma bicicleta por um trem-bala.

- 50 vezes mais rápido para alguns endpoints.
- A carga do processador foi reduzida pela metade.
- A atividade do GC caiu quase para nada.
- Os usuários pararam de me enviar "o site está fora do ar?" Mensagens no Slack.

Tudo porque substituí (ou removi) uma anotação.

**A Realidade**: Agora, antes de correr e sair para uma onda de deletes, lembre-se: `grep -r "@Transactional"`

- Transações são críticas para a integridade dos dados.
- Se você está modificando dados, precisa deles.
- Transações somente leitura ainda podem ser úteis para garantir alguma consistência.

Mas, por favor pelo amor do código limpo pare de colocá-los em todos os métodos "só por precaução." Isso é como usar capacete para dormir porque "nunca se sabe."

**O Aprendizado**: O código mais rápido é o que não roda. Cada anotação tem um custo. é poderoso, mas não é gratuito `@Transactional`

Da próxima vez que seu backend parecer lento, não olhe apenas para seu banco de dados ou rede. Confira suas anotações.

O problema pode ser uma linha de código que exige silenciosamente cada solicitação.

Ou, para ser mais preciso, o gerenciamento de transações é simples em um aplicativo monolítico que acessa um único banco de dados. O gerenciamento de transações é mais desafiador em um aplicativo monolítico complexo que usa vários bancos de dados e agentes de mensagens.

E em uma arquitetura de microsserviços, as transações abrangem vários serviços, cada um com seu próprio banco de dados.

Nessa situação, o aplicativo deve usar um mecanismo mais elaborado para gerenciar transações. Como você aprenderá nesta postagem do blog, a abordagem tradicional de usar transações distribuídas não é uma opção viável para aplicativos modernos. Em vez disso, um aplicativo baseado em microsserviços deve usar sagas.

A necessidade de transações distribuídas em uma arquitetura de microsserviços. Imagine que você é um desenvolvedor encarregado de implementar uma operação do sistema, essa operação deve: `createOrder()`

1. Verificar se um consumidor (cliente) pode fazer um pedido
2. Verifique os detalhes do pedido
3. Autorizar o cartão de crédito do consumidor
4. Crie um pedido no banco de dados.

É relativamente simples implementar essa operação em um aplicativo monolítico, todos os dados necessários para validar o pedido são prontamente acessíveis no monolítico. Além disso, você pode usar uma transação ACID para garantir a consistência dos dados.

Por outro lado, implementar a mesma operação em uma arquitetura de microsserviço é muito mais complicado. Nos microsserviços, os dados necessários estão espalhados por vários serviços, a operação acessa dados em vários serviços, conforme mostrado na Figura a seguir `createOrder()`

![1_RB5nSJvVQGKotfT8YIlFSQ](https://github.com/user-attachments/assets/8d6d9105-27d1-4fc3-a18b-cd6eb7251a39)

Explorando a integração de vários serviços em uma arquitetura de microsserviços

Ele lê dados do Atendimento ao consumidor e atualiza dados no `Serviço de pedidos`, `Serviço de cozinha` e `Serviço de contabilidade`. Como cada serviço tem seu próprio banco de dados, você precisa usar um mecanismo para manter a consistência dos dados nesses bancos de dados.

O problema com transações distribuídas: A abordagem tradicional para manter a consistência dos dados em vários serviços, bancos de dados ou agentes de mensagens é usar transações distribuídas. O padrão de fato para gerenciamento de transações distribuídas é o Modelo de Processamento de Transações Distribuídas (DTP) X / Open, XA usa confirmação de duas fases (2PC) para garantir que todos os participantes de uma transação se comprometam ou revertam.

Uma pilha de tecnologia compatível com XA consiste em bancos de dados e agentes de mensagens compatíveis com XA, drivers de banco de dados, APIs de mensagens e um mecanismo de comunicação entre processos que propaga o ID de transação global XA. A maioria dos bancos de dados SQL é compatível com XA, assim como alguns agentes de mensagens.

Por mais simples que pareça, há uma variedade de problemas com transações distribuídas heterogêneas. Um problema é que muitas tecnologias modernas, incluindo bancos de dados NoSQL, como MongoDB e Cassandra, não os suportam. Além disso, as transações distribuídas não são suportadas por agentes de mensagens modernos, como RabbitMQ e Apache Kafka.

Como resultado, se você insistir em usar transações distribuídas, estará limitado às tecnologias que podem suportar esse tipo de transação.

Outro problema com as transações distribuídas é que elas são uma forma de IPC (comunicação entre processos) síncrona, o que reduz a disponibilidade. Para que uma transação distribuída seja confirmada, todos os serviços participantes devem estar disponíveis.
A disponibilidade é o produto da disponibilidade de todos os participantes da transação. Se uma transação distribuída envolver dois serviços com 99,5% de disponibilidade, a disponibilidade geral será de 99%, o que é significativamente menor. Cada serviço adicional envolvido em uma transação distribuída reduz ainda mais a disponibilidade.

Superficialmente, as transações distribuídas são atraentes. Do ponto de vista de um desenvolvedor, eles têm o mesmo modelo de programação que as transações locais. Mas devido aos problemas mencionados até agora, as transações distribuídas não são uma tecnologia viável para aplicativos modernos.

Usando o padrão SAGA para manter a consistência dos dados: SAGAs são mecanismos para manter a consistência dos dados em uma arquitetura de microsserviço sem precisar usar transações distribuídas. Você define um SAGA para cada comando do sistema que precisa atualizar dados em vários serviços. Um SAGA é uma sequência de transações locais. Cada transação local atualiza dados em um único serviço usando as estruturas e bibliotecas de transações ACID familiares.

A operação do sistema inicia a primeira etapa do SAGA. A conclusão de uma transação local aciona a execução da próxima transação local.

Posteriormente, você verá como a coordenação das etapas é implementada usando mensagens assíncronas. Um benefício importante do sistema de mensagens assíncrono é que ele garante que todas as etapas de um SAGA sejam executadas, mesmo que um ou mais participantes da saga estejam temporariamente indisponíveis.

Os SAGAs diferem das transações ACID de algumas maneiras importantes. Eles não têm a propriedade de isolamento das transações ACID.

UM EXEMPLO DE SAGA: A SAGA 'CREATEOrder', a saga de exemplo usada em toda esta postagem do blog é o , que é mostrado na figura a seguir. O Serviço de Pedidos implementa a operação usando esta SAGA. A primeira transação local da SAGA é iniciada pela solicitação externa para criar um pedido. As outras cinco transações locais são acionadas pela conclusão da anterior. `Create Order SAGAcreateOrder()`

![1__2rGT54C72Zt3WILl1bW4w](https://github.com/user-attachments/assets/2b7d8513-3bf2-46a8-ab79-1e76c0c4c1e6)

Esta saga consiste nas seguintes transações locais:

1. Serviço de pedido — Crie um pedido em um `state.APPROVAL_PENDING`
2. Atendimento ao consumidor — Verifique se o consumidor pode fazer um pedido.
3. Serviço de cozinha — Valide os detalhes do pedido e crie um tíquete no `.CREATE_PENDING`
4. Serviço de contabilidade — Autorize o cartão de crédito do consumidor.
5. Serviço de cozinha — Altere o estado do Ticket para `.AWAITING_ACCEPTANCE`
6. Serviço de pedido — Altere o estado do pedido para `.APPROVED`

Um serviço publica uma mensagem quando uma transação local é concluída. Essa mensagem aciona a próxima etapa do SAGA, não apenas o uso de mensagens garante que os participantes do SAGA estejam fracamente acoplados, mas também garante que um SAGA seja concluído. Isso ocorre porque, se o destinatário de uma mensagem estiver temporariamente indisponível, o agente de mensagens armazenará a mensagem em buffer até que ela possa ser entregue.

Os SAGAs usam transações de compensação para reverter as alterações. Um grande recurso das transações ACID tradicionais é que a lógica de negócios pode reverter facilmente uma transação se detectar uma violação de uma regra de negócios. Ele executa uma instrução ROLL-BACK e o banco de dados desfaz todas as alterações feitas até o momento. Infelizmente, os SAGAs não podem ser revertidos automaticamente, porque cada etapa confirma suas alterações no banco de dados local.

Isso significa, por exemplo, que se a autorização do cartão de crédito falhar na quarta etapa do `Create Order SAGA`, o aplicativo deverá desfazer explicitamente as alterações feitas pelas três primeiras etapas. Você deve escrever o que é conhecido como transações de compensação.

![1_5NcEiR9QpU5AB64aPXneqQ](https://github.com/user-attachments/assets/011ca86d-cad2-4e87-9c83-6ae6b25f4c4b)

O SAGA executa as operações de compensação na ordem inversa das operações a termo:
- `Cn ... C1`. A mecânica de sequenciar o não é diferente de sequenciar o .
- A conclusão de `C(i)` deve desencadear a execução de `C(i-1).C(i)sT(i)s`

Considere, por exemplo, a `SAGA Create Order`. Esta SAGA pode falhar por vários motivos:

- As informações do consumidor são inválidas ou o consumidor não tem permissão para criar pedidos.
- As informações do restaurante são inválidas ou o restaurante não pode aceitar pedidos.
- A autorização do cartão de crédito do consumidor falha.

Se uma transação local falhar, o mecanismo de coordenação da saga deve executar transações de compensação que rejeitem a Ordem e, possivelmente, o Ticket.

A tabela a seguir mostra as transações de compensação para cada etapa da SAGA Criar Ordem. É importante observar que nem todas as etapas precisam de transações de compensação. As etapas somente leitura, como `verifyConsumerDetails()`, não precisam de transações de compensação. Nem passos como esse são seguidos por passos que sempre são bem-sucedidos`.authorizeCreditCard()`

![1_-sDXfjPYjdl-VADtx710Vg](https://github.com/user-attachments/assets/57da095f-11c2-4f16-b83b-514d1256598e)

Para ver como as transações compensadoras são usadas, imagine um cenário em que a autorização do cartão de crédito do consumidor falha. Nesse cenário, o SAGA executa as seguintes transações locais:

- Serviço de pedido — Crie um pedido em um `state.APPROVAL_PENDING`
- Atendimento ao consumidor — Verifique se o consumidor pode fazer um pedido.
- Serviço de cozinha — Valide os detalhes do pedido e crie um tíquete no `state.CREATE_PENDING`
- Serviço de contabilidade — Autorize o cartão de crédito do consumidor, que falha.
- Serviço de cozinha — Altere o estado do Ticket para `.CREATE_REJECTED`
- Serviço de pedido — Altere o estado do pedido para `.REJECTED`
- A quinta e a sexta etapas são transações compensatórias que desfazem as atualizações feitas pelo Kitchen Service e pelo Order Service, respectivamente.
- A lógica de coordenação de um SAGA é responsável por sequenciar a execução de transações a termo e de compensação. Vejamos como isso funciona.

Coordenação de SAGAs: A implementação de um SAGA consiste em uma lógica que coordena as etapas da saga. Quando um SAGA é iniciado por um comando do sistema, a lógica de coordenação deve selecionar e informar ao primeiro participante do SAGA para executar uma transação local. Uma vez concluída essa transação, a coordenação de sequenciamento da SAGA seleciona e invoca o próximo participante da saga.

Esse processo continua até que a SAGA tenha executado todas as etapas.

Se alguma transação local falhar, o SAGA deverá executar as transações de compensação na ordem inversa. Existem algumas maneiras diferentes de estruturar a lógica de coordenação de uma saga:

- **Coreografia** — Distribua a tomada de decisão e o sequenciamento entre os participantes da saga. Eles se comunicam principalmente por meio da troca de eventos.

- **Orquestração** — Centralize a lógica de coordenação de um SAGA em uma classe de orquestrador do SAGA. Um orquestrador do SAGA envia mensagens de comando aos participantes do SAGA informando quais operações executar.
Vejamos cada opção.

SAGAs baseados em coreografias: Uma maneira de implementar um SAGA é usando coreografia. Ao usar a coreografia, não há um coordenador central dizendo aos participantes da SAGA o que fazer. Em vez disso, os participantes da SAGA se inscrevem nos eventos uns dos outros e respondem de acordo.

Vamos implementar a SAGA usando `COREOGRAFIAcreateOrder`

A figura a seguir mostra o design da versão baseada em coreografia do Create Order SAGA. Os participantes se comunicam por meio da troca de eventos. Cada participante, começando com o Serviço de Pedidos, atualiza seu banco de dados e publica um evento que aciona o próximo participante.

![1_dY1KgVQaEIqe_N75sZBuPA](https://github.com/user-attachments/assets/f003496b-8ab6-4ec8-b384-0898adae7080)

O caminho FELIZ por esta SAGA é o seguinte:

1. O Serviço de Pedidos cria um Pedido no estado e publica um `event.APPROVAL_PENDINGOrderCreated`
2. O Serviço ao consumidor consome o evento, verifica se o consumidor pode fazer o pedido e publica um `event.OrderCreatedConsumerVerified`
3. O Kitchen Service consome o evento, valida o pedido, cria um ticket em um estado e publica o `event.OrderCreatedCREATE_PENDINGTicketCreated`
4. O Serviço de Contabilidade consome o evento e cria um em um `state.OrderCreateCreditCardAuthorizationPENDING`
5. O Serviço de Contabilidade consome os eventos and, cobra o cartão de crédito do consumidor e publica o `event.TicketCreatedConsumerVerifiedCreditCardAuthorized`
6. O Kitchen Service consome o evento `CreditCardAuthorized` e altera o estado do Ticket para `.AWAITING_ACCEPTANCE`
7. O serviço de pedido recebe os eventos, altera o estado do pedido para e publica um `event.CreditCardAuthorizedAPPROVEDOrderApproved`
8. A SAGA Criar Ordem também deve lidar com o cenário em que um participante da SAGA rejeita a Ordem e publica algum tipo de evento de falha.

Por exemplo, a autorização do cartão de crédito do consumidor pode falhar. O SAGA deve executar as transações de compensação para desfazer o que já foi feito.

A figura a seguir mostra o fluxo de eventos quando o não é possível autorizar o cartão de crédito do consumidor `AccountingService`

![1_JXEnpcsbDCEuftfUhdxzOg](https://github.com/user-attachments/assets/a5b89131-951d-4bc5-a5c1-1a8db3fd5022)

A sequência de eventos é a seguinte:

1. O Serviço de Pedidos cria um Pedido no estado e publica um `event.APPROVAL_PENDINGOrderCreated`
2. O Serviço ao consumidor consome o evento, verifica se o consumidor pode fazer o pedido e publica um `event.OrderCreatedConsumerVerified`
3. O Kitchen Service consome o evento, valida o pedido, cria um ticket em um estado e publica o `event.OrderCreatedCREATE_PENDINGTicketCreated`
4. O Serviço de Contabilidade consome o evento e cria um em um `state.OrderCreatedCreditCardAuthorizationPENDING`
5. O Serviço de Contabilidade consome os eventos and, cobra o cartão de crédito do consumidor e publica um `event.TicketCreatedConsumerVerifiedCreditCardAuthorizationFailed`
6. O Serviço de Cozinha consome o evento e altera o estado do Ticket para `.CreditCardAuthorizationFailedREJECTED`
7. O Serviço de Pedidos consome o evento e altera o estado do Pedido para `.CreditCardAuthorizationFailedREJECTED`

Como você pode ver, os participantes de SAGAs baseados em coreografia interagem usando publicar/assinar. Vamos dar uma olhada em algumas questões que você precisará considerar ao implementar a comunicação baseada em publicação/assinatura para seus SAGAs.

Comunicação confiável baseada em eventos: Existem algumas questões relacionadas à comunicação entre serviços que você deve considerar ao implementar SAGAs baseados em coreografia:

1. A primeira questão é garantir que um participante do SAGA atualize seu banco de dados e publique um evento como parte de uma transação de banco de dados. Cada etapa de uma SAGA baseada em coreografia atualiza o banco de dados e publica um evento. Por exemplo, na SAGA Criar pedido, o Serviço de cozinha recebe um evento Verificado pelo consumidor, cria um Ticket e publica um evento Ticket Created. É essencial que a atualização do banco de dados e a publicação do evento aconteçam atomicamente. Consequentemente, para se comunicar de forma confiável, os participantes da SAGA devem usar mensagens transacionais

2. A segunda questão que você precisa considerar é garantir que um participante da saga seja capaz de mapear cada evento que recebe para seus próprios dados. Por exemplo, quando o Order Service recebe um evento, ele deve ser capaz de pesquisar o Order correspondente. A solução é que um participante do SAGA publique eventos contendo um, que são dados que permitem que outros participantes executem o mapeamento. Por exemplo, os participantes da Saga Criar Pedido podem usar o orderId como um ID de correlação que é passado de um participante para o outro. O Serviço de Contabilidade publica um evento que contém o `orderId` do `event.CreditCardAuthorized*correlationId*CreditCardAuthorizedTicketCreated`

Benefícios e desvantagens dos SAGAs baseados em coreografia - Os SAGAs baseados em coreografia têm vários benefícios:

- Simplicidade — Os serviços publicam eventos quando criam, atualizam ou excluem objetos de negócios.
- Acoplamento fraco — Os participantes se inscrevem em eventos e não têm conhecimento direto uns dos outros.

E há algumas desvantagens:

- Mais difícil de entender — Ao contrário da orquestração, não há um único lugar no código que defina o SAGA. Em vez disso, a coreografia distribui a implementação do SAGA entre os serviços. Consequentemente, às vezes é difícil para um desenvolvedor entender como um determinado SAGA funciona.
- Dependências cíclicas entre os serviços — Os participantes do SAGA assinam os eventos uns dos outros, o que geralmente cria dependências cíclicas. Por exemplo, se você examinar cuidadosamente os diagramas anteriores, verá que há dependências cíclicas, como .
- Embora isso não seja necessariamente um problema, as dependências cíclicas são consideradas um cheiro de `design.Order Service → Accounting Service → Order Service`
- Risco de acoplamento estreito — Cada participante do SAGA precisa se inscrever em todos os eventos que os afetam. Por exemplo, o Serviço de Contabilidade deve se inscrever em todos os eventos que fazem com que o cartão de crédito do consumidor seja cobrado ou reembolsado. Como resultado, há o risco de que ele precise ser atualizado em sintonia com o ciclo de vida do pedido implementado pelo Serviço de pedido.

Sagas baseadas em orquestração. A orquestração é outra maneira de implementar SAGAs. Ao usar a orquestração, você define uma classe de orquestrador cuja única responsabilidade é dizer aos participantes do SAGA o que fazer. O orquestrador SAGA se comunica com os participantes usando interação no estilo de resposta assíncrona/comando.

Para executar uma etapa do SAGA, ele envia uma mensagem de comando a um participante informando qual operação executar. Depois que o participante do SAGA tiver executado a operação, ele enviará uma mensagem de resposta ao orquestrador. Em seguida, o orquestrador processa a mensagem e determina qual etapa do SAGA deve ser executada em seguida.

Vamos implementar a SAGA usando `ORCHESTRATIONcreateOrder`

A figura a seguir mostra o design da versão baseada em orquestração da SAGA Criar Ordem. O SAGA é orquestrado pela classe `CreateOrderSaga`, que invoca os participantes do SAGA usando solicitação/resposta assíncrona. Essa classe acompanha o processo e envia mensagens de comando aos participantes do SAGA, como Serviço de Cozinha e Serviço ao Consumidor.

A classe lê mensagens de resposta de seu canal de resposta e, em seguida, determina a próxima etapa, se houver, na saga `CreateOrderSaga`

![1_5GXe7OWevr7Xtaf4PZfokg](https://github.com/user-attachments/assets/18b61846-46c5-4bc9-8c91-1398515ba009)

O serviço de pedidos primeiro cria um orquestrador SAGA Order e Create Order Depois disso, o fluxo para o caminho feliz é o seguinte:

1. O orquestrador SAGA envia um comando para o Serviço do Consumidor.Verify Consumer
2. O Serviço de Atendimento ao Consumidor responde com uma mensagem.Consumer Verified
3. O orquestrador SAGA envia um comando para o Serviço de Cozinha.Create Ticket
4. O Serviço de Cozinha responde com uma mensagem.Ticket Created
5. O orquestrador SAGA envia uma mensagem para o Serviço de Contabilidade.Authorize Card
6. O Serviço de Contabilidade responde com uma mensagem.Card Authorized
7. O orquestrador do SAGA envia um comando para o Serviço de Cozinha.Approve Ticket
8. O orquestrador da saga envia um comando para o Serviço de Pedidos.Approve Order
9. Observe que, na etapa final, o orquestrador SAGA envia uma mensagem de comando para o Serviço de pedidos, mesmo que seja um componente do Serviço de pedidos. Em princípio, a Saga Criar Pedido poderia aprovar o Pedido atualizando-o diretamente. Mas, para ser consistente, a SAGA trata o Order Service como apenas mais um participante.

Eu entendo que os SAGAs podem ser complexos, mas para aplicações práticas, este exemplo reflete um fluxo de trabalho típico. Meu objetivo é fornecer um cenário realista nesta postagem do blog para melhorar a compreensão das implementações do mundo real.

**Orquestração SAGA e mensagens transacionais**: Cada etapa de um SAGA baseado em orquestração consiste em um serviço atualizando um banco de dados e publicando uma mensagem. Por exemplo, o Serviço de pedidos persiste um orquestrador de pedidos e um orquestrador Criar saga de pedidos e envia uma mensagem para o primeiro participante do SAGA.

Um participante do SAGA, como o Kitchen Service, lida com uma mensagem de comando atualizando seu banco de dados e enviando uma mensagem de resposta. O Serviço de Pedidos processa a mensagem de resposta do participante atualizando o estado do orquestrador do SAGA e enviando uma mensagem de comando para o próximo participante do SAGA.

Um serviço deve usar mensagens transacionais para atualizar atomicamente o banco de dados e publicar mensagens.

Vantagens e desvantagens dos SAGAs baseados em orquestração
Os SAGAs baseados em orquestração têm vários benefícios:

- Dependências mais simples — Um benefício da orquestração é que ela não introduz dependências cíclicas. O orquestrador do SAGA invoca os participantes do SAGA, mas os participantes não invocam o orquestrador. Como resultado, o orquestrador depende dos participantes, mas não vice-versa e, portanto, não há dependências cíclicas.

- Acoplamento de perda — Cada serviço implementa uma API que é invocada pelo orquestrador, portanto, não precisa saber sobre os eventos publicados pelos participantes do SAGA.

- Melhora a separação de preocupações e simplifica a lógica de negócios — A lógica de coordenação do SAGA está localizada no orquestrador do SAGA. Os objetos de domínio são mais simples e não têm conhecimento dos SAGAs dos quais participam. Por exemplo, ao usar orquestração, a classe Order não tem conhecimento de nenhum dos SAGAs, portanto, tem um modelo de máquina de estado mais simples. Durante a execução da SAGA Create Order, ela faz a transição direta do estado para o estado. A classe Order não tem nenhum estado intermediário correspondente às etapas do SAGA. Como resultado, o negócio é muito mais simples.APPROVAL_PENDINGAPPROVED

- A orquestração também tem uma desvantagem: o risco de centralizar muita lógica de negócios no orquestrador. Isso resulta em um design em que o orquestrador inteligente informa aos serviços burros quais operações fazer. Felizmente, você pode evitar esse problema projetando orquestradores que são os únicos responsáveis pelo sequenciamento e não contêm nenhuma outra lógica de negócios.

**Lidando com a falta de isolamento**: O in ACID significa isolamento. A propriedade de isolamento das transações ACID garante que o resultado da execução simultânea de várias transações seja o mesmo como se elas fossem executadas em alguma ordem serial.I

O banco de dados fornece a ilusão de que cada transação ACID tem acesso exclusivo aos dados. O isolamento facilita muito a escrita de lógica de negócios que é executada simultaneamente.

O desafio de usar SAGAs é que eles não têm a propriedade de isolamento das transações ACID. Isso ocorre porque as atualizações feitas por cada uma das transações locais de uma SAGA são imediatamente visíveis para outras SAGAs assim que a transação é confirmada.

Esse comportamento pode causar dois problemas:

Primeiro, outros SAGAs podem alterar os dados acessados pelo SAGA enquanto ele está em execução. Os outros SAGAs podem ler seus dados antes que o SAGA conclua suas atualizações e, consequentemente, podem ser expostos a dados inconsistentes.

Você pode, de fato, considerar uma SAGA como ACD:

- Atomicidade — A implementação do SAGA garante que todas as transações sejam executadas ou que todas as alterações sejam desfeitas.
- Consistência — A integridade referencial dentro de um serviço é tratada por bancos de dados locais. A integridade referencial entre os serviços é tratada pelos serviços.
- Durabilidade — Manipulado por bancos de dados locais.

Essa falta de isolamento potencialmente causa o que a literatura de banco de dados chama de anomalias.

An é quando uma transação lê ou grava dados de uma forma que não faria se as transações fossem executadas uma de cada vez. Quando ocorre uma anomalia, o resultado da execução simultânea de SAGAs é diferente do que se fossem executadas em série.anomaly

A seguir, discutimos um conjunto de estratégias de design SAGA que lidam com a falta de isolamento, essas estratégias são conhecidas como Algumas contramedidas implementam isolamento no nível do aplicativo. Outras contramedidas reduzem o risco comercial da falta de isolamento.countermeasures

Usando contramedidas, você pode escrever uma lógica de negócios baseada em SAGA que funcione corretamente.

Visão geral das anomalias
A falta de isolamento pode causar as três anomalias a seguir:

Atualizações perdidas — Uma SAGA substitui sem ler as alterações feitas por outra saga.
Leituras sujas — Uma transação ou uma SAGA lê as atualizações feitas por uma saga que ainda não concluiu essas atualizações.
Leituras difusas/não repetíveis — Duas etapas diferentes de um SAGA leem os mesmos dados e obtêm resultados diferentes porque outro SAGA fez atualizações.
Todas as três anomalias podem ocorrer, mas as duas primeiras são as mais comuns e as mais desafiadoras. Vamos dar uma olhada nesses dois tipos de anomalia, começando com atualizações perdidas.

ATUALIZAÇÕES PERDIDAS
Uma anomalia de atualização perdida ocorre quando um SAGA substitui uma atualização feita por outro SAGA.

Considere, por exemplo, o seguinte cenário:

A primeira etapa da SAGA Criar Pedido cria um Pedido.
Enquanto essa SAGA estiver em execução, a SAGA Cancelar Ordem cancelará a Ordem.
A etapa final da SAGA Criar Pedido aprova o Pedido.
Nesse cenário, a Saga Criar Pedido ignora a atualização feita pela Saga Cancelar Pedido e a substitui. Como resultado, o aplicativo enviará um pedido que o cliente cancelou.

LEITURAS SUJAS
Uma leitura suja ocorre quando um SAGA lê dados que estão no meio de serem atualizados por outro SAGA.

Considere, por exemplo, uma versão do aplicativo em que os consumidores têm um limite de crédito. Neste aplicativo, um SAGA que cancela um pedido consiste nas seguintes transações:

Atendimento ao consumidor — Aumente o crédito disponível.
Serviço de pedido — Altere o estado do pedido para cancelar.
Serviço de entrega — Cancele a entrega.
Vamos imaginar um cenário que intercala a execução das SAGAs Cancelar Pedido e Criar Pedido, e a SAGA Cancelar Pedido é revertida porque é tarde demais para cancelar a entrega.
É possível que a sequência de transações que invocam o Serviço do Consumidor seja a seguinte:

Cancelar pedido SAGA — Aumente o crédito disponível.
Criar SAGA de Pedidos — Reduza o crédito disponível.
Cancelar SAGA do pedido — Uma transação de compensação que reduz o crédito disponível.
Nesse cenário, o Create Order SAGA faz uma leitura suja do crédito disponível que permite ao consumidor fazer um pedido que exceda seu limite de crédito. É provável que este seja um risco inaceitável para o negócio.

Vejamos como evitar que esse e outros tipos de anomalias afetem um aplicativo.

Contramedidas para lidar com a falta de isolamento
O modelo de transação SAGA é ACD e sua falta de isolamento pode resultar em anomalias que fazem com que os aplicativos se comportem mal. É responsabilidade do desenvolvedor escrever SAGAs de uma forma que evite as anomalias ou minimize seu impacto nos negócios. Isso pode parecer uma tarefa assustadora, mas você já viu um exemplo de estratégia que evita anomalias. O uso de estados por uma Ordem, como , é um exemplo de uma dessas estratégias.
As SAGAs que atualizam Pedidos, como a SAGA Criar Pedido, começam definindo o estado de um Pedido como . O estado informa a outras transações que a Ordem está sendo atualizada por uma SAGA e deve agir de acordo.*_PENDINGAPPROVAL_PENDING*_PENDING*_PENDING

O uso de estados por uma ordem é um exemplo do que o artigo de 1998 "Propriedades ACID semânticas em multidatabases usando chamadas de procedimento remoto e propagações de atualização" de Lars Frank e Torben U. Zahle chama de contramedida de bloqueio semântico.
O artigo descreve como lidar com a falta de isolamento de transações em arquiteturas de vários bancos de dados que não usam transações distribuídas. Muitas de suas ideias são úteis ao projetar SAGAs.
Ele descreve um conjunto de contramedidas para lidar com anomalias causadas pela falta de isolamento que evitam uma ou mais anomalias ou minimizam seu impacto nos negócios.
As contramedidas descritas por este artigo são as seguintes:*_PENDING

Bloqueio semântico — Um bloqueio no nível do aplicativo.
Atualizações comutativas — Projete as operações de atualização para serem executáveis em qualquer ordem.
Visão pessimista — Reordene as etapas de uma saga para minimizar o risco comercial.
Valor de releitura — Evite gravações sujas relendo os dados para verificar se eles não foram alterados antes de substituí-los.
Arquivo de versão — Registre as atualizações em um registro para que possam ser reordenadas.
Por valor — Use o risco comercial de cada solicitação para selecionar dinamicamente o mecanismo de simultaneidade.
A estrutura de uma SAGA
O artigo de contramedidas mencionado na última seção define um modelo útil para a estrutura de um SAGA. Nesse modelo, mostrado na figura abaixo, um SAGA consiste em três tipos de transações:

Transações compensáveis — Transações que podem ser revertidas usando uma transação de compensação.
Transação de pivô — O ponto de ir / não ir em uma saga. Se a transação dinâmica for confirmada, a saga será executada até a conclusão. Uma transação dinâmica pode ser uma transação que não é compensável nem repetível. Como alternativa, pode ser a última transação compensável ou a primeira transação repassível.
Transações com pedido — Transações que seguem a transação dinâmica e têm garantia de sucesso.

![1_bMIA99rEKI3QDbppA2K_gg](https://github.com/user-attachments/assets/b066b296-4bf3-4f57-b114-f961f2597575)

na ordem de criação SAGA:

As etapas são transações compensáveis.createOrder(), verifyConsumerDetails(), and createTicket()
As transações têm transações de compensação que desfazem suas atualizações.createOrder() and createTicket()
A transação é somente leitura, portanto, não precisa de uma transação de compensação.verifyConsumerDetails()
A transação é a transação pivô desta SAGA. Se o cartão de crédito do consumidor puder ser autorizado, esta SAGA tem garantia de conclusão.authorizeCreditCard()
As etapas e são transações que podem ser repetidas que seguem a transação dinâmica.approveTicket()approveOrder()
A distinção entre transações compensáveis e transações passíveis de recuperação é especialmente importante.
Como você verá, cada tipo de transação desempenha um papel diferente nas contramedidas.

Vejamos agora cada contramedida, começando com a contramedida de bloqueio semântico.

CONTRAMEDIDA: BLOQUEIO SEMÂNTICO
Adiciona um bloqueio à linha que estamos criando ou atualizando para que ela possa ser bloqueada de outros consumidores.

Ao usar a contramedida de bloqueio semântico, a transação compensável de um SAGA define um sinalizador em qualquer registro que ele cria ou atualiza.

O sinalizador indica que o registro não é e pode ser alterado.committed

O sinalizador pode ser um bloqueio que impede que outras transações acessem o registro ou um aviso que indica que outras transações devem tratar esse registro com suspeita.
É compensado por uma transação recuperável - a SAGA está sendo concluída com sucesso - ou por uma transação de compensação: a saga está sendo revertida.

O campo é um ótimo exemplo de bloqueio semântico. Os estados, como e , implementam um bloqueio semântico. Eles dizem a outros SAGAs que acessam um Pedido que um SAGA está em processo de atualização do Pedido.Order.state*_PENDINGAPPROVAL_PENDINGREVISION_PENDING

Por exemplo, a primeira etapa da SAGA Criar Ordem, que é uma transação compensável, cria uma Ordem em um estado. A etapa final da SAGA Criar pedido, que é uma transação que pode ser corrigida, altera o campo para . Uma transação de compensação altera o campo para `.APPROVAL_PENDINGAPPROVEDREJECTED`

Gerenciar o bloqueio é apenas metade do problema. Você também precisa decidir caso a caso como uma SAGA deve lidar com um registro que foi bloqueado. Considere, por exemplo, o comando do sistema. Um cliente pode invocar essa operação para cancelar um pedido que está no `state.cancelOrder()APPROVAL_PENDING`

Existem algumas maneiras diferentes de lidar com esse cenário.

Uma opção é que o comando do sistema falhe e diga ao cliente para tentar novamente mais tarde. O principal benefício dessa abordagem é que ela é simples de implementar. A desvantagem, no entanto, é que isso torna o cliente mais complexo porque precisa implementar a lógica de repetição.cancelOrder()
Outra opção é bloquear até que o bloqueio seja liberado.cancelOrder()
CONTRAMEDIDA: ATUALIZAÇÕES COMUTATIVAS
Projete o SAGA para que possa ser executado em qualquer ordem ~ um exemplo seria um aumento e diminuição de uma conta blanace.

Uma contramedida simples é projetar as operações de atualização para serem comutativas. As operações são se puderem ser executadas em qualquer ordem.
As contas e as operações de uma conta são comutativas (se você ignorar os cheques a descoberto). Essa contramedida é útil porque elimina atualizações perdidas.commutativedebit()credit()

Considere, por exemplo, um cenário em que um SAGA precisa ser revertido depois que uma transação compensável debitou (ou creditou) uma conta. A transação de compensação pode simplesmente creditar (ou debitar) a conta para desfazer a atualização. Não há possibilidade de sobrescrever atualizações feitas por outros SAGAs.

CONTRAMEDIDA: VISÃO PESSIMISTA
Ele reordena as etapas de um SAGA para minimizar o risco de negócios devido a uma leitura suja.

Considere, por exemplo, o cenário usado anteriormente para descrever a anomalia de leitura suja. Nesse cenário, a SAGA Criar Pedido realizou uma leitura suja do crédito disponível e criou um pedido que excedeu o limite de crédito ao consumidor. Para reduzir o risco de isso acontecer, esta contramedida reordenaria o:Cancel Order SAGA

Serviço de pedido — Altere o estado do pedido para cancelado.
Serviço de entrega — Cancele a entrega.
Atendimento ao cliente — Aumente o crédito disponível.
Nesta versão reordenada do SAGA, o crédito disponível é aumentado em uma transação reutilizável, o que elimina a possibilidade de uma leitura suja.

CONTRAMEDIDA: VALOR DE RELEITURA
Um SAGA que usa essa contramedida relê um registro antes de atualizá-lo, verifica se ele não foi alterado e, em seguida, atualiza o registro. Se o registro foi alterado, a saga é abortada e possivelmente reiniciada.

A contramedida de valor de releitura evita atualizações perdidas.

Um SAGA que usa essa contramedida relê um registro antes de atualizá-lo, verifica se ele não foi alterado e, em seguida, atualiza o registro. Se o registro tiver sido alterado, o SAGA será interrompido e possivelmente reiniciado. Essa contramedida é uma forma do padrão Bloqueio Offline Otimista.

Eles podem usar essa contramedida para lidar com o cenário em que o Pedido é cancelado enquanto está em processo de aprovação.
A transação que aprova o pedido verifica se o pedido não foi alterado desde que foi criado anteriormente na SAGA. Se não for alterada, a transação aprova o pedido. Mas se a Ordem foi cancelada, a transação aborta a SAGA, o que faz com que suas transações compensadoras sejam executadas.Create Order SAGA

CONTRAMEDIDA: ARQUIVO DE VERSÃO
Ele registra as operações que são executadas em um registro para que possa executá-las em uma ordem.

A contramedida é assim chamada porque registra as operações executadas em um registro para que ele possa reordená-las. É uma maneira de transformar operações não comutativas em operações comutativas.version file

Para ver como essa contramedida funciona, considere um cenário em que o executa simultaneamente com um . A menos que as sagas usem a contramedida de bloqueio semântico, é possível que o cancele a autorização do cartão de crédito do consumidor antes que a Saga Criar Pedido autorize o cartão.Create Order SAGACancel Order SAGACancel Order SAGA

Uma maneira de o Serviço de Contabilidade lidar com essas solicitações fora de ordem é registrar as operações à medida que elas chegam e executá-las na ordem correta. Nesse cenário, ele registraria primeiro a solicitação de Cancelamento de Autorização. Então, quando o Serviço de Contabilidade receber a solicitação de Autorização de Cartão subsequente, ele perceberá que já recebeu a solicitação de Autorização de Cancelamento e ignorará a autorização do cartão de crédito.

CONTRAMEDIDA: POR VALOR
É uma estratégia para selecionar mecanismos de simultaneidade com base no risco comercial. usa as propriedades de cada solicitação para decidir entre usar sagas e transações distribuídas

A contramedida final é a contramedida. É uma estratégia para selecionar mecanismos de simultaneidade com base no risco comercial. Um aplicativo que usa essa contramedida usa as propriedades de cada solicitação para decidir entre usar SAGAs e transações distribuídas.
Ele executa solicitações de baixo risco usando SAGAs, talvez aplicando as contramedidas descritas na seção anterior. Mas executa solicitações de alto risco envolvendo, por exemplo, grandes quantias de dinheiro, usando transações distribuídas.by value

Essa estratégia permite que um aplicativo faça concessões dinamicamente sobre risco de negócios, disponibilidade e escalabilidade.

É provável que você precise usar uma ou mais dessas contramedidas ao implementar SAGAs em seu aplicativo.

**Long-Running Transactions (LRTs)** são transações que se estendem por um longo período e envolvem múltiplas operações distribuídas, possivelmente em diferentes serviços ou sistemas. Elas não podem ser tratadas com as técnicas tradicionais de transações ACID (Atomicidade, Consistência, Isolamento, Durabilidade) devido à natureza distribuída e à necessidade de alto desempenho e disponibilidade.

Características do Padrão Saga:

1. **Sequência de Passos**: Uma Saga é composta por uma sequência de transações locais, cada uma executada por um serviço diferente. Cada transação local é atômica e independente, mas juntas elas formam uma unidade lógica de trabalho.

2. **Compensação**: Caso alguma transação dentro da Saga falhe, é necessário desfazer (ou compensar) as transações que já foram concluídas para manter a consistência do sistema. Isso é feito através de transações de compensação, que são essencialmente o inverso das operações realizadas.

3. **Coordenação**: A coordenação das transações dentro de uma Saga pode ser feita de duas maneiras: **Coreografia** ou **Orquestração**.

**Coordenação de Sagas**: Na coreografia (Choreography), não há um coordenador central. Cada serviço sabe o que fazer após completar sua transação local e publica um evento que desencadeia a próxima etapa.

- **Vantagens**:
  - Alta descentralização e independência entre serviços.
  - Evita o ponto único de falha.
- **Desvantagens**:
  - Pode ser difícil de gerenciar e depurar devido à complexidade e falta de visibilidade central.
  - Pode levar a dependências cíclicas e aumento do acoplamento entre serviços.

**Exemplo de Coreografia**:

1. Serviço A realiza sua transação e publica um evento.
2. Serviço B escuta o evento do Serviço A, realiza sua transação e publica um novo evento.
3. Serviço C escuta o evento do Serviço B e realiza sua transação, e assim por diante.

Na orquestração (orchestration), um serviço central (o orquestrador) coordena a execução das transações da Saga. O orquestrador chama cada serviço em sequência e gerencia as compensações em caso de falhas.

- **Vantagens**:
  - Visibilidade central e controle do fluxo da transação.
  - Simplicidade na gestão e depuração das transações.

- **Desvantagens**:
  - Introduz um ponto único de falha e potencial gargalo no sistema.
  - Reduz a independência dos serviços.

**Exemplo de Orquestração**:
1. O Orquestrador inicia a transação chamando o Serviço A.
2. Após a conclusão do Serviço A, o Orquestrador chama o Serviço B.
3. Após a conclusão do Serviço B, o Orquestrador chama o Serviço C, e assim por diante.
4. Se o Serviço B falhar, o Orquestrador chama as transações de compensação necessárias para desfazer as operações dos serviços anteriores.

Exemplos de Aplicação do Padrão Saga:

1. **Processamento de Pedidos em E-commerce**:
   - **Passos**: 
     1. Serviço de criação de pedido cria um pedido.
     2. Serviço de pagamento processa o pagamento.
     3. Serviço de inventário reserva os produtos.
     4. Serviço de envio organiza a entrega.
   - **Compensação**: Se o serviço de envio falhar, desfaz-se a reserva no inventário, o pagamento é revertido, e o pedido é cancelado.

2. **Cadastro de Novo Usuário**:
   - **Passos**:
     1. Serviço de autenticação cria as credenciais do usuário.
     2. Serviço de perfil cria o perfil do usuário.
     3. Serviço de notificações envia um e-mail de boas-vindas.
   - **Compensação**: Se o serviço de perfil falhar, as credenciais são removidas.

<img width="720" height="432" alt="image" src="https://github.com/user-attachments/assets/270ee850-9dd0-40ed-95b7-db7154478d92" />

Se você estiver trabalhando em um microsserviço Java ou se preparando para uma entrevista de desenvolvedor Java em que as habilidades de microsserviço são necessárias, você deve se preparar sobre o padrão SAGA.

SAGA é um padrão de microsserviço essencial que visa resolver o problema de transações de longa duração na arquitetura de microsserviços. É também uma das perguntas populares da entrevista de microsserviço, frequentemente feita a desenvolvedores experientes.

Como a arquitetura de microsserviço divide seu aplicativo em vários aplicativos pequenos, uma única solicitação também é dividida em várias solicitações e há uma chance de que algumas partes das solicitações sejam bem-sucedidas e algumas partes falhem, nesse caso, é difícil manter a consistência dos dados.

Se você estiver lidando com dados reais, como fazer um pedido na Amazon, deverá lidar com esse cenário normalmente para que, se o pagamento falhar, o estoque volte ao seu estado original e o pedido não seja enviado.

Neste artigo, vou explicar O que é o padrão SAGA? O que ele faz, qual problema ele resolve, bem como prós e contras do padrão SAGA em uma arquitetura de microsserviço.

A propósito, se você está se preparando para entrevistas com desenvolvedores Java, também pode ver meus artigos anteriores, como 25 perguntas avançadas sobre Java, 25 perguntas sobre Spring Framework, 20 consultas SQL de entrevistas, 50 perguntas sobre microsserviços, 60 perguntas sobre estrutura de dados em árvore, 15 perguntas sobre design de sistema e 35 perguntas sobre Core Java.

E, se você gosta das minhas postagens, considere assinar meu boletim informativo, é GRATUITO e você não postará nenhuma das minhas postagens

O que é o padrão de design da SAGA? Que problema resolve? O padrão SAGA (ou Saga) é um padrão de design de microsserviço para gerenciar a consistência de dados em sistemas distribuídos.

Ele fornece uma maneira de lidar com transações de longa duração compostas por várias etapas, em que cada etapa é uma operação de banco de dados separada. A ideia principal é capturar todas as etapas da transação em um banco de dados para que, em caso de falha, o sistema possa reverter a transação ao seu estado inicial.

O padrão SAGA resolve o problema de manter a consistência dos dados em um sistema distribuído, onde é difícil garantir que todas as operações em uma transação sejam executadas atomicamente, especialmente em caso de falhas.

Um dos exemplos populares do padrão SAGA é uma transação de comércio eletrônico, como fazer um pedido na Amazon ou Flipkart, onde um pedido é feito, o pagamento é deduzido da conta do cliente e os itens são reservados no estoque. Se alguma dessas etapas falhar, as etapas anteriores serão revertidas para garantir a consistência. Por exemplo, se o pagamento falhar, a reserva de itens é cancelada.

O padrão SAGA resolve o problema de manter a consistência em uma transação envolvendo várias etapas que podem ou não ser bem-sucedidas.

Aqui está outro diagrama de arquitetura de microsserviço para demonstrar como o padrão SAGA funciona:

<img width="720" height="417" alt="image" src="https://github.com/user-attachments/assets/51cfce29-2014-4fa3-ac2c-3ae632c04dd0" />

Prós e contras do padrão de design SAGA na arquitetura de microsserviços
Sempre que aprendemos um padrão, devemos aprender seus prós e contras, pois isso nos ajuda a entender melhor os padrões e também nos ajuda a decidir quando usá-los em seu aplicativo:

Aqui estão algumas vantagens e desvantagens do padrão SAGA no Microsserviço:

Vantagens: Aqui estão algumas vantagens de usar o padrão SAGA Design na arquitetura de microsserviços:

- É fácil implementar transações complexas em vários microsserviços.
- Lida com falhas normalmente e garante a consistência dos dados.
- Aumenta a resiliência e a robustez do sistema.
- Evita inconsistências de dados e atualizações perdidas.
- Fornece um processo claro e bem definido para compensar transações.

Desvantagens: Aqui estão algumas desvantagens de usar o padrão SAGA Design na arquitetura de microsserviços:

- É difícil de implementar e manter, também é difícil de monitorar e depurar
- Você terá a sobrecarga de armazenar e gerenciar o estado das sagas.
- Ele também vem com sobrecarga de desempenho devido à necessidade de gerenciar transações em vários microsserviços.
- Seu aplicativo também sofrerá com o aumento da latência devido à necessidade de várias viagens de ida e volta entre microsserviços.
- Não há padronização na implementação de sagas em diferentes microsserviços. Seria melhor se frameworks como Spring Cloud ou Quarks suportassem nativamente esse padrão no futuro.

Como implementar o padrão SAGA em uma arquitetura de microsserviço? O padrão SAGA pode ser implementado em uma arquitetura de microsserviços, dividindo uma transação de negócios complexa em várias etapas ou serviços menores e independentes.

1. Cada etapa se comunicaria com seu microsserviço correspondente para concluir uma parte da transação.
2. Se alguma etapa falhar, o sistema iniciará uma transação de compensação para desfazer as etapas anteriores.
3. A coordenação dessas etapas pode ser obtida usando um banco de dados, fila de mensagens ou serviço de coordenação para armazenar o estado da transação e disparar transações de compensação.

Dessa forma, o sistema pode garantir a consistência eventual e lidar com falhas normalmente.

Se você está se perguntando se algum framework Java Microservice pode fornecer suporte para o padrão SAGA? Então, infelizmente, não há uma estrutura de microsserviço específica que forneça suporte direto para o padrão SAGA.

No entanto, você pode implementar o SAGA Pattern usando bibliotecas e estruturas como Apache Camel ou Spring integration, juntamente com tecnologias como Apache Kafka, fornecimento de eventos e arquitetura orientada a mensagens.

<img width="720" height="432" alt="image" src="https://github.com/user-attachments/assets/c372f5d4-ab78-4967-a6ae-f29614797e28" />

Material de preparação para entrevistas Java e Spring - Antes de qualquer entrevista com desenvolvedores Java e Spring, eu sempre costumo ler os recursos abaixo:

> [!Important]
> Entrevista Grokking the Java. Eu pessoalmente comprei esses livros para acelerar minha preparação.

Atualmente, os sistemas são frequentemente distribuídos. Isso reflete a necessidade de extensibilidade, escalabilidade e resiliência. Engenheiros e arquitetos estão explorando mais estilos de arquitetura para alcançar esses objetivos. Microsserviços é uma opção. CQRS é outra. EDA também.

Em CQRS, precisamos de sincronização de consistência entre o modelo de leitura e o de escrita, usando um barramento de eventos e implementando um padrão de projeto observador. EDA busca a assincronia e a consistência eventual entre os componentes de um sistema. Em CQRS, precisamos implementar o padrão de coreografia SAGA para garantir a consistência eventual entre os modelos de leitura e escrita. Com EDA, é necessário fornecer um meio para que os componentes se comuniquem entre si. Quando um evento ocorre em um componente, ele é publicado para que outros componentes possam reagir a ele. Esse é o padrão de projeto observador.

## [Microservices] Service mesh
<img src="https://img.shields.io/badge/Istio-Service_mesh-blue?style=flat&logo=Istio&logoColor=white"> <img src="https://img.shields.io/badge/Consul-Service_mesh-magenta?style=flat&logo=Consul&logoColor=white"> <img src="https://img.shields.io/badge/Consul-Service_mesh-magenta?style=flat&logo=Consul&logoColor=white"> <img src="https://img.shields.io/badge/Linkerd-Service_mesh-limegreen?style=flat&logo=Linkerd&logoColor=white"> <img src="https://img.shields.io/badge/Kuma-Service_mesh-black?style=flat&logo=Kuma&logoColor=white">

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

![FB_IMG_1723734690810](https://github.com/user-attachments/assets/4544ca94-5d71-4307-a202-08ff86aa18ae)

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

## [Microservices] Event Sourcing
<a href=""><img src="https://img.shields.io/badge/dev.to-REST-0A0A0A?style=flat&logo=dev.to&logoColor=white"></a> <a href=""><img src="https://img.shields.io/badge/Medium-REST-000000?style=flat&logo=Medium&logoColor=white"></a> <img src="https://img.shields.io/badge/GitBook-REST-000000?style=flat&logo=GitBook&logoColor=white"> <a href="https://github.com/IsaacAlves7/js/blob/vanilla/README.md#js-axios"><img src="https://img.shields.io/badge/Axios-REST-purple?style=flat&logo=Axios&logoColor=white"></a> <img src="https://img.shields.io/badge/GraphQL-REST-magenta?style=flat&logo=GraphQL&logoColor=white"> <img src="https://img.shields.io/badge/Swagger-REST-85EA2D?style=flat&logo=Swagger&logoColor=white"> 

**Event Sourcing** é um padrão de arquitetura em que o estado de uma aplicação não é armazenado diretamente em estruturas de dados tradicionais, como tabelas com os dados finais atualizados, mas sim reconstruído a partir de uma sequência de eventos que descrevem tudo o que aconteceu com aquele dado ao longo do tempo. Em vez de gravar apenas o estado atual de uma entidade, cada mudança de estado é registrada como um evento imutável e persistido de forma sequencial. 

Você já pensou em implementar event sourcing? Pode ser aplicado de forma eficaz em aplicações do mundo real? Como ele se integra com outros padrões e abordagens, como Design Orientado por Domínio (DDD) ou Arquitetura Orientada a Eventos (EDA)? Se você tem curiosidade sobre essas perguntas, continue lendo; Vou compartilhar minhas percepções depois de mergulhar nesse padrão (incluindo código! Meu Deus!).

Um exemplo prático: A **Conta Bancária**, como pessoa pragmática, acho mais fácil entender conceitos teóricos usando exemplos do mundo real. Neste artigo, explicarei minha exploração do event sourcing usando um subdomínio de Conta Bancária em uma empresa financeira imaginária, um banco.

Por exemplo, em vez de simplesmente atualizar o saldo de uma conta bancária, o sistema registraria eventos como “depósito de 100”, “saque de 50”, “transferência de 200 recebida”, e assim por diante. O estado atual da conta pode ser reconstruído a qualquer momento aplicando essa sequência de eventos na ordem em que ocorreram.

Essa abordagem tem diversas vantagens. Ela garante uma trilha auditável de tudo que aconteceu no sistema, o que é extremamente útil para rastreabilidade, debugging e conformidade. Além disso, permite flexibilidade para construir diferentes projeções ou visualizações dos dados, já que os eventos podem ser reprocessados para gerar outras formas de representar o estado. Também facilita integrações com outras partes do sistema que queiram reagir a eventos, alimentando notificações, logs ou sincronizações com outras bases. Em sistemas altamente distribuídos, especialmente quando usados em conjunto com o padrão CQRS (Command Query Responsibility Segregation), o Event Sourcing se encaixa muito bem, pois separa claramente o que muda os dados (comandos e eventos) do que apenas os consulta (queries e projeções).

Por outro lado, Event Sourcing também traz complexidades. Como os eventos são imutáveis, qualquer mudança de lógica de negócio pode demandar a reinterpretação ou migração de eventos antigos, o que exige cuidado com versionamento de eventos. Além disso, reconstruir o estado de entidades pode se tornar custoso com muitos eventos, exigindo uso de snapshots intermediários. Apesar disso, em sistemas onde a rastreabilidade, auditabilidade e reatividade são prioridades, o Event Sourcing oferece um modelo poderoso e alinhado com a natureza temporal dos dados. Ele muda a forma de pensar o estado: não como algo fixo e mutável, mas como uma consequência acumulada de tudo que já aconteceu.

O diagrama abaixo mostra uma comparação entre o design de um sistema CRUD tradicional e o design de um sistema de Event Sourcing. Usamos um serviço de pedidos como exemplo:

![unnamed](https://github.com/user-attachments/assets/98eeaa26-a1cc-4671-84e6-02ee7df7b220)

O paradigma de Event Sourcing é usado para projetar um sistema com determinismo. Isso altera a filosofia dos projetos de sistemas tradicionais.

Como isso funciona? Em vez de registrar os estados dos pedidos no banco de dados, o design de Event Sourcing persiste os eventos que levam às mudanças de estado no repositório de eventos. O repositório de eventos é um log de somente acréscimo. Os eventos devem ser sequenciados com números incrementais para garantir sua ordem. Os estados dos pedidos podem ser reconstruídos a partir dos eventos e mantidos na OrderView. Se a OrderView estiver indisponível, podemos sempre contar com o repositório de eventos, que é a fonte da verdade, para recuperar os estados dos pedidos.

Vejamos os passos detalhados:

Sem Event Sourcing:

- Passos 1 e 2: Bob quer comprar um produto. O pedido é criado e inserido no banco de dados.
- Passos 3 e 4: Bob quer alterar a quantidade de 5 para 6. O pedido é modificado com um novo estado.

Com Event Sourcing:

- Passos 1 e 2: Bob quer comprar um produto. Um evento `NewOrderEvent` é criado, sequenciado e armazenado no repositório de eventos com `eventID=321`.
- Etapas 3 e 4: Bob deseja alterar a quantidade de 5 para 6. Um evento `ModifyOrderEvent` é criado, sequenciado e persistido no repositório de eventos com `eventID=322`.
- Etapa 5: A visualização do pedido é reconstruída a partir dos eventos do pedido, mostrando o estado mais recente de um pedido.

A maioria dos aplicativos opera com dados, e o método comum é o programa manter os dados em seu estado atual, atualizando-os quando os usuários interagem com eles. Na arquitetura clássica de criar, ler, atualizar e excluir (CRUD), por exemplo, uma operação típica de dados é receber dados do armazenamento, fazer algumas alterações neles e então atualizar o estado atual dos dados com os novos valores — muitas vezes utilizando transações que travam os dados.

O design de Event Sourcing define um método para lidar com atividades de dados que são acionadas por uma série de eventos, cada um dos quais é registrado em um armazenamento apenas de anexação. O código da aplicação entrega uma série de eventos para o armazenamento de eventos, onde eles são mantidos em manuse, que devem descrever cada ação que ocorreu nos dados. Cada evento descreve uma coleção de mudanças de dados (por exemplo, "`AddedItemToOrder`").

<img width="720" height="459" alt="image" src="https://github.com/user-attachments/assets/c82a6be2-9c44-4148-8715-14edfae6801e" />

Os eventos são salvos em um armazenamento de eventos, que serve como sistema de registro (a fonte oficial de dados) para o estado atual dos dados. Esses eventos geralmente são publicados pelo varejista para que os consumidores estejam cientes e possam lidar com eles, se necessário. Os consumidores podem, por exemplo, iniciar tarefas que aplicam as operações dos eventos a outros sistemas, ou podem executar qualquer outra ação associada necessária para concluir o processo. Vale notar que o código da aplicação que gera os eventos é separado dos sistemas que os subscrevem.

## [Microservices] Event-bus
<img src="https://em-content.zobj.net/source/microsoft-teams/400/bus_1f68c.png" align="right" height="77">

Um **event-bus** é um mecanismo de comunicação baseado em eventos que funciona como um canal central por onde diferentes partes de um sistema enviam e recebem mensagens sem depender diretamente umas das outras. Em vez de um componente chamar o outro de forma direta, criando acoplamento e dependências rígidas, tudo passa pelo barramento: um serviço “publica” um evento e qualquer outro serviço interessado “ouve” esse evento e reage a ele. Isso produz um fluxo muito mais solto, assíncrono e escalável, porque nada precisa saber quem vai consumir a informação; basta emitir o acontecimento e deixar o barramento cuidar da distribuição.

A função essencial do <a href="https://medium.com/@denhox/sharing-data-between-microservices-fe7fb9471208">event-bus</a> é organizar essa comunicação assíncrona. Ele recebe eventos — que podem representar mudanças de estado, ações do usuário, comunicação entre microsserviços ou notificações internas — e encaminha tudo para os assinantes corretos. Em sistemas distribuídos, isso significa que um backend pode emitir um evento de “pedido criado”, por exemplo, e vários serviços podem reagir de formas diferentes: um calcula frete, outro atualiza estoque, outro envia e-mail. Nada disso exige que esses serviços se conheçam diretamente, porque o event-bus faz o papel de conector invisível entre todos eles.

Esse padrão é muito usado em arquiteturas orientadas a eventos, tanto em front-ends modernos quanto em plataformas de mensageria robustas. No contexto de aplicações JavaScript, por exemplo, um event-bus interno organiza a comunicação entre componentes sem que eles precisem se referenciar diretamente. Já no universo de microservices, o event-bus costuma ser implementado por ferramentas como RabbitMQ, Kafka, NATS ou SNS/SQS na AWS, que lidam com volume alto, tolerância a falhas, filas persistentes e distribuição confiável.

O event-bus não serve apenas para transportar mensagens; ele também cria uma forma mais saudável de estruturar a arquitetura, reduzindo acoplamento, aumentando testabilidade e facilitando evolução do sistema. Quando tudo gira em torno de eventos, o software passa a ser mais rastreável, auditar o comportamento fica simples, e é possível introduzir novas funcionalidades observando apenas os eventos existentes, sem tocar no código dos serviços que já funcionam. Em essência, o event-bus é o coração silencioso de sistemas modernos baseados em reatividade e comunicação assíncrona, garantindo fluidez, escalabilidade e clareza no fluxo de informações.

Um event-bus *não é um microsserviço em si*, mas *é um padrão arquitetural amplamente usado em microsserviços*. Ou seja, ele não é um “tipo de microsserviço”, mas um **mecanismo** que serve como base para arquiteturas orientadas a eventos dentro de um ecossistema distribuído.

Quando falamos de microsserviços, existem alguns padrões clássicos: API Gateway, Saga, CQRS, Event Sourcing, Backend for Frontend, Sidecar, entre outros. O event-bus se encaixa nessa família como um padrão de **mensageria** e **comunicação assíncrona**, funcionando como a “infraestrutura” que permite que os microsserviços troquem informações sem ficarem acoplados.

Em microsserviços, o event-bus ajuda a resolver problemas como dependência direta entre serviços, necessidade de sincronização e dificuldade de escalar fluxos de comunicação. Ele atua como o mediador central por onde todos os eventos passam, garantindo que cada serviço possa emitir informações e reagir apenas ao que lhe interessa. Isso torna a arquitetura mais tolerante a falhas, mais observável e mais fácil de evoluir.

Em resumo, o event-bus faz parte dos padrões fundamentais que sustentam uma arquitetura moderna de microsserviços, mas ele mesmo não é um serviço; é a **espinha dorsal de comunicação assíncrona** que permite que todo o ecossistema funcione com independência e baixo acoplamento.

<img src="https://em-content.zobj.net/source/microsoft-teams/400/oncoming-bus_1f68d.png" align="right" height="77">

Quando comecei a trabalhar com microsserviços, levei a regra comum de "dois serviços não devem compartilhar uma fonte de dados" um pouco literalmente.

Eu vi isso grampeado em todos os lugares da internet: "não compartilharás um banco de dados entre dois serviços", e definitivamente fazia sentido. Um serviço deve possuir seus dados e manter a liberdade de alterar seu esquema como quiser, sem alterar sua API externa.

Mas há uma sutileza importante aqui que eu não entendi até muito mais tarde. Para aplicar essa regra corretamente, temos que distinguir entre compartilhar uma fonte de dados e compartilhar dados.

Por que compartilhar uma fonte de dados é ruim: Um exemplo: o serviço Produtos deve ser o proprietário da tabela e de todos os registros nela. Eles expõem esses dados a outras equipes por meio de uma API, uma consulta GraphQL e a criação desses registros por meio de uma `mutation.products products createProduct`

O serviço de Produtos tem propriedade sobre a fonte de verdade dos produtos, e nenhuma outra equipe deve entrar em contato diretamente com isso, nunca. Se eles quiserem dados fora dele, eles devem solicitar ao serviço de Produtos por meio do contrato (API) ao qual aderem. Sob nenhuma circunstância você deve permitir acesso direto ao banco de dados ou perderá a liberdade de fazer alterações em seu esquema. Aprendi isso da maneira mais difícil.

Compartilhar dados está OK. O fato é que os serviços precisam de dados que pertencem a outros serviços.

Por exemplo, um serviço de Viagem (`Trip` service) precisará de acesso a passageiros (do Serviço de Passageiros) e motoristas (do Serviço de Motorista) para fornecer visões gerais de viagens.

<img width="720" height="302" alt="image" src="https://github.com/user-attachments/assets/dba44127-9ac4-4cf4-9370-a548123c869a" />

O serviço de viagem solicita a cada serviço respectivo seus dados, de forma síncrona, para atender à solicitação original `request ()`. Podemos ter certeza de que os dados são atualizados e o cliente solicitante terá uma visão fortemente consistente dos dados (alguns de vocês podem ver para onde estou indo neste momento ;). `getTrips`

Esse modelo síncrono de solicitação/resposta para transmitir dados entre microsserviços é um modelo mental muito natural para equipes que começam em microsserviços, pelo menos na minha experiência. Você precisa de alguns dados, sabe onde obtê-los, pede ao serviço proprietário e ele fornece os dados para você, sob demanda.

Além disso, fornecer dados novos e fortemente consistentes foi um acéfalo para as equipes em que eu estava. Dados fortemente consistentes significam dados atualizados, os dados "mais recentes" absolutos, direto da fonte (da verdade). Para mim, naquela época, servir qualquer coisa que não fosse dados consistentes era inaceitável. Como você poderia servir outra coisa além de dados atualizados? Qualquer outra coisa seria uma mentira!

Aplicamos esses padrões como dogma porque não víamos outra maneira e, acima de tudo, parecia natural.

Sincronicidade e consistência forte não escalam. Arquiteturas que dependem muito de solicitações síncronas e consistência forte não são bem dimensionadas. Às vezes, simplesmente não é viável, ou estritamente necessário, sempre ir direto à fonte para suas necessidades de dados.

O exemplo de serviço Trips acima parece legal no início, mas raramente os sistemas permanecem tão simples. Novos serviços nascem e exigirão dados dos serviços existentes. Aderir ao padrão de solicitação síncrona, com o tempo, fará com que você acabe com uma teia emaranhada de solicitações entre serviços. Aqui está um cenário:

<img height="718" align="right" src="https://github.com/user-attachments/assets/07b93673-020b-4d22-b3e6-3ae98c911904" />

Exemplo de fluxo com solicitações síncronas:

1. Um usuário concluiu um desafio, executa uma mutação no serviço `ChallengecompleteChallenge`
2. Depois de armazenar a conclusão, o serviço Desafio informa o serviço `Leaderboard`, para que ele possa atualizar o `leaderboard`
3. O serviço `Leaderboard` solicita ao serviço de usuário nomes de exibição e avatares do usuário para criar o novo estado do placar
4. O serviço de Classificação vê que há um novo líder no novo estado da tabela de classificação e permite que o serviço de Notificação saiba para que ele possa notificar os participantes de que há um novo líder!
5. O serviço de notificação solicita ao serviço do usuário os endereços de e-mail atualizados dos usuários nesse placar específico, para que ele possa enviar e-mails

O serviço ao usuário é claramente um ponto de discórdia aqui: todos dependem de uma forma ou de outra dele. Imagine que este serviço esteja fora do ar: ele também desativará a maioria dos outros serviços. Não apenas isso, mas você terá que manter este servidor aprimorado o tempo todo com mais réplicas e um banco de dados de alto desempenho para acompanhar a demanda.

Além disso, cada salto nessa cadeia de solicitações adiciona latência a toda a solicitação. Cada salto tem o potencial de adicionar uma quantidade exponencial de latência porque cada serviço na cadeia de dependências pode disparar mais de uma solicitação para suas próprias dependências. Antes que você perceba, você atingiu níveis insuportáveis de latência.

Por fim, cada dependência adicional na cadeia de solicitações aumenta a probabilidade de falha de toda a cadeia de solicitações. Em uma cadeia de solicitações envolvendo cinco serviços com um SLA de 99,9% (~9h de tempo de inatividade anual), o SLA composto se torna 99,5%. São quase 2 dias de inatividade por ano!

Podemos evitar todas essas desvantagens fazendo uma pergunta: os serviços realmente precisam de dados atualizados?

O serviço de notificação (etapa 5) provavelmente faz. Se um usuário alterar seu endereço e o serviço de notificação não souber, correrá o risco de enviar um e-mail para o endereço errado e não receber a notificação para o usuário pretendido.

O serviço `Leaderboard`, por outro lado, provavelmente não precisa de nomes de exibição e avatares atualizados para construir a tabela de classificação - não é grande coisa se os usuários virem avatares ou nomes de exibição obsoletos.

Como você pode ver, os serviços têm diferentes necessidades de consistência de dados. Existem compensações que podemos usar como alavanca para aplicar diferentes métodos de compartilhamento de dados e construir um sistema distribuído mais robusto.

Insira a consistência eventual. Foi nesse ponto da minha carreira que descobri que os serviços podem manter uma cópia dos dados de outros serviços, localmente em suas próprias tabelas de banco de dados. Ele vem com a responsabilidade de reter esses dados por meio de eventos ou pesquisas.

Incluído neste pacote está o fato de que os dados podem ficar obsoletos por algum tempo, mas que eventualmente serão atualizados, o que significa que os dados são eventualmente consistentes. Não podemos garantir que os dados não estejam obsoletos, mas podemos garantir que eventualmente nos atualizaremos.

O momento em que "clicou" para mim foi quando pensei nisso da perspectiva de um serviço de back-end que depende de uma API meteorológica pública para dados meteorológicos. Em vez de recuperar dados meteorológicos de Pristina ou Berlim toda vez que um usuário dessas respectivas cidades precisa de dados meteorológicos, eu os armazeno em cache (talvez várias vezes ao dia) materializando-os em uma tabela local e servindo dados em cache para esses usuários. Fiz a troca em favor da consistência eventual porque não é crucial para meus usuários ver os dados mais recentes, tudo bem se estiverem algumas horas obsoletos.

Voltando ao exemplo do Desafio: podemos cortar muitas dependências síncronas para o serviço do usuário apenas mantendo uma cópia local dos usuários nos serviços:

- O serviço de placar pode manter uma cópia local dos usuários e evitar a necessidade de fazer solicitações ao serviço do usuário. Ninguém realmente se importa se os dados são um pouco antigos, não é um empecilho se alguém vir um avatar um pouco antigo.
- O serviço de desafio pode fazer o mesmo; digamos que se ele expôs uma consulta e precisou de nomes de exibição e avatares de usuário para mostrar os participantes atuais do desafio - ele também pode fornecer esses dados eventualmente consistentes de sua própria tabela de usuários materializados.getChallengeDetails
- O serviço de notificação, embora um pouco mais sensível, também pode utilizar o compartilhamento de dados para remover sua dependência do serviço Usuários. Ele pode materializar os usuários localmente e manter um estado atualizado de melhor esforço ouvindo os eventos atualizados pelo usuário para garantir que ele tenha os e-mails mais atualizados.

Embora não tenhamos falado muito sobre como os serviços compartilham esses dados (um tópico para outra hora), uma arquitetura de exemplo final usaria uma combinação de fornecimento de eventos e armazenamento em cache. Aqui está uma prévia de como seria esse tipo de arquitetura:

<img width="720" height="506" alt="image" src="https://github.com/user-attachments/assets/f07ad644-4980-4a1e-aa07-6b6832966822" />

Exemplo de arquitetura com dois métodos principais de compartilhamento de dados entre serviços: fornecimento de eventos e cache

Se você quiser mais exemplos, dê uma olhada em Como compartilhar dados entre microsserviços em alta escala por Shiran Metsuyanim, engenheiro da Fiverr. É um ótimo post que mostra como manter a robustez ao adicionar um novo serviço. Ele começa estabelecendo as restrições e, em seguida, discutindo as compensações entre soluções síncronas, assíncronas e híbridas.

Conclusão, eu queria transmitir esse ponto aos desenvolvedores que, como eu há alguns anos, estão presos no sentido literal de "não compartilhe dados", mas devem perceber que isso só se aplica a não compartilhar a fonte da verdade. Manter uma cópia dos dados de um serviço no domínio de outro serviço é perfeitamente aceitável e abrange o espírito de consistência eventual.

## [Microservices] EDA - Event-Driven Architecture
<a href="http://tryrabbitmq.com/"><img src="https://img.shields.io/badge/RabbitMQ-16.17.0-orange?style=flat&logo=RabbitMQ&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/RabbitMQ-16.17.0-orange?style=flat&logo=Medium&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/Apache_Kafka-16.17.0-black?style=flat&logo=Apache-Kafka&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/Apache_Kafka-16.17.0-black?style=flat&logo=Apache-Kafka&logoColor=white"></a> <a href="https://medium.com/innoviletech/rabbitmq-producer-and-consumer-solution-with-docker-in-net-core-9a825d3c2448"><img src="https://img.shields.io/badge/Apache_Kafka-16.17.0-black?style=flat&logo=Apache-Kafka&logoColor=white"></a>

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/99011c9e-9092-45d4-9487-e3bdb7346352" align="right" height="277">

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

**Event-Based Architecture** é frequentemente usada como sinônimo de Event-Driven Architecture. Quando alguém se refere a uma arquitetura baseada em eventos, geralmente está falando de um sistema onde os eventos desempenham um papel central na comunicação e no controle do fluxo de trabalho, com características semelhantes às descritas na EDA.

As diferenças sutis, se houverem, se for necessário fazer uma distinção técnica entre Event-Based e Event-Driven, pode-se considerar:

- Event-Based pode ser uma descrição mais ampla que inclui qualquer sistema que use eventos como parte de sua lógica, sem necessariamente seguir todos os princípios de uma arquitetura Event-Driven, como desacoplamento rigoroso e comunicação assíncrona.

- Event-Driven implica um conjunto mais específico de princípios e práticas que promovem a reatividade, a escalabilidade e o desacoplamento através do uso de eventos.

Um **Event-bus**, ou barramento de eventos, é um padrão de arquitetura de software usado para facilitar a comunicação assíncrona entre diferentes partes de um sistema distribuído. Ele permite que os componentes do sistema comuniquem-se entre si sem ter conhecimento direto uns dos outros.

Basicamente, um Event-bus atua como um intermediário entre os vários componentes de um sistema, permitindo que eles publiquem eventos (mensagens, notificações, atualizações etc.) e se inscrevam para receber eventos específicos que são relevantes para eles.

Existem dois tipos principais de Event-bus:

- Event-bus baseado em mensagens: Neste tipo, os componentes enviam e recebem mensagens assíncronas através de um barramento centralizado. Cada componente pode ser um produtor (enviando eventos) ou um consumidor (recebendo eventos). Exemplos populares incluem Apache Kafka, RabbitMQ e ActiveMQ.

- Event-bus baseado em publish/subscribe (publicar/inscrever-se): Aqui, os componentes publicam eventos em "tópicos" específicos e outros componentes se inscrevem nos tópicos relevantes para receber esses eventos. Quando um evento é publicado em um tópico, todos os assinantes desse tópico recebem o evento. Exemplos incluem o uso de sistemas de mensagens como MQTT ou tecnologias como Redis Pub/Sub.

O Event-bus é amplamente utilizado em arquiteturas de microsserviços, sistemas distribuídos e ambientes orientados a eventos, pois oferece flexibilidade, escalabilidade e desacopla os componentes do sistema, permitindo que eles evoluam independentemente.

Ao adotar um Event-bus, é essencial planejar cuidadosamente os eventos que serão enviados e recebidos, garantir a confiabilidade na entrega de mensagens e considerar a escalabilidade e o desempenho do sistema como um todo.

https://medium.com/@vinciabhinav7/common-problems-in-message-queues-with-solutions-f0703c0bd5af

## [Microservices] Outbox Pattern
<a href="https://medium.com/@praveengaddam319/the-outbox-pattern-explained-how-spring-boot-microservices-avoid-data-inconsistenc-b868dcb48a18"><img height="177" align="right" src="https://github.com/user-attachments/assets/ea001cdf-436e-41ce-a04c-cb74872359bc" /></a>

Simplesmente, quando sua API publica mensagens de evento, ela não as envia diretamente. Em vez disso, as mensagens são mantidas em uma tabela de banco de dados. Depois disso, um trabalho publica eventos no sistema do agente de mensagens em intervalos de tempo predefinidos.

Basicamente, o padrão de caixa de saída (**Outbox Pattern**) fornece a publicação de eventos de forma confiável. A ideia dessa abordagem é ter uma tabela "Caixa de saída" no banco de dados do microsserviço.

Nesse método, os eventos de domínio não são gravados diretamente em um barramento de eventos. Em vez disso, ele é gravado em uma tabela na função "caixa de saída" do serviço que armazena o evento em seu próprio banco de dados.

No entanto, o ponto crítico aqui é que a transação executada antes do evento e o evento gravado na tabela da caixa de saída fazem parte da mesma transação.

<img width="700" height="361" alt="image" src="https://github.com/user-attachments/assets/19fdca78-5dcd-4192-9365-93005db42742" />

Por exemplo, quando um novo produto é adicionado ao sistema, o processo de adicionar o produto e gravar o evento ProductCreated na tabela da caixa de saída é feito na mesma transação, garantindo que o evento seja salvo no banco de dados.

A segunda etapa é receber esses eventos gravados na tabela de caixa de saída por um serviço independente e gravá-los no barramento de eventos.

Como você pode ver na imagem acima, o serviço Order executa suas operações de caso de uso e atualiza sua própria tabela e, em vez de publicar um evento, ele escreve outra tabela com esse registro de evento e esse evento é lido de outro serviço e publica um evento.

Por que usamos este padrão de caixa de saída? Se você estiver trabalhando com dados críticos que precisam ser consistentes e precisos para capturar todas as solicitações, é bom usar o padrão Caixa de saída. Se no seu caso, a atualização do banco de dados e o envio da mensagem devem ser atômicos para garantir a consistência dos dados, é bom usar o padrão de caixa de saída.

Por exemplo, as transações de venda de pedidos, já está claro o quão importantes são esses dados. Porque eles são sobre negócios financeiros. Assim, os cálculos devem estar 100% corretos. Para poder acessar essa precisão, devemos ter certeza de que nosso sistema não está perdendo nenhuma mensagem de evento. Portanto, o padrão de caixa de saída deve ser aplicado neste tipo de casos.

Portanto, devemos evoluir nossa arquitetura com a aplicação de outros padrões de dados de microsserviços para acomodar adaptações de negócios, tempo de lançamento no mercado mais rápido e lidar com solicitações maiores.

## [Microservices] Streaming
O **streaming** é um dos padrões (patterns) usados em arquiteturas de microservices. É particularmente útil para cenários onde os dados precisam ser processados em tempo real ou quase real, permitindo uma comunicação eficiente e contínua entre serviços. O streaming é um padrão fundamental em arquiteturas de microservices, especialmente útil para casos que exigem processamento de dados em tempo real, baixa latência e alta escalabilidade. Ao utilizar sistemas de mensageria e plataformas de streaming de eventos, é possível construir sistemas reativos, escaláveis e resilientes, capazes de lidar com grandes volumes de dados e alta taxa de eventos de maneira eficiente.

Padrões de Streaming em Microservices:

1. **Event Streaming**: Serviços produzem eventos que são transmitidos para outros serviços em tempo real. Isso é frequentemente implementado usando sistemas de mensageria ou de streaming de eventos como Apache Kafka, RabbitMQ, ou Amazon Kinesis. Casos de Uso: Monitoramento em tempo real, análise de dados em tempo real, atualização de caches distribuídos, etc.

2. **Data Streaming**: Dados são continuamente transmitidos entre serviços. Pode envolver a transmissão de grandes volumes de dados de forma eficiente, dividindo-os em pequenos chunks. Casos de Uso: Streaming de mídia (vídeo, áudio), sincronização de bases de dados, processamento contínuo de dados de sensores IoT.

Vantagens do Streaming em Microservices:

- **Baixa Latência**: Permite a comunicação em tempo real, essencial para aplicações que exigem respostas rápidas.
- **Escalabilidade**: Facilita a escalabilidade horizontal, permitindo que diferentes partes do sistema processem fluxos de dados em paralelo.
- **Desacoplamento**: Promove o desacoplamento entre serviços, onde produtores e consumidores de eventos/dados não precisam estar diretamente conectados.

Ferramentas Comuns para Streaming:

- **Apache Kafka**: Uma plataforma distribuída de streaming de eventos que permite a publicação e assinatura de fluxos de registros, armazenamento de fluxos de registros de maneira tolerante a falhas e processamento de fluxos de registros em tempo real.
- **RabbitMQ**: Um broker de mensagens que suporta a transmissão de mensagens de forma confiável entre produtores e consumidores.
- **Amazon Kinesis**: Uma plataforma gerenciada para streaming de dados em tempo real na AWS.
- **Apache Flink e Apache Spark Streaming**: Ferramentas para processamento de fluxos de dados em tempo real, permitindo a análise e transformação de dados em movimento.

Exemplos de Padrões de Streaming em Microservices:

1. **Log Aggregation**: Coletar logs de diferentes serviços e transmiti-los para um serviço central para armazenamento e análise. **Ferramenta Comum**: Apache Kafka.

2. **Event Sourcing**: Armazenar o estado do sistema como uma sequência de eventos. Cada mudança no estado gera um novo evento que é transmitido. **Ferramenta Comum**: Event Store, Apache Kafka.

3. **CQRS (Command Query Responsibility Segregation) com Streaming**: Usar um modelo separado para comandos (escrita) e consultas (leitura), onde as mudanças são propagadas através de eventos transmitidos para diferentes modelos de leitura. **Ferramenta Comum**: Apache Kafka, RabbitMQ.

4. **Real-Time Analytics**: Processamento contínuo de dados para gerar insights e análises em tempo real. **Ferramenta Comum**: Apache Flink, Apache Spark Streaming.

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

![FB_IMG_1729173505724](https://github.com/user-attachments/assets/e99a84c7-247d-4559-a6f8-ca605e51db89)

![FB_IMG_1724073369311](https://github.com/user-attachments/assets/9ce31510-ba4c-4427-b597-bd3955719a4a)

## [Microservices] Circuit breaker
<img src="https://img.shields.io/badge/Medium-Circuit_Breaker-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Circuit_Breaker-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Circuit_Breaker-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Circuit_Breaker-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/DEV-Circuit_Breaker-blue?style=flat&logo=dev.to&logoColor=white"> <img src="https://img.shields.io/badge/GitBook-Circuit_Breaker-blue?style=flat&logo=GitBook&logoColor=white">

<img src="https://github.com/user-attachments/assets/bc7a8876-5d7e-4759-b3dc-086a27936c25" height="177" align="right">

**Circuit breaker**, ou disjuntor em português, é um padrão de design utilizado em sistemas distribuídos, principalmente em arquiteturas baseadas em microserviços, para lidar com falhas temporárias e evitar sobrecargas em serviços instáveis ou fora do ar. A ideia central é inspirada nos disjuntores elétricos: quando um circuito apresenta falha ou sobrecarga, o disjuntor desarma para impedir danos maiores; da mesma forma, em software, o circuit breaker monitora chamadas remotas e, ao detectar uma quantidade excessiva de falhas consecutivas, ele "abre" o circuito, interrompendo temporariamente as tentativas de comunicação com o serviço problemático. Padrão de disjuntor: proteja seus microsserviços contra falhas em cascata.

Inspirando-se nos disjuntores elétricos, em sistemas de software, objetos disjuntores funcionam de forma semelhante, interrompendo automaticamente o fluxo de solicitações quando anomalias são detectadas. Ele está situado entre o atendimento e o serviço de chamada.
O disjuntor 'desliga' quando o interlocutor não está disponível. Esse mecanismo não só previne danos adicionais, mas também permite que o tempo de falha se recupere.

Enquanto o circuito está aberto, as tentativas de acesso ao serviço são bloqueadas de imediato, evitando que a aplicação continue enviando requisições inúteis que só iriam falhar e consumir recursos preciosos. Após um intervalo de tempo pré-definido (geralmente chamado de timeout), o circuito entra em estado de teste (half-open), permitindo algumas chamadas para verificar se o serviço voltou ao normal. Se as tentativas forem bem-sucedidas, o circuito é fechado e o serviço volta a receber tráfego normalmente. Se falhar novamente, o circuito permanece aberto, protegendo o sistema de novos colapsos.

Esse padrão é fundamental para manter a resiliência e a estabilidade de sistemas que dependem de muitos serviços externos ou internos, especialmente em contextos onde a indisponibilidade de um componente pode provocar efeito cascata, travando partes críticas da aplicação. O circuit breaker ajuda a degradar o sistema de forma controlada, oferecendo respostas rápidas de fallback ao invés de deixar os usuários esperando por tempo de resposta indefinido.

Na arquitetura de microserviços, comunicar-se por meio de chamadas remotas de procedimentos e dependências de API a jusante introduz uma camada de complexidade onde erros transitórios podem ocorrer devido a problemas de rede ou o serviço pode falhar por qualquer motivo, como interrupção de rede, sobrecarga do sistema, travamento, etc.

Nessa situação, é muito importante desconectar os componentes/serviços que estão falhando e não solicitar mais informações sabendo que estão falhando no momento, permitindo que o sistema se recupere. Um componente de disjuntor pode facilmente desconectar serviços que falharam a jusante.

1. **O fracasso que não ficou contido**: Começou, como essas coisas costumam acontecer, com um gráfico um pouco estranho. Um serviço a jusante foi mais lento que o normal — não foi para baixo, apenas lento. Nenhum alerta disparado. As taxas de erro estavam boas. Mas em poucos minutos, os painéis de serviços não relacionados começaram a ficar âmbar, depois vermelhos. Latências aumentaram lentamente. Piscinas de fios preenchidas. Tentativas se acumulavam sobre chamadas já lentas. De repente, o problema não era mais aquele serviço — era tudo.

O que tornava tudo doloroso em retrospecto era o quão previsível era. Nada exótico falhou. Sem falha no data center. Apenas uma dependência sendo lenta, permitida continuar prejudicando seus chamadores. Este artigo não é sobre prevenir falhas completamente. É sobre contê-los. Disjuntores não são uma solução mágica. Eles são uma forma de impedir que uma interação ruim arraste uma plataforma inteira para baixo.

![1_2MQxm46MrcgLVZ37g2rmXQ](https://github.com/user-attachments/assets/e7daddf3-64a2-4427-a4a7-985202917205)

2. **Como as falhas em cascata realmente acontecem**: A maioria das falhas em cascata não é misteriosa. Eles são mecânicos.

Imagine uma cadeia simples: `Serviço A → Serviço B → Serviço C`

O serviço C desacelera — talvez um problema no banco de dados, talvez pressão do GC. O serviço B chama C sincronizadamente, espera

<img src="https://github.com/user-attachments/assets/f997bedf-6422-4006-b83b-5510cd07430f" align="right" height="177">

> [!Important]
> O livro de Michael Nygard, <a href="https://pragprog.com/titles/mnee2/release-it-second-edition/">Release It!</a>, popularizou o padrão Circuit Breaker, que pode impedir que um aplicativo tente executar continuamente uma ação que provavelmente falhará, permitindo que ele prossiga sem esperar a correção do problema ou gastar ciclos de CPU para determinar a duração da falha. “Release It! – Second Edition”, do Michael T. Nygard, é um dos livros mais importantes sobre como projetar, construir e operar sistemas realmente prontos para produção. O tema central não é apenas código, mas como softwares se comportam no mundo real, onde falhas acontecem, tráfego cresce inesperadamente, dependências externas quebram e a infraestrutura reage de formas imprevisíveis.

O padrão de disjuntor também permite que a aplicação determine se o problema foi resolvido ou não. Se o problema parecer resolvido, o programa pode tentar realizar a operação.

> O padrão Disjuntor serve a um propósito distinto do padrão Retry. O padrão Retry permite que uma aplicação tente novamente uma operação na esperança de que ela tenha sucesso na próxima vez.

O design do Disjuntor proíbe que uma aplicação realize uma atividade de risco. Uma aplicação pode usar o padrão Retry para acionar uma ação através de um disjuntor e combinar esses dois padrões. A lógica de retentativa, por outro lado, deve estar alerta para quaisquer exceções fornecidas pelo disjuntor e deve cessar as tentativas repetidas se o disjuntor indicar que a falha não é temporária.

<img width="651" height="539" alt="image" src="https://github.com/user-attachments/assets/29d5340b-0957-4702-aab7-1f5ebb1b3e2e" />

Ferramentas como **Hystrix** (da Netflix), **Resilience4j**, **Polly** (para .NET) e algumas implementações no Spring Cloud oferecem suporte a esse padrão, muitas vezes combinando com retries, timeouts e mecanismos de fallback para formar uma estratégia robusta de tolerância a falhas. Em suma, o circuit breaker permite que aplicações sobrevivam em ambientes imprevisíveis, garantindo que uma falha localizada não se torne um problema sistêmico.

Você está preocupado com o efeito cascata de falhas em sua arquitetura de microsserviços? Conheça o padrão de disjuntor - sua proteção definitiva contra falhas em cascata. Esse padrão monitora falhas e impede que as solicitações cheguem a um serviço com falha, dando tempo para se recuperar e protegendo todo o sistema contra colapso.

Por que você deve implementar o padrão de disjuntor? Em um ecossistema de microsserviços, um único serviço com defeito pode causar um efeito dominó, interrompendo outros serviços que dependem dele. Ao usar disjuntores, você pode isolar o serviço defeituoso e evitar mais danos, garantindo a resiliência e a estabilidade do seu sistema.

Os disjuntores podem ser facilmente implementados usando bibliotecas como Netflix, Hystrix e Resilience4j. Essas bibliotecas oferecem uma variedade de recursos, como métodos de fallback e monitoramento, para ajudá-lo a gerenciar e se recuperar de falhas com eficiência.

Em essência, o padrão de disjuntor é essencial para a criação de microsserviços resilientes e tolerantes a falhas. Ao incorporar esse padrão em sua arquitetura, você pode efetivamente proteger seu sistema contra os efeitos adversos de falhas de serviço. Você está pronto para fortalecer seus microsserviços com o padrão de disjuntor?

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

## [Microservices] Onion architecture
<img src="https://em-content.zobj.net/source/microsoft-teams/400/onion_1f9c5.png" align="right" height="77">

**Onion Architecture** é um padrão de design de software e foi introduzido por Jeffrey Palermo em 2008 como uma alternativa para abordar algumas das limitações e problemas de outras arquiteturas tradicionais, como a arquitetura em camadas. A Onion Architecture promove uma maior separação de preocupações e independência das dependências externas, como frameworks e bibliotecas. 

A Onion Architecture é um poderoso padrão de design que promove a separação de preocupações e a independência de tecnologia, facilitando a criação de sistemas mais flexíveis, testáveis e manuteníveis. Ela é especialmente útil em ambientes de desenvolvimento complexos e de rápida mudança, onde a capacidade de adaptar e evoluir o sistema é crucial.

A arquitetura Onion pode ser utilizada em uma arquitetura de microsserviços. Na verdade, muitos dos princípios da Onion Architecture se alinham bem com os objetivos e práticas de desenvolvimento de microsserviços. A Onion Architecture pode ser uma abordagem eficaz para estruturar microsserviços, promovendo um design desacoplado, testável e fácil de manter. Ao aplicar os princípios da Onion Architecture, cada microsserviço pode ser desenvolvido de forma independente, mantendo a lógica de negócios centralizada e livre de dependências externas desnecessárias.

Principais Conceitos da Onion Architecture:

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/ddc4a9ac-7547-47d0-a56e-c964c8fb38a8" height="377" align="right">

1. **Camadas Concêntricas**: A arquitetura é visualizada como um conjunto de camadas concêntricas, onde cada camada depende apenas das camadas mais internas, nunca das camadas externas. As dependências fluem para dentro, não para fora.

2. **Domínio no Centro**: O núcleo da arquitetura é o domínio. Isso inclui as entidades de negócio e as regras de negócio. O domínio é completamente independente de detalhes externos como bancos de dados, interfaces de usuário ou serviços.

3. **Independência de Tecnologia**: Detalhes de implementação, como frameworks de persistência, interfaces de usuário e outros serviços externos, são mantidos nas camadas mais externas, permitindo que a lógica de negócio permaneça livre de dependências técnicas.

Estrutura da Onion Architecture:

1. **Camada de Domínio (Core)**:
   - **Entidades**: Classes que representam o modelo de domínio e encapsulam as regras de negócio.
   - **Serviços de Domínio**: Serviços que contêm lógica de negócio que não pertence a nenhuma entidade específica.

2. **Camada de Aplicação**: **Casos de Uso**: Contém a lógica de aplicação que orquestra o uso das entidades de domínio para atender a um caso de uso específico. Não contém lógica de negócio em si, mas coordena operações entre diferentes partes do domínio.

3. **Camada de Interface (Application Interfaces)**: **Interfaces**: Define contratos (interfaces) para serviços externos, como repositórios de dados, serviços de mensagem, etc. As implementações dessas interfaces ficam em uma camada ainda mais externa.

4. **Camada de Infraestrutura**: **Implementações**: Contém as implementações reais das interfaces definidas na camada de aplicação. Isso inclui detalhes específicos de tecnologia, como acesso a banco de dados, serviços de mensageria, etc.

Benefícios da Onion Architecture:

1. **Desacoplamento**: Permite que a lógica de negócio seja desacoplada de detalhes técnicos e frameworks, tornando o sistema mais flexível e testável.

2. **Testabilidade**: As camadas internas (domínio e aplicação) podem ser testadas isoladamente sem a necessidade de dependências externas, facilitando a escrita de testes unitários.

3. **Manutenibilidade**: Com uma separação clara de responsabilidades, a manutenção do código se torna mais fácil, pois as mudanças em uma camada (por exemplo, detalhes de acesso a dados) não afetam outras camadas (como a lógica de negócio).

Comparação com Outras Arquiteturas:

- **Arquitetura em Camadas (Layered Architecture)**: Embora a arquitetura em camadas também tenha uma separação de preocupações, ela não impõe a mesma direção de dependência. Em uma arquitetura em camadas tradicional, a camada de apresentação pode ter dependências diretas na camada de persistência, o que não é o caso na Onion Architecture.

- **Arquitetura Hexagonal (Ports and Adapters)**: Muito semelhante à Onion Architecture, a arquitetura hexagonal também promove a separação de lógica de negócio das dependências externas. A principal diferença é na terminologia e na ênfase no uso de "portas" e "adaptadores" para representar interfaces e implementações externas.

Exemplo de Implementação: Suponha um sistema de gerenciamento de pedidos:

- **Domínio**:
  - **Entidade Pedido**: Representa um pedido com propriedades como ID, lista de itens, status, etc.
  - **Serviço de Domínio PedidoService**: Contém lógica de negócio, como criação de pedidos, cancelamento, etc.

- **Aplicação**:
  - **Caso de Uso CriarPedidoUseCase**: Orquestra a criação de um pedido, utilizando as entidades e serviços do domínio.

- **Interfaces**:
  - **PedidoRepository**: Interface para persistência de pedidos.
  - **NotificacaoService**: Interface para envio de notificações.

- **Infraestrutura**:
  - **PedidoRepositoryImpl**: Implementação do repositório utilizando um banco de dados específico.
  - **NotificacaoServiceImpl**: Implementação do serviço de notificação utilizando um serviço de e-mail externo.

## [Microservices] Clean architecture
<img src="https://img.shields.io/badge/Python-3.10.7-3776AB?style=flat&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-339933?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/Ruby-3.3-CC342D?style=flat&logo=Ruby&logoColor=white"> <img src="https://img.shields.io/badge/Go-1.21-00ADD8?style=flat&logo=Go&logoColor=white"> <img src="https://img.shields.io/badge/PHP-8.2-777BB4?style=flat&logo=PHP&logoColor=white"> <img src="https://img.shields.io/badge/C++-23-F5455C?style=flat&logo=CPlusPlus&logoColor=white"> <img src="https://img.shields.io/badge/Java-22.0.1-chocolate?style=flat&logo=OpenJDK&logoColor=white"> <img src="https://img.shields.io/badge/.NET-8.0.300-512BD4?style=flat&logo=DotNet&logoColor=white"> <img src="https://img.shields.io/badge/Rust-1.82.0-dda584?style=flat&logo=Rust&logoColor=white"> 

A **Arquitetura limpa** (Clean Architecture) é um conjunto de princípios e práticas que buscam organizar o código de uma aplicação de forma que ela seja sustentável, flexível e fácil de manter ao longo do tempo. A ideia central é separar claramente as responsabilidades das diferentes partes do sistema, mantendo os detalhes de implementação (como frameworks, bancos de dados ou interfaces) isolados do **núcleo da aplicação** (Application Core), que contém as regras de negócio e lógica central. Essa separação permite que mudanças em tecnologias externas, como a troca de um banco de dados ou a modificação de uma interface de usuário, não impactem diretamente o núcleo do sistema. 

O Clean Code e a Clean Architecture são conceitos diferentes, embora ambos tenham como objetivo melhorar a qualidade e a manutenibilidade do software, eles se concentram em áreas distintas do desenvolvimento. Em resumo, o Clean Code se concentra na legibilidade e manutenibilidade do código em si, enquanto a Clean Architecture trata da organização e estruturação do sistema como um todo, visando criar sistemas mais independentes, testáveis e adaptáveis. Esses conceitos muitas vezes são aplicados em conjunto para desenvolver sistemas de software de alta qualidade e facilmente mantidos.

As regras universais de arquitetura de software desempenham um papel fundamental na produtividade dos desenvolvedores ao longo da vida útil dos sistemas. Agora, aproveitando o sucesso dos aclamados livros "Código Limpo" e "O Codificador Limpo", o renomado artesão de software Robert C. Martin, também conhecido como "Uncle Bob", traz sua experiência para apresentar essas regras e auxiliar os leitores em sua aplicação.

<img src="https://github.com/user-attachments/assets/038eb886-2db7-456a-a67c-3707b7020c31" align="right" height="177">

> [!Important]
> Em **A Arquitetura Limpa: O Guia do Artesão para Estrutura e Design de Software**, Martin vai além de um simples catálogo de opções. Com base em mais de meio século de experiência em diversos ambientes de software, ele oferece orientações sobre as escolhas cruciais e explica por que são essenciais para o sucesso. Como esperado de Uncle Bob, o livro apresenta soluções simples e diretas para os desafios reais enfrentados pelos desenvolvedores, desafios que podem determinar o êxito ou o fracasso de seus projetos.

O desenvolvimento de software moderno geralmente envolve sistemas complexos que precisam se adaptar rapidamente às mudanças, sejam requisitos do usuário, atualizações de tecnologia ou mudanças de mercado.

A Clean Architecture pode ajudar com isso. É uma filosofia de design de software que enfatiza a criação de sistemas fáceis de entender, manter e estender.

Em sua essência, a Clean Architecture tenta garantir que as partes mais importantes do seu aplicativo, como regras de negócios e lógica, sejam independentes de preocupações externas, como estruturas, bancos de dados ou interfaces de usuário.

A Arquitetura Limpa foi popularizada por Robert C. Martin, também conhecido como Tio Bob. Ele introduziu o conceito em seu livro Clean Architecture, onde se baseou em paradigmas de design anteriores, como Hexagonal Architecture e Onion Architecture.

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/0212933c-7199-4f15-ba63-94580c350a57" height="777"></td>
	    <td><img src="https://github.com/user-attachments/assets/52dc9da7-7b78-42cc-91cf-a899804b2e4d" height="877"></td>
	</tr>
</table>

O principal objetivo da Clean Architecture é:

- Torne o software sustentável
- Melhore a escalabilidade
- Melhore a capacidade de teste dos componentes
- Desacoplar a lógica de negócios dos detalhes externos

Em termos simples, a Clean Architecture organiza um sistema de software em camadas, cada uma com uma responsabilidade específica. As dependências fluem apenas em uma direção: em direção à lógica de negócios principal. Essa estrutura ajuda a manter o sistema modular, testável e resiliente a alterações.

Exploraremos os princípios-chave da Arquitetura Limpa e também examinaremos as várias partes da estrutura em camadas.

A obra aborda uma ampla gama de tópicos, incluindo as metas dos arquitetos de software, disciplinas e práticas fundamentais para alcançá-las, princípios essenciais de design de software para lidar com funcionalidades, separação de componentes e gerenciamento de dados, além da influência dos paradigmas de programação na disciplina dos desenvolvedores. Martin também ensina a distinguir o que é crucialmente importante do que é apenas um "detalhe", e explora a implementação de estruturas de alto nível para diferentes tipos de aplicações. O livro ainda aborda a importância de estabelecer limites apropriados, organizar componentes e serviços, e oferece insights sobre a prevenção e correção de falhas em designs e arquiteturas, bem como a compreensão de suas causas.

Com sua vasta experiência e expertise, Robert C. Martin fornece insights valiosos para o desenvolvimento de software de qualidade, tornando este livro um guia abrangente e prático para arquitetura de software eficiente. Se você busca aprimorar suas habilidades e elevar seu trabalho a um nível superior, "A Arquitetura Limpa" é uma leitura imprescindível que abrirá novos horizontes em sua jornada como desenvolvedor de software.

O Clean Architecture é um conjunto de práticas para projetar a arquitetura de um sistema de software, separando as preocupações em camadas distintas e definindo claramente como as diferentes partes do sistema se relacionam. Enfatiza a separação de preocupações (separation of concerns), criando fronteiras bem definidas entre as camadas da aplicação. Propõe uma estrutura modular que permite que o código de negócio não dependa de detalhes de implementação externos, como banco de dados ou frameworks específicos. Busca criar sistemas flexíveis, testáveis e independentes de detalhes de implementação, facilitando a manutenção e a evolução do software ao longo do tempo.

<img src="https://github.com/user-attachments/assets/8fc2d208-54d2-4e30-a01b-d26056dd268e" align="right" height="277">

O foco está na independência e na testabilidade do código. Na arquitetura limpa, as regras de negócio não dependem de detalhes de implementação, mas o contrário pode acontecer: os detalhes devem se conformar às regras de negócio. Isso é alcançado por meio de camadas bem definidas, onde a camada mais interna (ou núcleo) contém as entidades e casos de uso, enquanto as camadas externas lidam com detalhes como APIs, frameworks ou dispositivos.

Essa abordagem também promove a inversão de dependência, geralmente utilizando interfaces para desacoplar implementações concretas. O resultado é um sistema mais modular, onde cada parte pode ser alterada ou substituída sem afetar significativamente o restante da aplicação. Arquitetura limpa não é uma receita fixa, mas sim um guia para projetar sistemas que resistam à passagem do tempo e às inevitáveis mudanças de requisitos, priorizando sempre a clareza e a simplicidade no design.

A arquitetura limpa se encaixa bem tanto em aplicações monolíticas quanto em arquiteturas de microserviços, pois seus princípios são agnósticos em relação à forma como o software é implantado ou estruturado. O objetivo principal da arquitetura limpa é organizar o código de maneira que ele seja fácil de manter, testar e evoluir, independentemente do contexto em que está sendo usado. 

No caso de uma **aplicação monolítica**, a arquitetura limpa ajuda a modularizar o sistema internamente. Mesmo que todo o código esteja em um único processo ou projeto, a separação de camadas e responsabilidades evita que partes diferentes do sistema fiquem acopladas de forma inadequada. Isso significa que, mesmo em um monólito, é possível aplicar as mesmas boas práticas de desacoplamento que seriam usadas em microserviços. Além disso, facilita a refatoração ou a futura divisão do sistema em serviços menores, caso seja necessário migrar para microserviços no futuro.

Por outro lado, em um contexto de **microserviços**, a arquitetura limpa é igualmente valiosa, pois cada serviço é tratado como uma unidade independente. Dentro de cada microserviço, os princípios da arquitetura limpa podem ser aplicados para garantir que ele tenha uma estrutura interna bem definida e resiliente a mudanças. Isso é especialmente importante em cenários de microserviços, onde a comunicação entre serviços já adiciona complexidade, e manter cada serviço coeso e bem organizado é fundamental para evitar problemas de manutenção e escalabilidade.

Portanto, a arquitetura limpa não é restrita a um único paradigma de implantação. Ela é uma abordagem universal que visa garantir qualidade e sustentabilidade no desenvolvimento, seja em um monólito ou em um conjunto de microserviços. O contexto ideal depende mais das necessidades do sistema e dos objetivos do time do que do padrão arquitetural escolhido.

![What is Clean Architecture2](https://github.com/user-attachments/assets/fbf314e1-e62a-4b5a-ad36-7b555426c097)

## [Microservices] DDD - Domain-Driven Design
<img src="https://img.shields.io/badge/Python-3.10.7-3776AB?style=flat&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-339933?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/Ruby-3.3-CC342D?style=flat&logo=Ruby&logoColor=white"> <img src="https://img.shields.io/badge/Go-1.21-00ADD8?style=flat&logo=Go&logoColor=white"> <img src="https://img.shields.io/badge/PHP-8.2-777BB4?style=flat&logo=PHP&logoColor=white"> <img src="https://img.shields.io/badge/C++-23-F5455C?style=flat&logo=CPlusPlus&logoColor=white"> <img src="https://img.shields.io/badge/Java-22.0.1-chocolate?style=flat&logo=OpenJDK&logoColor=white"> <img src="https://img.shields.io/badge/.NET-8.0.300-512BD4?style=flat&logo=DotNet&logoColor=white"> <img src="https://img.shields.io/badge/Rust-1.82.0-dda584?style=flat&logo=Rust&logoColor=white"> <img src="https://img.shields.io/badge/UML-diagrams-purple?style=flat&logo=UML&logoColor=white"> 

<a href=""><img src="https://em-content.zobj.net/source/microsoft-teams/363/ferris-wheel_1f3a1.png" align="right" height="77"></a>

O **DDD - Domain-Driven Design** (Projeto Orientado a Domínio) é uma abordagem de desenvolvimento de software que se concentra em entender o **domínio do negócio** e modelar o software em torno desses conceitos e regras de negócio. É um tipo de <a href="">modelagem de software</a> e um <a href="">design de software</a> orientado a objetos (OOP) que procura reforçar conceitos e boas práticas relacionadas à OOP e surgiu como uma resposta às dificuldades enfrentadas por desenvolvedores ao lidarem com sistemas complexos, especialmente em domínios de negócio onde a lógica e os requisitos mudam frequentemente. 

Isso vem em contrapartida com o uso comum do <a href="">Data-Driven Design</a> (Projeto Orientado a Dados), que a maioria dos desenvolvedores usa sem mesmo ter consciência disso. O design orientado por domínio (DDD) é uma abordagem importante de design de software, focada em modelar software para corresponder a um domínio de acordo com a contribuição dos especialistas desse domínio. A DDD é contra a ideia de ter um modelo unificado único; em vez disso, divide um grande sistema em contextos limitados, cada um com seu próprio modelo. 

Sem levar em conta o DDD, as **técnicas de modelagem de domínio** são métodos utilizados na engenharia de software para compreender e representar o domínio de um problema específico. 

O **domínio** (domain) refere-se à área de conhecimento, contexto ou setor de negócios em que o software está sendo desenvolvido. A modelagem de domínio tem como objetivo capturar os conceitos, regras e relacionamentos do domínio em um formato compreensível e utilizável pelos desenvolvedores. Então, o DDD (Domain-Driven Design) é uma abordagem para o desenvolvimento de software que combina conceitos de design de software e técnicas de modelagem de domínio. 

Não é considerado um design pattern específico, mas sim uma abordagem geral para projetar e estruturar sistemas de software. Domain-Driven Design (DDD) é um método de design de software em que os desenvolvedores constroem modelos para entender os requisitos de negócios de um domínio. Esses modelos servem como base conceitual para o desenvolvimento de software.

O termo foi cunhado por Eric Evans em seu livro de mesmo nome, publicado em 2003. No entanto, a definição mais simples que encontrei foi ao ler o livro Fundamentals of Software Architecture de Neal Ford e Mark Richards:

> O design orientado a domínio (DDD) é uma técnica de modelagem que permite a decomposição organizada de domínios de problemas complexos. - Neal Ford e Mark Richards. Fundamentos da Arquitetura de Software. 2020.

Eric Evans cunhou o termo Domain-Driven Design (DDD) como parte do título de seu livro de 2004, Domain-Driven Design: Tackling Complexity in the Heart of Software.

<a href=""><img src="https://github.com/user-attachments/assets/47723806-ab10-490c-844f-6c5e8980e08f" align="right" height="177"></a>

> [!Important]
> Foi popularizado por Eric Evans em seu livro **Domain-Driven Design: Tackling Complexity in the Heart of Software**, publicado em 2003. Esse livro não é leve, especialmente se você ainda está no início da jornada. Ele exige uma certa base em desenvolvimento orientado a objetos (OOP), arquitetura de software e experiência prática com projetos reais. Geralmente, ele é mais proveitoso depois que você já trabalhou em sistemas mais complexos ou com arquitetura em camadas. O Design Orientado por Domínio (DDD) ganhou atenção significativa no desenvolvimento de software por seu potencial de enfrentar desafios complexos de software, especialmente nas áreas de refatoração de sistemas, reimplementação e adoção. Utilizando o conhecimento do domínio, o DDD visa resolver problemas de negócios complexos de forma eficaz.

Embora o design orientado a domínio (DDD) exista desde 2004, o conceito não foi capaz de se espalhar excessivamente em todo esse tempo. Nos últimos anos, no entanto, o termo experimentou uma segunda primavera. Onde o desenvolvimento de software não é um fim em si mesmo. Em vez disso, o software é desenvolvido para resolver problemas técnicos do mundo real. Isso requer tecnologia, mas esse não é o foco, é apenas um meio para um fim. O foco real está no assunto, o **domínio** (domain)! Portanto, uma boa compreensão disso é essencial para um desenvolvimento bem-sucedido e direcionado.

Sob design orientado por domínio, a estrutura e a linguagem do código de software (nomes de classes, métodos de classe, variáveis de classe) devem corresponder ao domínio de negócio. Por exemplo: se o software processa solicitações de empréstimo, pode ter classes como "`solicitação de empréstimo`", "`clientes`" e métodos como "`aceitar oferta`" e "`retirar`".

DDD só funciona plenamente quando *anda alinhado* com design de software, design de sistemas e arquitetura, não porque eles sejam a mesma coisa, mas porque o DDD sozinho não consegue se sustentar sem uma estrutura técnica que dê corpo às suas ideias. O ponto central é que o Domain-Driven Design é uma abordagem profundamente conceitual: ele organiza o pensamento sobre o domínio, define limites claros, introduz linguagens específicas, identifica contextos independentes e estabelece modelos consistentes. 

Só que tudo isso precisa inevitavelmente se materializar em código, fluxos, integrações, decisões de infraestrutura, modularização e comunicação entre serviços. Se esse materializar não acompanha a lógica do domínio, o DDD implode, ou vira apenas documentação bonita.

O objetivo do DDD é, em primeiro lugar, adquirir conhecimento sobre o problema para identificar a solução. Em seguida, concordaremos com os vários componentes desta solução para implementá-la. Esse objetivo é alcançado por meio dos padrões fundamentais do DDD: padrões estratégicos e táticos. Os padrões estratégicos respondem à pergunta: "Por que estamos construindo este software e quais são seus componentes?". Por outro lado, os padrões táticos dão a resposta à pergunta: "Como esses componentes são implementados?"

Portanto, o design orientado por domínio baseia-se nos seguintes objetivos:

1. Colocando o foco principal do projeto no domínio central e na camada de lógica de domínio;
2. Basear projetos complexos em um modelo do domínio;
3. Iniciando uma colaboração criativa entre especialistas técnicos e especialistas do domínio para refinar iterativamente um modelo conceitual que aborde problemas específicos do domínio.

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/dff34406-3889-446f-818f-2353d4be9589"></td>
		<td><img src="https://github.com/user-attachments/assets/40d50d38-bef7-4b85-8aab-8eba9d22891b"></td>
	</tr>
</table>

<img src="https://github.com/user-attachments/assets/038eb886-2db7-456a-a67c-3707b7020c31" align="right" height="177">

> [!Important]
> Em seu livro **Clean Architecture: A Craftsman's Guide to Software Structure and Design**, Uncle Bob chama uma arquitetura que informa ao leitor sobre o sistema, não as estruturas usadas no sistema, de "Arquitetura Gritante". Em **A Arquitetura Limpa: O Guia do Artesão para Estrutura e Design de Software**, <a href="https://martinfowler.com/bliki/DomainDrivenDesign.html">Martin</a> vai além de um simples catálogo de opções. Com base em mais de meio século de experiência em diversos ambientes de software, ele oferece orientações sobre as escolhas cruciais e explica por que são essenciais para o sucesso. Como esperado de Uncle Bob, o livro apresenta soluções simples e diretas para os desafios reais enfrentados pelos desenvolvedores, desafios que podem determinar o êxito ou o fracasso de seus projetos.

Então, faz sentido para mim pensar em design de software como design gritante quando fala alto e claro sobre o domínio do problema. Geralmente, o ativo mais crítico no design de uma solução é adquirir conhecimento sobre os problemas que estamos tentando resolver, o processo que queremos automatizar ou as dificuldades que queremos facilitar. Então, para nos aproximarmos da solução, tínhamos que já estar próximos do problema.

Falaremos sobre a maneira de se aproximar do problema e da solução: o caminho do Domain-Driven Design (DDD) em direção a um design gritante, o design que informa ao leitor sobre o domínio do negócio, não sobre os frameworks usados.

> [!Warning]
> Quando não usar DDD? Às vezes só é necessário um CRUD (entrega de um produto funcional)! DDD não é uma solução para tudo. A maioria dos sistemas possui uma boa parte composta por cadastros básicos (CRUD) e não seria adequado usar DDD para isso. A engenharia de domínios tem sido criticada por focar demais em "engenharia para reutilização" ou "engenharia com reutilização" de recursos genéricos de software, em vez de se concentrar em "engenharia para uso", de modo que a visão de mundo, linguagem ou contexto de um indivíduo seja integrado ao design do software. Um CRUD é praticamente o estágio MVP funcional, voltado a registrar, atualizar e consultar informações, geralmente com baixo acoplamento conceitual e alto acoplamento técnico. Você descreve tabelas, cria endpoints, faz o básico para o sistema existir. Ele resolve o problema imediato, mas não escala bem quando as regras começam a se multiplicar, quando várias áreas de negócio influenciam o mesmo fluxo ou quando múltiplos times precisam trabalhar em partes diferentes da solução sem se bloquear. Então, depende da complexidade do projeto e das regras de negócio.

> [!Tip]
> Já o DDD é “nível engenharia” (entrega de um produto sustentável, capaz de sobreviver à complexidade, a mudanças constantes, a regras de negócio extensivas e a um ciclo de vida longo), porque exige que o desenvolvedor deixe de pensar apenas como codificador e passe a operar como analista de domínio, arquiteto e estrategista ao mesmo tempo. É necessário entender profundamente o negócio, descobrir limites contextuais, refinar invariantes, identificar agregados, modelar comportamentos, conversar com especialistas e traduzir tudo isso para uma arquitetura mais sólida, isolada e resiliente, geralmente integrada com abordagens como Clean Architecture, Hexagonal, Onion, EDA, CQRS, Event Sourcing e microsserviços.
>
> Você aplica DDD quando a complexidade do domínio começa a crescer a ponto de inviabilizar soluções lineares ou meramente CRUD. Ele se torna realmente vantajoso quando você precisa que o software represente fielmente regras de negócio dinâmicas, mutáveis e distribuídas, principalmente em arquiteturas mais sofisticadas como microsserviços, BFF, EDA, Hexagonal, Clean Architecture, Onion ou Tomato. Nessas abordagens, há múltiplos contextos, integrações, fluxos assíncronos, eventos, fronteiras claras e times diferentes trabalhando sobre partes distintas do sistema; tudo isso exige linguagem ubíqua, modelagem explícita, separação de responsabilidades e decisões guiadas pelo domínio. Em sistemas simples, centralizados ou puramente transacionais, DDD vira peso morto, mas em cenários complexos ele traz clareza, previsibilidade e alinhamento entre tecnologia e negócio, evitando entropia arquitetural e facilitando evolução contínua.

Por isso, ele é usado quando a aplicação deixa de ser “só um sistema” e passa a ser um ecossistema vivo, com equipe, visão de produto, múltiplos contextos e evolução contínua. É literalmente a fronteira entre “programação” e “engenharia de software aplicada ao domínio”.

No entanto, críticos do design orientado por domínio argumentam que os desenvolvedores normalmente precisam implementar uma grande quantidade de isolamento e encapsulamento para manter o modelo como uma construção pura e útil. Embora o design orientado por domínio ofereça benefícios como manutenção, a Microsoft o recomenda apenas para domínios complexos onde o modelo oferece benefícios claros na formulação de uma compreensão comum do domínio.

A exigência de construir um entendimento profissional também se aplica aos desenvolvedores. Uma boa compreensão do assunto (domínio) surge da comunicação regular e de uma linguagem comum, o que representa um desafio, principalmente em equipes interdisciplinares: Afinal, cada disciplina tem sua linguagem técnica, por isso os mal-entendidos são inevitáveis.

<img height="413" align="right" src="https://github.com/user-attachments/assets/e2c65dfd-24ff-473c-9007-4d1256554953" />

Num <a href="">Code Review</a>, o time não está apenas olhando se o código “funciona”, mas se ele está legível, sustentável e alinhado ao domínio. É aí que DDD se torna um guia. Por exemplo, quando você define entidades e value objects, o revisor consegue avaliar se você está representando o domínio corretamente ou se misturou regras de negócio com detalhes de infraestrutura. Se você trabalha com bounded contexts, o code review ajuda a garantir que cada módulo está respeitando suas fronteiras e não está acoplando responsabilidades que deveriam estar separadas. E quando se usa a linguagem ubíqua, qualquer pessoa envolvida no projeto pode bater o olho no código e identificar termos familiares do negócio, reduzindo ambiguidades.

A ideia central é trazer o domínio (o sujeito, a razão) à tona...O <a href="https://unibo-dtm-se.github.io/course-slides/ddd/#/">DDD</a> acaba aparecendo muito em code reviews (revisões de código) porque ele não é só um conjunto de padrões técnicos, mas uma maneira de organizar o raciocínio e o design do sistema a partir do domínio de negócio. Diferente de TDD e BDD, que são mais voltados ao como testar e como validar comportamento, o DDD toca no como estruturar o código para refletir a realidade do problema que a aplicação resolve.

Isso muda o tom da revisão: em vez de ser só “esse método está mal nomeado” ou “esse if pode virar um switch”, passa a ser “essa entidade realmente pertence a este contexto?” ou “essa regra deveria estar no domínio ou no serviço de aplicação?”. São discussões de mais alto nível, que evitam dívida técnica e fortalecem a coerência do sistema. Por isso, times que adotam DDD costumam ter code reviews mais ricos, que não param na forma, mas questionam se a essência do código está fiel ao problema que ele resolve.

O DDD (Domain-Driven Design) entra no fluxo do desenvolvimento de produto antes do MVP, como um alicerce. Ele não é um artefato de entrega como MVP, UAT ou Release, mas sim uma abordagem de modelagem que orienta como o software deve ser desenhado para refletir o domínio do problema.

Se você pensar em sequência, o fluxo ficaria assim: Engenharia de domínio + Engenharia de requisitos + MVP - Minimum Product Viable + Design orientado por domínio + Design Evolutivo + Arquitetura de aplicações

<img height="277" align="right" src="https://github.com/user-attachments/assets/29d08cac-4445-4200-be35-d46f5e822991" />

1. **DDD – Domain-Driven Design**: Aqui você faz a imersão no domínio de negócio, conversa com especialistas e stakeholders, descobre a linguagem ubíqua e modela o sistema em termos que façam sentido para o negócio. É nessa etapa que surgem conceitos como entidades, agregados, bounded contexts e eventos de domínio. O objetivo é garantir que a estrutura do software nasça aderente à realidade que ele pretende resolver.

2. **MVP – Minimum Viable Product**: Uma vez que o domínio esteja bem modelado, você constrói o MVP. Esse MVP já se beneficia do DDD, porque mesmo sendo mínimo, ele está fundamentado em um design que respeita a linguagem e as regras do negócio. Isso evita que o MVP vire um “protótipo descartável” e aumenta a chance de evoluir para produto de verdade.

3. **QA interno** → **UAT** → **Release** → **Continuous Delivery**: Depois disso, o fluxo segue normalmente como te expliquei antes.

Então, se o MVP é o “primeiro produto que entrega valor real”, o *DDD é o mapa que garante que esse valor seja o certo*, modelando desde o início com consistência e visão de futuro. Sem o DDD, corre-se o risco de o MVP ser feito de qualquer jeito e depois ser difícil ou custoso de evoluir.

Um conceito fundamental para tudo isso é a **Engenharia de domínio** que é todo o processo de reutilização do conhecimento de domínio na produção de novos sistemas de software. É um conceito-chave no reuso sistemático de software e na engenharia de linhas de produtos. Uma ideia-chave na reutilização sistemática de software é o domínio. A maioria das organizações atua em apenas alguns domínios. Eles constroem repetidamente sistemas semelhantes dentro de um determinado domínio, com variações para atender a diferentes necessidades dos clientes. Em vez de construir cada nova variante do zero, economias significativas podem ser alcançadas reutilizando partes de sistemas anteriores no domínio para construir novos.

O processo de identificar domínios, delimitá-los e descobrir semelhanças e variáveis entre os sistemas do domínio é chamado de análise de domínio. Essas informações são capturadas em modelos usados na fase de implementação do domínio para criar artefatos como componentes reutilizáveis, uma linguagem específica de domínio ou geradores de aplicações que podem ser usados para construir novos sistemas no domínio.

Na **engenharia de linhas de produtos**, conforme definido por ISO26550:2015, a Engenharia de Domínios é complementada pela Engenharia de Aplicações, que cuida do ciclo de vida dos produtos individuais derivados da linha de produtos. 

A engenharia de domínio é projetada para melhorar a qualidade dos produtos de software desenvolvidos por meio do reaproveitamento de artefatos de software. A engenharia de domínios mostra que a maioria dos sistemas de software desenvolvidos não são sistemas novos, mas sim variantes de outros sistemas dentro do mesmo campo. Como resultado, por meio do uso da engenharia de domínio, as empresas podem maximizar lucros e reduzir o tempo de lançamento no mercado utilizando conceitos e implementações de sistemas de software anteriores e aplicando-os ao sistema-alvo. A redução de custos é evidente mesmo durante a fase de implementação. Um estudo mostrou que o uso de linguagens específicas de domínio permitiu que o tamanho do código, tanto em número de métodos quanto em número de símbolos, fosse reduzido em mais de 50%, e o número total de linhas de código fosse reduzido em quase 75%.

A engenharia de domínios foca em capturar o conhecimento adquirido durante o processo de engenharia de software. Ao desenvolver artefatos reutilizáveis, os componentes podem ser reutilizados em novos sistemas de software a baixo custo e alta qualidade. Como isso se aplica a todas as fases do ciclo de desenvolvimento de software, a engenharia de domínios também foca nas três fases principais: análise, design e implementação, paralelamente à engenharia de aplicações. Isso produz não apenas um conjunto de componentes de implementação de software relevantes para o domínio, mas também requisitos e projetos reutilizáveis e configuráveis.

Dado o crescimento dos dados na Web e da Internet das Coisas, uma abordagem de engenharia de domínios está se tornando relevante para outras disciplinas também. O surgimento de cadeias profundas de serviços Web destaca que o conceito de serviço é relativo. Serviços web desenvolvidos e operados por uma organização podem ser utilizados como parte de uma plataforma por outra organização. Como os serviços podem ser usados em diferentes contextos e, portanto, requerem configurações distintas, o projeto de famílias de serviços pode se beneficiar de uma abordagem de engenharia de domínio.

A engenharia de domínios, assim como a engenharia de aplicações, consiste em três fases principais: análise, projeto e implementação. No entanto, enquanto a engenharia de software foca em um único sistema, a engenharia de domínios foca em uma família de sistemas. Um bom modelo de domínio serve como referência para resolver ambiguidades mais adiante no processo, um repositório de conhecimento sobre as características e definição do domínio, e uma especificação para desenvolvedores de produtos que fazem parte do domínio.

A **análise de domínio** é usada para definir o domínio, coletar informações sobre o domínio e produzir um modelo de domínio. Por meio do uso de modelos de características (inicialmente concebidos como parte do método de análise de domínio orientada a características), a análise de domínio visa identificar os pontos comuns em um domínio e os pontos variáveis dentro do domínio. Por meio do uso da análise de domínio, é possível o desenvolvimento de requisitos e arquiteturas configuráveis, em vez de configurações estáticas que seriam produzidas por uma abordagem tradicional de engenharia de aplicação.

A análise de domínio é significativamente diferente da engenharia de requisitos e, como tal, abordagens tradicionais para derivar requisitos são ineficazes para o desenvolvimento de requisitos configuráveis, como estariam presentes em um modelo de domínio. Para aplicar a engenharia de domínio de forma eficaz, o reuso deve ser considerado nas fases iniciais do ciclo de vida do desenvolvimento de software. Por meio da seleção de recursos dos modelos desenvolvidos, a reutilização da tecnologia é realizada muito cedo e pode ser aplicada adequadamente durante todo o processo de desenvolvimento.

A análise de domínio é derivada principalmente de artefatos produzidos a partir de experiências passadas no domínio. Sistemas existentes, seus artefatos (como documentos de projeto, documentos de requisitos e manuais do usuário), padrões e clientes são todas fontes potenciais de entrada para análise de domínio. No entanto, ao contrário da engenharia de requisitos, a análise de domínio não consiste apenas na coleta e formalização de informações; Existe também um componente criativo. Durante o processo de análise de domínio, os engenheiros buscam ampliar o conhecimento do domínio além do que já é conhecido e categorizar o domínio em semelhanças e diferenças para aumentar a reconfigurabilidade.

A análise de domínio produz principalmente um modelo de domínio, representando as propriedades comuns e variáveis dos sistemas dentro do domínio. O modelo de domínio auxilia na criação de arquiteturas e componentes de maneira configurável, atuando como uma base sobre a qual projetar esses componentes. Um modelo de domínio eficaz não inclui apenas as características variáveis e consistentes de um domínio, mas também define o vocabulário usado no domínio e define conceitos, ideias e fenômenos dentro do sistema.

Modelos de características decompõem conceitos em suas características necessárias e opcionais para produzir um conjunto totalmente formalizado de requisitos configuráveis.

O **design de domínio** toma o modelo de domínio produzido durante a fase de análise de domínio e visa produzir uma arquitetura genérica à qual todos os sistemas dentro do domínio possam se conformar. Da mesma forma que a engenharia de aplicações utiliza os requisitos funcionais e não funcionais para produzir um projeto, a fase de projeto de domínio da engenharia de domínios toma os requisitos configuráveis desenvolvidos durante a fase de análise de domínio e produz uma solução configurável e padronizada para a família de sistemas. O design de domínios visa produzir padrões arquitetônicos que resolvam um problema comum entre os sistemas dentro do domínio, apesar das diferentes configurações de requisitos. Além do desenvolvimento de padrões durante o projeto de domínio, os engenheiros também devem tomar cuidado para identificar o escopo do padrão e o nível em que o contexto é relevante para o padrão. A limitação do contexto é crucial: contexto excessivo resulta em o padrão não ser aplicável a muitos sistemas, e contexto insuficiente resulta em um padrão insuficientemente poderoso para ser útil. Um padrão útil deve ser frequentemente recorrente e de alta qualidade.

O objetivo do design de domínio é satisfazer o maior número possível de requisitos de domínio, mantendo a flexibilidade oferecida pelo modelo de características desenvolvido. A arquitetura deve ser suficientemente flexível para satisfazer todos os sistemas dentro do domínio, ao mesmo tempo em que rígida o bastante para fornecer uma estrutura sólida sobre a qual basear a solução.

Implementação de domínio é a criação de um processo e de ferramentas para gerar eficientemente um programa personalizado no domínio.

Um domínio bem modelado só tem efeito se o design de software respeita a coesão do modelo, preserva invariantes, mantém consistência interna e evita que detalhes técnicos vazem para áreas onde não deveriam. Se o design de software decide misturar responsabilidades, criar acoplamentos arbitrários, espalhar regras por camadas que não conversam com o domínio ou ignorar o Ubiquitous Language, então o DDD perde força, porque o código deixa de refletir as estruturas conceituais. O resultado é um sistema que só “parece DDD no papel”, mas opera como um monólito acoplado, com entidades sem significado e casos de uso sem fronteiras.

<img height="413" align="right" src="https://github.com/user-attachments/assets/d4500284-4180-420e-b551-056dbe5a17d0" />

Ao mesmo tempo, DDD também depende do design de sistemas, porque os **Bounded Contexts** (Contextos limitados), para existirem de verdade, precisam de fronteiras técnicas: precisam ser isolados, ter seus próprios modelos, seus próprios fluxos de dados, sua própria vida. É o <a href="">design de sistemas (System design)</a> que decide como esses contextos conversam, se por eventos, filas, APIs, contratos assíncronos ou mensagens. O DDD diz *“esses dois contextos são independentes e têm linguagens diferentes”*; o design de sistemas transforma essa independência em topologia real e se ele falha nisso, os contextos se fundem, o sistema fica acoplado e a proposta de modularidade do DDD desaparece.

E por fim, a arquitetura de software é o alicerce onde o DDD se apoia. É ela que escolhe padrões como microservices, monólito modular, event-driven, CQRS, event sourcing, hexagonal ou clean architecture, que definem como as partes se organizam, como as dependências fluem, como proteções ao domínio são criadas. A arquitetura é o meio técnico que permite que o domínio respire. Quando a arquitetura é mal desenhada, a equipe tenta aplicar DDD sobre um terreno instável, e o domínio acaba se adaptando aos problemas arquiteturais em vez de a arquitetura se adaptar ao domínio. DDD, nesse cenário, vira ornamento.

Então, sim: DDD precisa andar alinhado com design de software, design de sistemas e arquitetura. O DDD é a visão conceitual, estratégica e semântica; o design de software é a expressão detalhada e tática; o design de sistemas é a topologia operacional; e a arquitetura é a fundação estrutural. Quando esses quatro caminham juntos, o domínio guia o software, o sistema é coerente, a linguagem é compartilhada, os limites são respeitados, e a complexidade fica organizada. Quando andam separados, o DDD deixa de ser um modelo vivo e vira apenas teoria sem impacto real no código e no comportamento do sistema.

O design orientado por domínio articula uma série de conceitos e práticas de alto nível. De importância primordial é o domínio do software, a área de estudo à qual o usuário aplica um programa. Os desenvolvedores de software constroem um modelo de domínio: um sistema de abstrações que descreve aspectos selecionados de um domínio e pode ser usado para resolver problemas relacionados a esse domínio.

Esses aspectos do design orientado por domínio visam fomentar uma linguagem comum compartilhada por especialistas em domínio, usuários e desenvolvedores — a **linguagem onipresente**. A linguagem onipresente é usada no modelo de domínio e para descrever os requisitos do sistema. A linguagem onipresente é um dos pilares do DDD junto com o design estratégico e o design tático. No design orientado por domínio, a camada de domínio é uma das camadas comuns em uma **arquitetura multicamadas orientada a objetos**.

Os conceitos e práticas do DDD são dividos em camadas de domínio: Quando você diz que os conceitos e práticas do Domain-Driven Design são divididos em camadas, você está tocando em uma das características mais marcantes do DDD, mas que muitas vezes é mal compreendida. DDD não é exatamente uma “arquitetura em camadas”, mas ele influenciou fortemente arquiteturas que usam camadas de maneira disciplinada. O ponto central é que DDD organiza o software em torno do domínio, e essa organização naturalmente cria zonas distintas de responsabilidade, que acabam se parecendo com camadas lógicas, mesmo que o padrão em si não force isso.

Na prática, quando falamos de camadas em DDD, normalmente estamos falando do conjunto de estruturas conceituais que separa o coração do domínio (onde vivem as regras de negócio puras) das partes infraestruturais, externas ou acopladas a tecnologia. O domínio fica isolado, limpo, autocontido, enquanto o resto da aplicação orbita em volta dele, servindo-o, protegendo-o e garantindo que ele se mantenha expressivo e imutável diante das mudanças tecnológicas. 

<img width="100%" alt="image" src="https://github.com/user-attachments/assets/cc8dad6f-afc7-4b1b-8ebd-30df9b57b557" />

Os padrões estratégicos lidam com a obtenção de uma visão geral do domínio de negócios, o que inclui decompô-lo em regras de negócios.

> Estritamente falando, as regras de negócios são regras ou procedimentos que fazem ou economizam o dinheiro da empresa. — Tio Bob, Arquitetura Limpa: Guia de um Artesão para Estrutura e Design de Software

<img height="977" align="right" src="https://github.com/user-attachments/assets/e10458c3-c96c-46aa-8007-27e1a11c0282" />

Em outras palavras, as regras de negócios são os recursos funcionais que requerem desenvolvimento. No entanto, existem diferentes tipos de regras de negócios. Existem urgentes e importantes. Ainda assim, outros não são urgentes, mas são importantes. Coletar e reagrupar essas regras de forma significativa ajuda a decompor a complexidade do domínio de negócios em subdomínios: subdomínios principais, genéricos e de suporte.

O **subdomínio principal** contém as regras de negócios que oferecem vantagem competitiva e destacam a diferença entre as empresas que trabalham no mesmo domínio de negócios. Ele incorpora uma lógica de negócios altamente complexa e volátil. Portanto, ele deve estar aberto a mudanças na lógica de negócios, o que pode envolver a adição de novos requisitos, a atualização dos antigos ou até mesmo a remoção de alguns deles. Em seguida, ele deve ser cuidadosamente implementado internamente para permitir que essas alterações ocorram de forma eficiente sem causar muitos problemas em todo o software.

A conclusão das regras de negócios do subdomínio principal requer outras regras de negócios que não envolvem lógica altamente complexa nem volátil. Em vez disso, eles apenas apoiam os negócios da empresa sem invocar nenhuma vantagem competitiva, pois estão resolvendo um problema muito óbvio. Eles são desenvolvidos internamente e podem ser terceirizados. Aqui, falamos sobre o subdomínio de suporte. No entanto, o subdomínio genérico consiste em regras de negócios relacionadas a um problema já resolvido para que ele possa ser comprado ou adotado.

Ao destilar o domínio de negócios em busca de subdomínios, devemos falar a mesma língua para nos entendermos. Devemos, portanto, usar o mesmo termo para nos referirmos a um determinado objeto, comportamento ou campo. Na terminologia do DDD, é chamada de linguagem onipresente. Aqui, estamos evocando um dos ingredientes indispensáveis para construir uma solução de software: comunicação eficaz entre as diferentes partes interessadas do projeto, incluindo desenvolvedores, especialistas de domínio, analistas de negócios, gerentes de projeto, gerentes de marketing, etc.

Como desenvolvedores de software, devemos garantir que nossas suposições estejam alinhadas com o conhecimento dos especialistas do domínio. Alberto Brandolini, que é um consultor versátil na área de Tecnologia da Informação, disse uma vez:

> Não é o conhecimento dos especialistas de domínio que vai para a produção, são as suposições dos desenvolvedores que vão para a produção. — Alberto Brandolini

Ele é um especialista em DDD que criou o **EventStorming**, uma metodologia colaborativa envolvendo todas as partes interessadas do projeto para compartilhar conhecimento sobre o domínio do problema. Ele os reuniu com post-its e canetas coloridas diante de um quadro branco para iniciar uma sessão de análise de conhecimento. Essas metodologias ajudam a encontrar limites para separar regras de negócios consistentes e reagrupá-las por contexto. Na terminologia do DDD, esses grupos são chamados de Contextos Limitados, cada um contendo regras de negócios consistentes.

Como reconhecemos regras de negócios consistentes? Regras de negócios consistentes falam uma linguagem onipresente consistente. Quando chamamos de conceito "um" usando um vocabulário diferente e começamos a tratá-lo de um ponto de vista diferente, podemos estar falando de duas responsabilidades comerciais diferentes que exigem segregação de contexto. Além disso, regras de negócios consistentes geralmente mudam pelo mesmo motivo, portanto, mantê-las juntas é melhor.

Cada contexto limitado incorpora determinados recursos de domínio para cumprir uma única responsabilidade e pode ser empacotado de forma independente. Dessa forma, nosso software será fatiado verticalmente e empacotado por recurso. Além disso, essas fatias verticais devem se comunicar para processar um fluxo de trabalho de negócios específico. Portanto, nossos contextos limitados precisam colaborar; Enquanto isso, devemos proteger a consistência das regras de negócios. Devemos escolher o tipo de comunicação que melhor se adapta aos requisitos do negócio, nem mais, nem menos.

A maneira como os contextos limitados devem se comunicar também afeta a maneira como as equipes devem se organizar e colaborar. Duas formas de comunicação são possíveis: cooperação ou comunicação cliente-fornecedor.

Como cooperamos em diferentes contextos delimitados? A cooperação é possível através de parcerias. Nesse tipo de relacionamento, as equipes são parceiras na solução de problemas que surgem durante a integração de contextos limitados; Eles devem, portanto, sincronizar com frequência para detectar pontos de bloqueio, a fim de garantir a integridade do software.

Outra maneira de cooperar entre contextos limitados é ter um kernel compartilhado. As equipes criam um modelo compartilhado que deve ser consistente em todos os contextos limitados que o utilizam. O uso desse padrão deve ser justificado pelo custo da duplicação, que é maior do que o custo da coordenação.

E quanto à relação Cliente-Fornecedor? No tipo de comunicação Cliente-Fornecedor, tínhamos dois lados. O lado do fornecedor é chamado de "upstream", enquanto os clientes são conhecidos como "downstream". O fornecedor é aquele que presta um serviço aos seus clientes. No entanto, os clientes podem interagir de forma diferente com esse serviço, dependendo do padrão de serviço conformista, anticorrupção ou de host aberto.

Conformista significa que o downstream estará em conformidade com o modelo upstream. No entanto, o downstream não estará em conformidade com o modelo upstream na camada anticorrupção. Em vez disso, ele o personalizará para se adequar ao seu modelo por meio de uma camada anticorrupção para proteger seu modelo contra corrupção e conceitos irrelevantes que podem prejudicar a consistência do contexto limitado. Outra maneira de proteger o downstream é seguir o padrão de serviço de host aberto. Nesse padrão, o fornecedor exporá um serviço que esteja em conformidade com seus clientes. Em outras palavras, o upstream pode ter versões diferentes de uma linguagem publicada para estar em conformidade com seu modelo downstream correspondente.

Após essa longa jornada de obtenção do conhecimento essencial, decomposição do domínio de negócios em subdomínios, delimitação de contextos e desenho das relações entre eles, traçamos um mapa de contexto. É uma representação visual que fornece insights, em primeiro lugar, sobre o design de alto nível, incluindo nossos subdomínios, contextos limitados, bem como o modelo que eles implementarão, em segundo lugar, sobre os padrões de comunicação que devem ser usados entre os contextos limitados e, finalmente, sobre a organização e colaboração das equipes.

O DDD nos permite planejar uma arquitetura de microsserviços decompondo o sistema maior em unidades independentes, compreendendo as responsabilidades de cada uma e identificando seus relacionamentos, ele não é um design pattern específico, mas sim uma importante abordagem de design de software, com foco na modelagem de software para corresponder a um **domínio** de acordo com as informações dos especialistas desse domínio. O Domain-Driven Design (DDD) surgiu como uma metodologia revolucionária para a modelagem de software, desenvolvida com o intuito de refinar e otimizar a correspondência entre o design do software e o domínio do software e o domínio do problema que ele busca resolver.

> Os microsserviços são a forma mais escalável de desenvolver software. Mas você precisa de um bom design que permita que as equipes de desenvolvedores trabalhem de forma autônoma e implementem sem atrapalhar umas às outras, caso contrário, você perderá os benefícios de escalabilidade. O DDD ajuda a delimitar responsabilidades claras entre os serviços, o que permite que equipes atuem de forma independente e coordenada.

No entanto, suas raízes vêm de práticas e ideias que estavam sendo discutidas na indústria desde os anos 1990. Durante esse período, muitas empresas estavam adotando metodologias ágeis e enfrentando problemas ao construir sistemas que não apenas funcionassem, mas que também fossem fáceis de entender, modificar e expandir. Um dos grandes desafios era a chamada "lacuna semântica" entre os especialistas de domínio (pessoas que entendem o negócio) e os desenvolvedores (que implementam soluções técnicas). Essa lacuna frequentemente levava a softwares que funcionavam de forma errada ou que eram difíceis de adaptar a mudanças nos requisitos.

A ideia inicial do DDD é voltar à uma modelagem OO mais pura, por assim dizer. Devemos esquecer de como os dados são persistidos e nos preocupar em como representar melhor as necessidades de negócio em classes e comportamentos (métodos). Isso significa que em DDD um `Cliente` pode não ter um *setter* para os seus atributos comuns, mas pode ter métodos com lógica de negócio que neste domínio de negócio pertencem ao `cliente`, como `void associarNovoCartao(Cartao)` ou `Conta recuperarInformacoesConta()`. Em resumo, as classes modeladas e os seus métodos deveriam representar o negócio da empresa, usando inclusive a mesma nomenclatura. A persistência dos dados é colocada em segundo plano, sendo apenas uma camada complementar.

O DDD nasceu da necessidade de aproximar esses dois mundos. Eric Evans observou que o software bem-sucedido em contextos complexos era construído em torno de um **modelo de domínio** que capturava com precisão o conhecimento do negócio. Ele também percebeu que os sistemas mais sustentáveis utilizavam linguagens comuns entre especialistas e desenvolvedores, além de técnicas para isolar a complexidade e tornar o código mais alinhado com as regras do domínio.

Com a evolução do desenvolvimento de softwares e no aumento da complexidade dos requisitos da aplicação, é extremamente relevante definirmos uma comunicação clara entre as várias partes envolvidas em um projeto de software. É bastante comum haver conflitos entre os termos técnicos utilizados pelas diferentes áreas, seja entre analistas de negócios, desenvolvedores, especialistas financeiros ou de vendas. Nada mais natural haja visto que as equipes estão cada vez mais multidisciplinares. Para auxiliar em uma comunicação fluida, os conceitos do DDD — Domain Driven Design, propõem como um dos seus pilares a definição de uma _Linguagem Ubíqua_.

<a href=""><img src="https://github.com/user-attachments/assets/4873d674-b778-448b-a311-26f9307e624f"></a>

O DDD formalizou essas práticas ao introduzir conceitos como **Ubiquitous Language** (Linguagem Ubíqua), o cerne do DDD, que promove a criação de uma linguagem compartilhada entre todas as partes interessadas, e **Bounded Contexts** (Contextos Limitados), que ajudam a dividir sistemas grandes e complexos em partes menores e mais compreensíveis. Além disso, o DDD trouxe atenção para padrões arquiteturais que dão suporte ao domínio, como **Entidades** (Entity), **Agregados** (), **Repositórios** () e **Serviços de Domínio** (), estabelecendo um design centrado na lógica de negócios em vez de nas tecnologias subjacentes.

Para que possamos iniciar uma compreensão acerca de Linguagem Ubíqua (Ubiquitous Language), podemos nos valer da análise semântica do termo ubíquo: `u-bí-quo` (latim _ubiquus_, -a, -um), adjetivo:

- Que está ao mesmo tempo em toda a parte. = `ONIPRESENTE`
- Que tem dom da ubiquidade. = `ONIPRESENTE`
- Que está difundido em todo o lado. = `GERAL, UNIVERSAL`.

De forma conceitual, a linguagem ubíqua é o conjunto de termos e inter-relações que fornecem a semântica da comunicação do domínio, que reflete a visão do negócio. E de forma prática, ao se trabalhar com DDD, entende-se como comunicação de mesma linguagem, em um único modelo, de forma que todos os envolvidos no projeto tenham a mesma compreensão acerca dos termos utilizados. Linguagem ubíqua pode parecer um termo complexo de se compreender, mas outro termo também utilizado para identificar este tipo de comunicação, nos auxilia em uma melhor compreensão: _Linguagem Onipresente_.

**Linguagem Onipresente** é essencialmente os termos, palavras e definições utilizadas por todo o domínio do projeto. É o idioma utilizado no cotidiano da empresa, as terminologias da realidade do negócio. Quando um projeto não respeita a **linguagem do domínio** diversos problemas de comunicação surgem, dificultando o desenvolvimento, implantação e sustentação da solução.

Quando termos utilizados no projeto vão sendo traduzidos, de acordo com o uso em cada departamento, a comunicação se torna anêmica e a assimilação do conhecimento disperso. Em seu livro Domain Driven Design — Atacando as Complexidades no Coração do Software, Eric Evans descreve de maneira clara esta problemática:

> O custo de toda a tradução, além do risco de entendimento errado, é simplesmente muito alto. Um projeto precisa de uma linguagem em comum que seja mais robusta que o mínimo denominador comum.

<a href=""><img src="https://github.com/user-attachments/assets/5ac09617-ba80-4f3f-955a-62bd9dfe77ee" align="right" height="77"></a>

A Linguagem Onipresente (ubiquitous language) não está limitada a diagramas em <a href="">UML (Unified Modeling Languages, ou Linguagem de Modelagem Unificada)</a>, mas principalmente, define em seu vocabulário nome das classes e operações de destaque. Inclui regras para implantar um dicionário uniforme e explícito para o modelo, para que o mesmo possa ser utilizado com o máximo de eficiência possível.

O **Diagram as code** (Diagrama como código) é uma abordagem de criação de diagramas que utiliza código, em vez de ferramentas gráficas, para desenhar e manter diagramas. Essa abordagem permite que os diagramas sejam criados e atualizados utilizando linguagens de programação ou marcadores, em vez de ferramentas de desenho gráfico. A prática de "Diagram as code" (Diagrama como código) pode auxiliar no Domain-Driven Design (DDD), pois é uma prática útil no DDD que ajuda a manter a documentação atualizada, facilita a colaboração, fornece controle de versão e permite a geração automática de diagramas. Vantagens do "Diagram as code" no DDD:

1. **Melhor documentação**: Com o "Diagram as code", você pode manter a documentação do seu modelo de domínio atualizada e sincronizada com o código. Isso ajuda a garantir que a documentação seja precisa e refletida nas mudanças no código.
2. **Modelagem colaborativa**: O "Diagram as code" permite que os membros da equipe colaborativamente trabalhem no modelo de domínio, tornando mais fácil para os desenvolvedores, especialistas em domínio e outros stakeholders discutirem e refinarem o modelo.
3. **Versão e controle**: Com o "Diagram as code", você pode usar sistemas de controle de versão (como Git) para rastrear as alterações no modelo de domínio. Isso ajuda a garantir que todas as alterações sejam documentadas e possam ser revertidas se necessário.
4. **Geração automática de diagramas**: Muitas ferramentas de "Diagram as code" permitem que você gere diagramas automaticamente a partir do código. Isso pode economizar tempo e reduzir a chance de erros manuais.
5. **Integração com o ciclo de desenvolvimento**: O "Diagram as code" pode ser integrado ao ciclo de desenvolvimento de software, permitindo que os desenvolvedores trabalhem no modelo de domínio em paralelo com o desenvolvimento do código.

As ferramentas permitem que você crie diagramas como código, utilizando sintaxes específicas para desenhar os diagramas. Em seguida, elas geram imagens ou diagramas a partir do código. Algumas ferramentas populares para "Diagram as code" incluem:

<a href="https://www.plantuml.com/plantuml/uml/SyfFKj2rKt3CoKnELR1Io4ZDoSa700003"><img src="https://github.com/user-attachments/assets/cd3deff0-176a-4d9b-8735-0a1b2b1d2a33" align="right" height="77"></a>

- Mermaid
- **PlantUML**
- Graphviz
- C4 (abordagem de modelagem de software)

Normalmente os especialistas de um domínio, diretores, administradores, analistas, técnicos, possuem pouca familiaridade com o jargão técnico utilizado no desenvolvimento de software, mas utilizam os jargões próprios de sua área de atuação. A partir desta realidade, os especialistas de um domínio descrevem superficialmente o que necessitam, fazendo com que desenvolvedores criem abstrações que sustentem o design da aplicação. Com isso, uma compreensão uniforme vai se deteriorando exponencialmente.

<a href="https://www.plantuml.com/plantuml/uml/SyfFKj2rKt3CoKnELR1Io4ZDoSa700003"><img src="https://github.com/user-attachments/assets/d51f18a5-193c-49ef-8a83-83f42f1924f5" align="right" height="277"></a>

Como solução a esta dispersão na comunicação, devemos usar a linguagem baseada no modelo de forma exaustiva até que a comunicação seja fluida e compreensível entre os diversos setores envolvidos no projeto. Para que possamos alcançar esta fluência, os especialistas do domínio devem vetar termos ou estruturas que não transmitam uma compreensão clara acerca das funcionalidades envolvidas; os desenvolvedores devem se empenhar no cuidado com ambiguidades ou inconsistências que possam corromper o modelo proposto. Ou seja, é um esforço conjunto entre todos os envolvidos, mas, é essencialmente necessário que ocorra.

Como identificar os especialistas de domínio? Especialistas de domínio são os profissionais envolvidos no dia a dia da operação, nos mais diferentes setores, ou seja, são os “conhecedores” do negócio (stakeholders). Normalmente estes especialistas são analistas, técnicos, engenheiros, podendo ser todo aquele que possui a compreensão acerca do fluxo de operação da empresa. Os especialistas de domínio detém o conhecimento sobre as necessidades e requisitos necessários para o processamento das atividades organizacionais.

<img src="https://github.com/user-attachments/assets/3e5b0f4e-5517-4b6d-a8a8-cd650c6f577d" align="right" height="277">

Em essência, o DDD surgiu para enfrentar a complexidade inerente ao desenvolvimento de software em domínios desafiadores, permitindo que os sistemas sejam projetados de forma que o código seja uma expressão direta das regras e processos do negócio. Com o tempo, o DDD ganhou popularidade e passou a ser usado em diversos contextos, especialmente em sistemas corporativos onde o domínio de negócio é complexo e sujeito a constantes mudanças.

Para o sucesso de um projeto de software, o DDD sugere que tanto especialistas de domínio quanto desenvolvedores devem falar a mesma língua.

A figura acima, ilustra a existência de termos que só os especialistas de domínio conhecem e apresentam expressões somente de caráter tecnológico, os quais são de uso apenas do time de desenvolvimento. Contudo, é necessário que exista um conjunto de termos que devem ser de conhecimento universal, no que se refere ao domínio da aplicação, formando a Linguagem Ubíqua do sistema. A definição de uma linguagem onipresente objetiva principalmente dois propósitos:

- Possibilitar uma comunicação fluida entre os membros de equipes multidisciplinares; Nomear elementos do código da aplicação, como classes, métodos, variáveis, funções, módulos, tabelas de bancos de dados, rotas de APIs, etc.

- Ademais a padronização na comunicação propõe elucidar o significado dos termos, de um forma simples, objetiva e compreensível para facilitar os relacionamentos e associações entre todos módulos necessários.

Qualquer pessoa técnica contribuindo para o modelo deve programar, pelo menos tocar no código, independente do papel desempenhado no projeto. Um responsável por mudar o código deve sempre aprender a expressar o modelo através do código. Todo desenvolvedor deve estar envolvido na discussão sobre o modelo e ter contato com os especialistas do domínio. (EVANS, 2016).

Em seu livro Implementando Domain Driven Design, Vaughn Vernon, pontua que um especialista de domínio tem uma forte influência sobre a linguagem utilizada, devido ao maior conhecimento acerca do negócio, que no final é o contexto imperativo de todo projeto. Estes especialistas tendem a ser influenciados pelos padrões da indústria, contudo, uma linguagem universal deve ser centrada em como o próprio negócio pensa e opera. Ou seja, cada empresa possui seu próprio domínio acerca da execução de seus processos.

Não entenda Linguagem Ubíqua como um conjunto de jargões de negócios sendo impostos ao time de desenvolvimento, e nem mesmo uma sobreposição de termos técnicos sobre o contexto de negócio, mas sim, uma linguagem real que é criada por toda a equipe e que é propagada por toda a corporação.

Compreende-se que haverá discordâncias em relação aos termos utilizados e que estão na mente dos especialistas, mas, a partir do uso aberto da linguagem, a evolução é natural e consolidada por este processo de maturação da comunicação.

O DDD enfatiza a compreensão profunda do domínio do problema e o uso de uma linguagem ubíqua compartilhada entre as equipes de desenvolvimento e especialistas do domínio. Ele propõe a organização do código em torno do domínio do problema, separando-o dos detalhes técnicos e infraestrutura. 

Embora o DDD não seja um design pattern em si, ele pode ser combinado com vários design patterns e princípios de design, como Agregado, Repositório, Especificação, Event Sourcing, entre outros. O DDD fornece diretrizes e conceitos para ajudar na criação de uma arquitetura de software robusta e flexível.

Portanto, podemos dizer que o DDD é uma abordagem de design e uma metodologia de modelagem que pode ser aplicada em diferentes arquiteturas de software, como arquitetura em camadas, arquitetura hexagonal, arquitetura de microsserviços, entre outras. Ele fornece princípios e práticas para projetar e estruturar o código em torno do domínio do problema, visando um modelo de domínio rico, desacoplamento e flexibilidade.

É uma abordagem mais ampla para o design de software que abrange vários conceitos e técnicas. DDD enfatiza a modelagem do domínio, a colaboração entre especialistas do domínio e desenvolvedores, e a criação de um código baseado em um entendimento profundo do domínio do problema.

O DDD deve ajudar na modelagem das classes mais importantes e mais centrais do sistema de forma e diminuir a complexidade e ajudar na manutenção das mesmas, afinal este é o objetivo dos princípios de orientação a objetos.

> [!Important]
> Outro ponto é sobre nós desenvolvedores estarmos compartilhando dados com outros sistemas, as rotinas de integração que recebem ou disponibilizam dados para outros sistemas não devem ser "inteligentes". Muitos desenvolvedores acabam modelando suas classes de negócios tentando resolver as questões internas do sistema e, ao mesmo tempo, pensando em como essas classes serão expostas para outros sistemas. Padrões como DTO (Data Transfer Object) que usam objetos "burros" são mais adequados para isso.

Portanto, o DDD não tenta resolver todos os problemas de todas as camadas de um sistema. Seu foco é na modelagem das entidades principais de negócio usando a linguagem adequada daquele domínio para facilitar a manutenção, extensão e entendimento. Particularmente, eu não seguiria à risca o padrão, até porque existem inúmeros padrões e variações de modelagem OO. Estude os princípios por detrás desses padrões, pois eles são geralmente parecidos e veja o que funciona melhor para cada projeto.

A maioria dos softwares não quebra por causa de erros de sintaxe ou lógica if-else falha.

Ele quebra porque as equipes perdem o alinhamento com o problema de negócios que deveriam resolver. Os sistemas se emaranham com suposições técnicas que envelhecem mal. Os recursos são implementados sem considerações de design adequadas. E com o tempo, cada novo requisito cria mais problemas que continuam se acumulando.

Muitas vezes, isso não é um problema de ferramentas. É um problema de modelagem.

O DDD (Design Controlado por Domínio) tenta resolver esse problema de frente. Em sua essência, o DDD é uma maneira de projetar software que mantém o domínio de negócios, não o esquema de banco de dados ou a estrutura mais recente, no centro da tomada de decisões. Ele insiste que os engenheiros colaborem profundamente com especialistas de domínio durante o ciclo de vida do projeto, não apenas para reunir requisitos uma vez e desaparecer nos tickets do Jira. Ele fornece às equipes o vocabulário, os padrões e os limites para modelar sistemas complexos sem serem enterrados na complexidade acidental.

Claro, o DDD não é uma bala de prata. Ele não gera código e não conserta magicamente um monólito legado. Mas oferece algo mais valioso a longo prazo: clareza sobre o que o sistema deve fazer e onde pode mudar.

Essa abordagem se torna especialmente valiosa quando:

- O domínio não é trivial e continua evoluindo. Pense em finanças, saúde, logística ou mercados gigantes.
- Várias equipes estão trabalhando em partes sobrepostas do sistema.
- O código precisa refletir o comportamento do mundo real, não construções técnicas abstratas.

O DDD não se importa se a arquitetura é monolítica ou baseada em microsserviços. O que importa é se o modelo reflete as regras e a linguagem do mundo real do domínio e se esse modelo pode evoluir com segurança à medida que o domínio muda.

Exploramos as ideias centrais do DDD (como Contextos Limitados, Agregados e Linguagem Ubíqua) e explicamos como eles funcionam juntos na prática. Também veremos como o DDD se encaixa nos sistemas do mundo real, onde ele brilha e onde pode falhar.

Essa divisão natural acaba sendo organizada em três grandes agrupamentos: uma **camada de domínio**, uma **camada de aplicação** e uma **camada de infraestrutura**. Mas, novamente, isso não é um dogma do DDD, é apenas a forma como as ideias do DDD funcionam melhor em arquiteturas limpas e separadas:

<table>
 <tr>
  <td><img src="https://github.com/user-attachments/assets/ee84d4c8-e5d3-4469-9a41-8eed9718659c" height="777"></td>
  <td><img src="https://github.com/user-attachments/assets/29d64a52-176c-46d9-8b54-68b9c6be717f" height="777"></td>
  <td><img src="https://github.com/user-attachments/assets/c7b24ba8-f883-4fcf-a89b-6b864209ccd4" height="777"></td>
 </tr>
</table>

No contexto do DDD, existem design patterns específicos que são frequentemente utilizados para ajudar a implementar os conceitos e princípios do DDD. Alguns desses padrões incluem:

1. <a href="">Agregado</a>: Se refere a um padrão de design que agrupa um conjunto de objetos relacionados em uma única unidade coesa. O Agregado é uma das principais construções utilizadas para modelar e organizar o domínio em DDD;

2. <a href="">Repositório</a>: Fornece uma interface para acessar coleções de objetos agregados, permitindo que o domínio permaneça livre de preocupações com persistência. Ele atua como uma camada intermediária entre o domínio e a fonte de dados (como bancos de dados).

3. <a href="">Serviço de Domínio</a>: Representa operações ou ações do domínio que não pertencem naturalmente a uma única entidade ou value object. Encapsula lógica de negócio que depende de múltiplos objetos.

4. <a href="">Value Object</a>: Objetos que não possuem identidade própria e são definidos apenas por seus atributos. São imutáveis e usados para representar conceitos como dinheiro, coordenadas ou medidas.

5. <a href="">Entidade</a>: Objetos do domínio que possuem identidade própria (geralmente um ID) e um ciclo de vida distinto. Diferente de value objects, entidades podem mudar seus atributos ao longo do tempo.

6. <a href="">Factory</a>: Padrão responsável por encapsular a lógica de criação complexa de objetos, especialmente agregados. Evita a poluição do construtor com lógica de montagem de objetos.

7. <a href="">Especificação</a>: Define regras de negócio reutilizáveis e combináveis para verificar se um objeto atende a determinados critérios. É útil para separação de responsabilidades e clareza das regras de domínio.

8. <a href="">Event Sourcing</a>: Técnica onde o estado do sistema é determinado por uma sequência de eventos (ao invés de snapshots de dados). Permite reconstruir o estado do sistema e ter um histórico detalhado das mudanças.

9. <a href="">Injeção de Dependência (DI - Dependency Injection)</a>: Técnica que permite desacoplar componentes do sistema, facilitando testes, manutenção e extensibilidade. No DDD, é comum para injetar repositórios, serviços de domínio e unidades de trabalho nos agregados e serviços de aplicação.

Esses padrões, juntamente com outros conceitos e técnicas, podem ser aplicados para construir uma arquitetura que segue os princípios do DDD. O DDD, portanto, não é um design pattern em si, mas uma abordagem que pode ser implementada usando diversos padrões de design específicos.

<a href=""><img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/0ade6281-cdca-47d3-8b95-57e81b61d04a" align="right" height="377"></a>

O coração é sempre o **domínio**: entidades, objetos-valor, agregados, repositórios como contratos e os serviços de domínio quando algo não cabe numa entidade específica. Aqui não existe conhecimento técnico como banco de dados, HTTP, mensageria ou UI. É o código que sobrevive quando se troca tudo ao redor. É onde o vocabulário ubíquo vive, onde o modelo mental da empresa vira código executável. É a camada mais estável e a mais valiosa de todas:

Quando você fala dessas **“camadas do domínio”**: entidades, objetos-valor, agregados, repositórios e serviços de domínio, na verdade você está descrevendo **os blocos estruturais internos do próprio Domain Model**, isto é, os elementos que compõem o **núcleo** do DDD. Eles não são camadas no sentido arquitetural, mas sim *componentes conceituais do modelo*, cada um representando um papel distinto dentro da lógica de negócio. E essa distinção é crucial, porque o domínio só fica expressivo e coerente quando cada peça é usada para aquilo que foi criada.

O design orientado por domínio reconhece múltiplos tipos de modelos. Por exemplo, uma entidade é um objeto definido não por seus atributos, mas por sua identidade. Por exemplo, a maioria das companhias aéreas atribui um número único aos assentos de cada voo: essa é a identidade do assento. Em contraste, um objeto valor é um objeto imutável que contém atributos, mas não possui identidade conceitual. Quando as pessoas trocam cartões de visita, por exemplo, elas se importam apenas com as informações do cartão (seus atributos), em vez de tentar distinguir entre cada cartão único.

<img src="https://github.com/user-attachments/assets/28e98845-bfde-4ecb-a5f7-84b24328cdb3" align="right">

Dentro do domínio, as **entidades** representam conceitos que têm identidade persistente ao longo do tempo, mesmo que seus atributos mudem. Elas capturam comportamentos essenciais ligados a um identificador único, como um `Cliente`, um `Pedido` ou um `Veículo`. Já os **objetos-valor** são as estruturas que descrevem características imutáveis, conceituais, que não têm identidade própria, mas têm significado. Eles existem para impedir que o domínio fique cheio de tipos primitivos sem sentido, substituindo-os por tipos ricos, como `Email`, `CPF`, `Placa`, `Endereço` ou `Dinheiro`. Essa relação entre entidades e objetos-valor sustenta a expressividade do vocabulário ubíquo dentro do código.

Modelos também podem definir **eventos** (algo que aconteceu no passado). Um evento de domínio é um evento pelo qual especialistas de domínio se importam. Modelos podem ser ligados por uma entidade raiz para se tornarem um agregado. Objetos fora do agregado podem conter referências à raiz, mas não a qualquer outro objeto do agregado. A raiz agregada verifica a consistência das mudanças no agregado. Os motoristas, por exemplo, não precisam controlar individualmente cada roda de um carro: eles simplesmente dirigem o carro. Nesse contexto, um carro é um conjunto de vários outros objetos (o motor, os freios, os faróis, etc.).

Quando o sistema cresce e você percebe que certas entidades começam a formar agrupamentos naturais de regras e invariantes, entra o conceito de **agregado**. Ele funciona como um limite de consistência: um conjunto de entidades e objetos-valor que sempre deve ser manipulado de forma coerente. O agregado garante que você não mexa em partes internas que não deveriam ser alteradas isoladamente e que toda modificação passe por uma única entidade-raiz. Essa raiz é quem expõe métodos públicos e controla as regras internas do agregado, protegendo sua integridade lógica.

No design orientado por domínio, a criação de um objeto frequentemente é separada do próprio objeto.

Um repositório, por exemplo, é um objeto com métodos para recuperar objetos de domínio de um armazenamento de dados (por exemplo, um banco de dados). De forma semelhante, uma fábrica é um objeto com métodos para criar diretamente objetos de domínio. Já os **repositórios** são contratos dentro do domínio — e isso é importante: contratos, não implementações. Eles definem as operações necessárias para persistir e recuperar agregados, mas não sabem nada sobre banco de dados, ORM, SQL ou infraestrutura. Eles expressam apenas a intenção: “preciso obter esse agregado”, “preciso persistir esse agregado”. A tecnologia que faz isso acontecer vive fora do domínio. O repositório é o ponto de contato mais importante entre o núcleo do domínio e o resto da aplicação, porque permite que o domínio permaneça independente e limpo.

<img src="https://github.com/user-attachments/assets/ee335c88-c613-47f9-8a0c-afbd7f28cc3a" align="right" height="477">

Por fim, os **serviços de domínio** (Domain service) são como espaços auxiliares dentro do modelo. Eles só existem quando uma regra de negócio não pertence naturalmente a nenhuma entidade ou objeto-valor. São operações puramente de domínio, mas sem estado próprio, que coordenam comportamentos entre objetos. 

Muitas vezes representam cálculos, validações complexas, políticas ou decisões de negócio que não cabem dentro de um único agregado. O fato de eles existirem mostra maturidade na modelagem, porque impede que entidades se tornem “deuses” com responsabilidades demais. 

Esse diagrama junta vários conceitos de DDD, microsserviços, Domain Services, CQRS e Event-Driven Architecture, e por isso parece mais abstrato do que realmente é.

O *contextual service* não tem relação com *application context* no sentido técnico de frameworks, mas sim com o contexto de domínio definido pelo DDD. Ele representa um serviço que atua dentro do **bounded context**, carregando as regras de negócio específicas daquele domínio. É um tipo de componente que não é simplesmente uma *service class* de aplicação, mas uma unidade que encapsula conhecimento do domínio e age conforme as regras internas do contexto. Ele existe para isolar o significado, o vocabulário e as invariantes daquele pedaço do sistema, de modo que aquilo que faz sentido dentro daquele contexto não vaze para outro. Ou seja, é um serviço que só funciona dentro do contexto semântico onde ele pertence e é por isso que ele é “contextual”, porque depende do significado local daquele domínio, e não de uma API genérica ou do framework.

Já o *managed state transition event* aparece quando o domínio possui algum tipo de estado que muda com o tempo e essas mudanças têm significado de negócio. Quando um agregado ou entidade passa de um estado para outro, essa transição pode gerar um evento que registra essa mudança para que outras partes do sistema possam reagir. O termo “managed” indica que esse estado é **controlado e validado pelo próprio domínio**, obedecendo invariantes, regras e consistência interna. Portanto, esse tipo de evento é originado quando o domínio aceita, valida e confirma uma mudança de estado, e então emite um evento que pode acionar comportamento assíncrono, projeções, atualizações ou integrações. Não é apenas um evento técnico, mas sim a expressão de uma transformação relevante dentro da lógica da operação.

O *business event*, por sua vez, é o evento de mais alto nível, aquele que traduz uma ocorrência de valor para o negócio. É diferente do managed state transition event porque ele não diz apenas que um agregado mudou seu estado interno, mas que **algo significativo aconteceu dentro da empresa**, algo que outros serviços, contextos e até sistemas externos precisam saber. Esse tipo de evento é emitido quando o domínio reconhece que ocorreu um fato com relevância semântica, como “Pagamento Confirmado”, “Pedido Cancelado”, “Cliente Registrado”. Ele se torna um ponto de integração entre bounded contexts e é geralmente publicado em sistemas de mensageria ou barramento de eventos, servindo de gatilho para fluxos, reações automáticas ou pipelines de consumo. Em termos de EDA e CQRS, é o que permite que projeções atualizem *read models*, ou que outros microserviços sincronizem decisões e comportamentos sem acoplamento direto.

Assim, o diagrama articula três camadas de significado. O contextual service executa lógica de domínio situada no contexto adequado. O managed state transition event registra a mudança interna e valida dentro do domínio. E o business event expõe para o ecossistema aquele fato relevante que deve ser consumido por outros componentes, dando vida à característica distribuída de <a href="https://medium.com/walmartglobaltech/building-domain-driven-microservices-af688aa1b1b8">microservices com DDD e CQRS</a>.

Quando parte da funcionalidade de um programa não pertence conceitualmente a nenhum objeto, ela normalmente é expressa como um *serviço*.

Existem diferentes tipos de eventos no DDD, e as opiniões sobre sua classificação podem variar. Segundo Yan Cui, existem duas categorias-chave de eventos:

- **Eventos de domínio** significam ocorrências importantes dentro de um domínio de negócios específico. Esses eventos são restritos a um contexto limitado e são vitais para preservar a lógica de negócios. Normalmente, eventos de domínio têm cargas úteis mais leves, contendo apenas as informações necessárias para o processamento. Isso ocorre porque os ouvintes de eventos geralmente estão dentro do mesmo serviço, onde seus requisitos são mais claramente compreendidos.

- Por outro lado, **eventos de integração** servem para comunicar mudanças entre diferentes contextos limitados. Eles são cruciais para garantir a consistência dos dados em todo o sistema. Eventos de integração tendem a ter cargas úteis mais complexas com atributos adicionais, pois as necessidades dos ouvintes potenciais podem variar significativamente. Isso frequentemente leva a uma abordagem mais completa da comunicação, resultando em excesso de comunicação para garantir que todas as informações relevantes sejam compartilhadas de forma eficaz.

O que você chamou de “camadas” é, portanto, o conjunto de **padrões que estruturam o modelo de domínio** internamente. Eles servem para que o núcleo do sistema represente a realidade de negócio de forma organizada, expressiva e coerente. Cada um desempenha um papel específico e todos se combinam para formar o coração do DDD. Esses elementos não vivem separados por fronteiras técnicas — eles convivem dentro do mesmo contexto, mas com funções bem definidas. E é exatamente essa organização interna que permite ao domínio permanecer sólido mesmo quando todo o resto do sistema muda.

Ao redor do domínio está a camada de aplicação, que não contém regras de negócio, mas coordena casos de uso. Ela funciona como um orquestrador, chamando o domínio e o que está fora dele para cumprir um fluxo. Esse nível também permanece relativamente estável, mas já conhece elementos mais concretos, como serviços de email, notificações ou repositórios que serão implementados no mundo técnico. Essa camada é a ponte entre a intenção de negócio e a execução tecnológica.

Por fim, a infraestrutura é a camada que toca na realidade: banco de dados, HTTP, mensageria, arquivos, serviços externos, ORM, drivers, tudo que é acoplado à tecnologia. Aqui ficam as implementações concretas dos contratos definidos nas camadas superiores. A infraestrutura depende do domínio, mas o domínio nunca depende dela — essa é a inversão fundamental que mantém a modelagem limpa. Quando se aplica arquitetura hexagonal ou Onion Architecture, o domínio fica no centro e a infraestrutura fica nas bordas, o que reforça a mesma ideia.

Então, quando se fala que DDD tem camadas, a verdade é que ele inspira a criação de camadas porque a modelagem orientada ao domínio exige separação clara entre regras de negócio e tecnologia. É por isso que tantos times que aplicam DDD acabam automaticamente usando Clean Architecture, Hexagonal Architecture ou Onion Architecture: essas estruturas preservam o modelo de domínio e permitem que ele evolua sem ser destruído por detalhes técnicos.

DDD não existe sem essa separação. Ele até poderia ser aplicado em uma bagunça de código monolítico distribuído, mas não funcionaria. O poder do DDD acontece justamente quando o domínio é posto no centro e protegido por camadas que impedem que a tecnologia engula as regras de negócio. Essa divisão natural acaba sendo percebida como “camadas do DDD”, apesar de tecnicamente elas pertencerem mais a estilos arquiteturais compatíveis com DDD do que ao DDD em si.

<img src="https://github.com/user-attachments/assets/b2544370-f786-49e5-8b98-162d68e232b5" align="right" height="377">

O **AOP - Aspect-Oriented Programming** pode fortalecer muito as boas práticas de DDD, TDD e BDD, e essa conexão faz bastante sentido quando entendemos o papel de cada um desses paradigmas dentro de uma arquitetura limpa e organizada. A orientação a aspectos não substitui nenhum deles, mas funciona como uma espécie de tecido estrutural que mantém o código limpo, modular e fiel aos princípios que essas abordagens defendem.

O DDD se beneficia especialmente porque a regra número um do design orientado ao domínio é manter o domínio puro, expressivo e livre de detalhes técnicos acoplados. O AOP ajuda justamente a retirar do domínio tudo aquilo que não é domínio: logs, transações, auditorias, repetição de validações estruturais, políticas de segurança, métricas e qualquer outra funcionalidade transversal. Ao deslocar essas responsabilidades para aspectos, o modelo de domínio permanece limpo e orientado exclusivamente à lógica do negócio, sem anotações excessivas, sem serviços utilitários misturados e sem ruídos que atrapalhem a clareza conceitual do código. Isso deixa o domínio mais próximo da linguagem ubíqua, mais fácil de evoluir e mais coerente com o propósito principal do DDD, que é representar conhecimento e regras do negócio de forma elegante e sustentável.

No caso do TDD, o AOP traz uma contribuição igualmente importante. Quando usamos TDD, queremos testar a lógica de forma isolada, sem que camadas externas interfiram no comportamento esperado. Se o código estiver poluído com logs, tratamentos repetitivos ou preocupações técnicas envolvendo transações ou autenticação, o ato de testar se torna mais difícil, mais lento e mais sujeito a falhas colaterais. O AOP limpa esse cenário ao remover grande parte desse ruído estrutural, permitindo que você escreva testes focados apenas na lógica essencial. Além disso, como os aspectos podem ser desativados ou simulados durante os testes, você consegue um ambiente de testes mais controlado, determinístico e alinhado com o espírito do TDD, que exige ciclos rápidos, previsíveis e com feedback imediato sobre a execução da regra de negócio.

Sobre o BDD, o AOP também se encaixa de maneira natural, porque o BDD exige clareza comportamental e foco na história do usuário ou no comportamento esperado de uma funcionalidade. Quando você descreve um comportamento no formato Given-When-Then, espera que o código reflita essa lógica de forma limpa, sem camadas técnicas misturadas. O AOP impede que esses comportamentos de alto nível fiquem escondidos ou embrulhados por detalhes de infraestrutura, preservando a naturalidade da leitura tanto no código quanto nos testes comportamentais. Isso torna os cenários mais fiéis à linguagem de negócio, diminui ruídos e deixa as tratativas técnicas centralizadas fora do fluxo principal. Em outras palavras, o BDD ganha em clareza, o TDD ganha em eficácia e o DDD ganha em pureza — tudo porque o AOP protege a regra de negócio de interferências externas.

Assim, quando você coloca tudo isso junto, percebe que AOP não é um acessório técnico, mas uma ferramenta arquitetural que sustenta a separação de responsabilidades, reduz acoplamento e melhora a manutenção do sistema como um todo. Ele permite que o domínio seja domínio, que os testes sejam testes e que o comportamento da aplicação seja descrito de maneira simples e coerente. O AOP acaba se tornando um verdadeiro aliado para sistemas que queiram adotar DDD, TDD e BDD de forma madura, escalável e profissional, principalmente em ambientes como o ecossistema Java/Kotlin, onde essa abordagem é amplamente consolidada através de frameworks como o Spring.

<table>
 <tr>
  <td><img src="https://github.com/user-attachments/assets/40876f04-b257-4eca-a7b0-72af3adc66a6" height="777" /></td>
  <td><img src="https://github.com/user-attachments/assets/6f12e517-635b-4959-ac10-0d1c2af6aa25" height="777" /></td>
 </tr>
</table>

**DDD - Segregação de Responsabilidade de Consulta de Comando (CQRS)** os comandos são complexos, as consultas são simples, anteriormente, examinamos as Entidades DDD, que têm **estado**, e **Eventos**, onde o estado muda. Para reduzir a complexidade, podemos ser específicos sobre o que tem estado e encapsular onde ele muda. Os eventos são códigos de alto nível, situados no meio da Onion Architecture. Veremos como os comandos de nível inferior vinculam a interface do usuário ou a API a eventos para permitir que os usuários alterem o estado.

<table>
 <tr>
  <td><img src="https://github.com/user-attachments/assets/6ed3f6e0-e3ec-4cf2-a2ae-cc486f510748" height="777"></td>
  <td><img src="https://github.com/user-attachments/assets/99724450-0a18-4e9e-b5e6-f80af13c47d5" height="777" /></td>
 </tr>
</table>

Os eventos de domínio existem no centro de domínio de alto nível de um diagrama Onion Architecture, coberto por Robert C. Martin em Clean Architecture. A camada externa da cebola contém detalhes de baixo nível, entradas e saídas, como armazenamento, interfaces de usuário e APIs. Os comandos estão em algum lugar no meio, vinculando as entradas ao domínio de nível superior para que os usuários possam acionar os eventos para alterar o estado.

<table>
	<tr>
		<td><img width="720" height="313" alt="image" src="https://github.com/user-attachments/assets/2ed856b3-baf7-49f2-bf70-c4d3c52e17f2" /></td>
		<td><img width="720" height="313" alt="image" src="https://github.com/user-attachments/assets/0402fae7-d682-4b35-ba61-7cc365ab3909" /></td>
	</tr>
</table>

Para que um usuário interaja com um sistema e para que ele seja útil, precisamos ser capazes de fazer duas coisas. A primeira é exibir informações para o usuário.

![Screenshot_20251207-215042_Instagram](https://github.com/user-attachments/assets/56297bc0-d597-4148-b26a-acdeb5daa9e7)

O Clean Architecture (CA) é a diretriz de arquitetura de sistemas proposta por Robert C. Martin (Uncle Bob) derivada de muitas diretrizes arquitetônicas como Hexagonal Architecture e Onion Architecture, entre outras. Eric Evans introduziu o conceito de Domain-Driven Design (DDD). Ele escreveu sobre isso em seu livro Domain-driven Design em 2004 (também conhecido como "The Big Blue Book"). O Design Orientado a Domínio é uma abordagem para o desenvolvimento de software que centra o desenvolvimento na programação de um modelo de domínio com uma rica compreensão dos processos e regras de um domínio.

<table>
 <tr>
  <td>Hexagonal Architecture + DDD</td>
  <td>Hexagonal Architecture + Clean Architecture + DDD</td>
 </tr>
 <tr>
  <td><img src="https://github.com/user-attachments/assets/5cf836ff-c109-4afe-9dec-8fb33455bb30" height="777"></td>
  <td><img src="https://github.com/user-attachments/assets/26e7d71b-c8bc-407c-8370-2914904f0306" height="777" /></td>
 </tr>
</table>

Comecei com minha equipe a adotar o Domain-Driven Design (DDD) em nosso trabalho, e nossa missão era tirar o máximo proveito do DDD e do CA, se possível. À medida que a adoção cresce, estamos cada vez mais perto do negócio e do domínio que estamos abordando; começamos a falar a linguagem onipresente do domínio.

<table>
 <tr>
  <td><img height="310" src="https://github.com/user-attachments/assets/223fb00f-a4ad-4ce4-a3ed-97ca8c5a2f3b" /></td>
  <td><img width="800" height="310" alt="hexagonal-architecture-vs-clean-architecture-2 v4-800x310" src="https://github.com/user-attachments/assets/293ade6d-7009-4466-be85-f404646b82aa" /></td>
 </tr>
</table>

> [!Note]
> Não existe tal arquitetura que sirva para todos. Toda arquitetura ou padrão de desenvolvimento de software tem prós e contras; Baseie sua decisão no projeto, no escopo e na equipe. Vamos descrever o caminho que tomamos.

Exemplo: DDD + Hexagonal Architecture - GalleryManager

<img src="https://github.com/user-attachments/assets/e5af5f61-d5e1-4d2f-af36-cab98828ac36" />

Nos concentraremos em como estruturamos o código de acordo com DDD e Clean Architecture, para que o código também fale a linguagem onipresente do domínio com mais facilidade:

Primeiro, dividimos o sistema em partes independentes menores em torno dos subdomínios de negócios por meio de algumas iterações (ferramentas <a href="https://vaadin.com/blog/ddd-part-1-strategic-domain-driven-design">estratégicas de DDD</a>, como tempestade de eventos, narrativa e muito mais). Idealmente, essas partes devem ser implantáveis de forma independente (microsserviços), mas nem sempre é esse o caso. Muitas vezes, podemos ter um código legado que não podemos alterar facilmente, então temos que mantê-lo por um tempo. Nesses casos, temos esses subdomínios em um único projeto (monólito), com cada subdomínio em uma pasta ou pacote separado.

**Estrutura de código de contexto limitado (Bounded Contexts)**: Depois de dividir o domínio extenso em partes menores, também chamadas de subdomínios. Em seguida, tentamos resolver cada subdomínio; Um "contexto limitado" implementará um subdomínio. Cada contexto limitado pode ser um microsserviço separado ou um pacote separado que encapsula esse contexto limitado dentro de um serviço atual. Então, vamos falar sobre essa parte agora, como projetamos cada contexto limitado, quantas camadas de alto nível temos e como elas se comunicariam juntas.

Exemplos de contextos limitados em um sistema de comércio eletrônico

```txt
├───wallet       
├───orderManagement
├───shipping  
├───..
```

<img src="https://github.com/user-attachments/assets/bbbd4c71-4a40-475a-aecb-f934ad00bd1d" align="right">

**Comando vs. Consulta (CQRS)**: A primeira camada que temos em cada contexto limitado são comandos e consultas. O que eles significam?

Todo caso de uso em um sistema pode ser considerado um Comando ou Consulta, onde um Comando é qualquer caso de uso que altera o estado atual do sistema, enquanto uma Consulta é qualquer caso de uso que busca o estado atual SEM mudar o estado atual. Como esses dois têm preocupações diferentes, decidimos usar o padrão CQRS (Command Query Responsibility Segregation)

Então, temos pastas de nível muito alto; Cada uma contém o restante das camadas, que discutiremos mais adiante nesta página para isolar essas duas preocupações.

```txt
├───shipping
|   ├───commands
|   ├───queries
```

**Camadas de Arquitetura**: Ter camadas claras em nosso código onde cada camada tem responsabilidade clara torna adequado para nós identificar a direção da dependência, testar facilmente o código, trabalhar em paralelo sem esperar uns pelos outros, e muito mais.

Concordamos em ter as seguintes camadas

- Camada de domínio
- Camada de Aplicação
- Camada de Infraestrutura

```txt
├───shipping
    ├───commands
        ├───application
        ├───domain
        ├───infrastructure
    ├───queries
        ├───application
        ├───infrastructure
```

Você provavelmente percebeu que a subpasta de consultas não tem camada de domínio! A seção a seguir explicará os motivos por isso.

**Camada de domínio**: A camada de domínio é a parte central de um contexto limitado, contendo o domínio central e todos os invariantes de negócios e a lógica para esse contexto limitado. Não deve depender de nenhuma camada ou biblioteca ou framework de terceiros. Em vez disso, todas as camadas dependem disso. O conteúdo típico nessa camada é o seguinte.

```txt
├───shipping
    ├───commands
        ├───domain
            ├───models
               ├───Shipment
               ├───Order
               ├───ShippingCompany
               ├───OrderStatus
               ├───Receiver
            ├───services
               ├───ShippingService
            ├───events
                ├───ShipmentCreated
                ├───ShipmentDelievered
            ├───contracts
                ├───ShipmentRepo
                ├───OrderRepo
                ├───ShippingCompanyProvider
```

**Componentes do Domínio**: Resumindo, temos modelos de domínio, serviços de domínio, eventos e contratos. Existem principalmente três tipos de modelos de domínio que envolvem a lógica de negócios:

- AggregateRoot,
- Entidade, e
- Objeto de valor.

E qualquer código que não se encaixe em nenhum desses modelos deve ir para um serviço de domínio. Também temos os eventos produzidos pelo **AggregateRoots** sempre que algo muda no modelo. E, por fim, os contratos/interfaces para qualquer domínio de implementação de infraestrutura que possam precisar.

**Camada de aplicação**: Essa camada fina atua como uma API que expõe as funcionalidades do contexto limitado por meio de casos de uso.

É o cliente direto do modelo de domínio, responsável pela coordenação de tarefas (orquestração) dos fluxos de casos de uso. Além disso, ao usar um banco de dados ACID, a camada de aplicação controla as transações, garantindo que a aplicação persista atômicamente as transições de estado do modelo.

> [!Note]
> Nota: É um erro considerar o caso de uso da Aplicação igual ao dos **Serviços de Domínio**. Eles não são. O contraste deve ser marcante. Devemos nos esforçar para colocar toda a lógica de domínio de negócios no modelo de domínio, seja em Agregados, Objetos de Valor ou Serviços de Domínio. Mantenha os Serviços de Aplicação enxutos, usando-os apenas para coordenar tarefas no modelo. (Vaughn Vernon)

Uma camada típica de aplicação consiste em duas pastas, conforme segue:

```txt
├───shipping
|   ├───commands
|       ├───application
|           ├───usecases
|              ├───CreateShipment
|              ├───OrderConfirmedEventHandler
|           ├───models
|               ├───CreateShipmentRequest
|               ├───OrderConfirmedEvent
|   ├───queries
|       ├───application
|           ├───usecases
|              ├───ListShipments
|           ├───models
|              ├───ListShipmentsQuery
```

Implementamos uma classe separada por caso de uso; Cada classe contém um único método chamado executar algo como <a href="https://refactoring.guru/design-patterns/command">padrão de comando</a>

Existem três tipos de casos de uso:

1. **Solicitar para fazer algo** (`CriarEnvio`, `AtualizarStatusEnvio`)
2. **Consultar algo** (`GetShipments`)
3. **Manipulador de Eventos** (`OrderReceivedEventHandler`)

**Camada de infraestrutura**: O trabalho da infraestrutura é fornecer capacidades técnicas para outras partes da nossa aplicação. Ele contém qualquer implementação de banco de dados, IOs ou rede, como MongoDB, Postgres, serviços analíticos, controladores, acesso ao sistema de arquivos ou cache de memória.

É útil manter uma mentalidade de Princípio da Inversão de Dependência. Então, onde quer que as camadas de aplicação ou domínio precisem de detalhes de infraestrutura, dependemos de interfaces. Então, quando um caso de uso de aplicação consulta um repositório, ele dependerá apenas da interface do modelo de domínio, mas usando a implementação da infraestrutura.

Um diagrama simples para ilustrar como isso funciona é o seguinte.

![1_avfevQaNbjyHxKj9D4YYJQ](https://github.com/user-attachments/assets/09dd1b31-43f0-4a0b-9345-170c40d48d99)

O Serviço de Aplicação depende da interface do Repositório do modelo de domínio, mas utiliza a classe de implementação da infraestrutura. Os pacotes abrangem amplas responsabilidades.

```
├───shipping
|   ├───commands
|       ├───infrastructure
|           ├───controllers
|           ├───services
|           ├───repositories
|           ├───..
```

**Repositórios**: Repositórios são classes ou componentes que encapsulam a lógica necessária para acessar fontes de dados. Eles centralizam funcionalidades comuns de acesso a dados, proporcionando melhor manutenção e desacoplando a infraestrutura ou tecnologia usada para acessar bancos de dados a partir da camada do modelo de domínio.

Para cada agregado ou raiz agregada, você deve criar uma classe de repositório.

Criamos uma classe de repositório para cada agregado ou raiz agregada, já que a raiz agregada não permite acesso direto às suas entidades filhas para impor variantes agregadas. Precisamos puxar todo o agregado do banco de dados, realizar ações e salvá-lo.

> Dito isso, tenha cuidado ao projetar seu agregado para evitar penalidades de desempenho. Por exemplo, não projete uma raiz agregada contendo uma lista de entidades que aumenta ao longo do tempo. Você precisará extrair uma parte significativa dos dados toda vez que operar com esse agregado. Como resultado, você pode acabar com uma operação muito lenta e, pior ainda, OutOfMemory!.

Algo como uma raiz agregada de carteira com uma lista de transações é um exemplo de um design ruim desse tipo; A transação de uma carteira aumenta com o tempo. Existem múltiplas soluções para esses casos; Uma delas é usar event sourcing.

O último ponto a mencionar aqui é que o repositório esconde diferentes fontes de dados usadas da camada de domínio para que possa usar MongoDB e Redis sem alterações na interface.

**Controladores**:
- Nos esforçamos para ter um único controlador por API. Por exemplo, `GetUserController` e `SaveUserController`. Um controlador único por API mantém os controladores menores e diretos ao ponto.
- Um controlador recebe a solicitação, a mapeia para o modelo de Aplicação, chama o caso de uso apropriado da aplicação e mapeia o resultado para a entidade de resposta desejada.

**Como é um fluxo completo?** Os dois diagramas a seguir explicam a implementação de cada fluxo típico.

<table>
 <tr>
  <td>Fluxo Típico de Comando:</td>
  <td>Fluxo típico de consulta:</td>
 </tr>
 <tr>
  <td><img src="https://github.com/user-attachments/assets/105e10ee-f3ab-45fe-a6de-5ca671d335c2"></td>
  <td><img src="https://github.com/user-attachments/assets/1dbbc0f6-9d52-4a4a-9136-8ea68e554d93"></td>
 </tr>
</table>

Novamente, não existe uma arquitetura que sirva para todos. Toda arquitetura ou padrão de desenvolvimento de software tem prós e contras; Baseie sua decisão no projeto, no escopo e na equipe.

**Padrões de Arquitetura de Integração Empresarial - Redações sobre arquitetura**

<img width="720" height="484" alt="image" src="https://github.com/user-attachments/assets/0943cefd-3069-43a6-8c6f-e9609ca22a56" />

A perspectiva: Sistemas de TI interagem e, portanto, se integram pelos mesmos motivos que as pessoas.

1. Quando precisamos de informações de outras pessoas para o nosso trabalho
2. Quando precisamos de alguém para fazer algo por nós
3. Quando queremos socializar com alguém

Os exemplos correspondentes de TI são uma chamada de API para uma consulta, uma operação e um cheeping de keep-alive/checagem de saúde (com IA, pode surgir uma verdadeira socialização entre sistemas de TI). Eles também são os tipos de interação mais comuns para os menos comuns.

A empresa se preocupa com a interação entre sistemas tecnológicos e os humanos envolvidos nos processos de negócios. Estes últimos podem ser clientes, funcionários e parceiros. Nem tudo pode ser automatizado, e há humanos nas extremidades ou dentro de sequências de eventos, e precisamos torná-los igualmente parte da solução.

A integração de sistemas é cara e frequentemente o ponto de falha. Assim como nas pessoas, os seguintes princípios tornam a interação entre os sistemas rápida, eficiente e espaçosa.

1. A especialização de responsabilidades (coesão)
2. A falta de importância de saber como algo funciona ou fornece informação (acoplamento frouxo)
3. Uma comunalidade de linguagem (protocolos padronizados)

**Como pensar em integração**: Integração não é apenas HTTP, REST e algum FTP ou SQLNet antigo em segundo plano. É uma área arquitetônica e disciplina interessante e complexa. Não existe uma única forma de encarar isso. Eu vejo isso sob seis pontos de vista que nos permitem criar requisitos sólidos de arquitetura de integração, declarações de problemas e soluções.

Esses pontos de vista de integração, dos mais amplos aos mais detalhados, são

Escopo da integração empresarial → Hierarquia de padrões de integração empresarial → Padrões de integração de aplicações → Integração horizontal das camadas dos sistemas → integração sem estado versus com estado → Segurança da integração

(Usaremos terminologia arquitetonicamente relevante do Design Orientado por Domínio, especialmente os termos específicos de DDD para camadas — UI, Aplicação, Domínio e Infraestrutura. Outros termos DDD estão em itálico. Por favor, consulte meus artigos sobre Arquitetura Orientada por Domínio Parte I e II.)

Uma vez que você entenda a integração sob os pontos de vista abaixo, poderá definir e resolver problemas de integração de forma holística, eficiente e eficaz.

**Ponto de Vista 1: O escopo da integração empresarial**: É útil começar com uma visão de onde as interações estão acontecendo, pois isso influencia sua natureza e soluções.

**Intra-Domínio**: Integrações dentro de um domínio de negócios são as mais comuns. Eles conectam sistemas relacionados com arquitetura e modelos de design semelhantes (assumindo o Domain Driven Design). Isso permite mapas de contexto mais simples entre contextos limitados e integrações mais diretas, com menos preocupações de capacidade e escalabilidade: por exemplo, integração entre um sistema de Gestão de Estoque e um Sistema de Compras.

**Interdomínio**: As integrações entre domínios de negócio são menores, mas apresentam mais desafios. A Linguagem Ubíqua provavelmente diferirá em cada domínio, e a carga útil de dados e os objetos de resposta frequentemente precisam ser transformados nas interações. A infraestrutura também pode ser separada um pouco ou muito, introduzindo a necessidade de várias funções de suporte (veja ponto de vista #2 abaixo) para uma integração bem-sucedida, por exemplo, integração entre um Sistema de Gerenciamento de Pedidos no domínio de vendas com um Sistema de Gerenciamento de Relacionamento com o Cliente no domínio de atendimento ao cliente.

**Inter-Empresas**: A integração entre empresas parceiras em cenários B2B e B2B2C está aumentando exponencialmente com os serviços modernos de web e digitais. Felizmente, os padrões de integração de serviços e serviços em nuvem acompanharam as arquiteturas emergentes da web, mobile e digital, atendendo às necessidades de serviços integrados confiáveis, rápidos e rápidos em escala, seguros e ágeis, desenvolvendo serviços integrados que abrangem de duas a dezenas de empresas em ecossistemas como eCommerce, logística, viagens, automotivo, manufatura, companhia aérea, bancos e serviços financeiros.

A imagem abaixo ilustra esse ponto de vista:

![1_z2eWnKg4fEFYP58W-pwNiQ](https://github.com/user-attachments/assets/fb4185f4-7d02-47bb-9583-f5b74695f830)

**Diretrizes**: Considere cada tipo de integração acima separadamente por suas características e os cinco pontos de vista abaixo para personalizar as arquiteturas de integração.

**Ponto de Vista 2: Hierarquia dos padrões de integração empresarial - Hierarquia de funções de negócio**

- **BPM** — A gestão de processos de negócios coordena pessoas, sistemas, informações e coisas para produzir resultados de negócios para os domínios e subdomínios da empresa. Exemplos são design de produto, fabricação, marketing, aquisição de clientes, vendas, etc. A arquitetura BPM automatiza a integração dinâmica dos processos de negócios na máxima medida possível para fornecer resultados bem definidos, repetíveis, eficientes e confiáveis.

- **Fluxo de trabalho** — Um fluxo de trabalho é uma sequência definida de tarefas realizadas por sistemas e humanos trabalhando juntos para entregar uma tarefa de negócio. Pode ser considerado um subconjunto de um processo de negócios. Um exemplo é o fluxo de aprovação de um empréstimo empresarial. A arquitetura de workflow integra sistemas de TI e humanos para a iniciação, roteamento, suporte analítico à decisão, etapas manuais, tarefas automatizadas, coordenação e monitoramento dos fluxos de trabalho.

- **Integração de sistemas** — Em um cenário de TI bem projetado, a funcionalidade é dividida em sistemas coesos que mapeiam capacidades de domínio e subdomínio de negócio. Esses sistemas devem trabalhar juntos para entregar resultados úteis para fluxos de trabalho e processos de negócios. A integração de sistemas automatiza a cooperação dinâmica deles. (Leia este artigo para saber mais sobre os tipos de sistemas que precisam ser integrados → Uma Abstração Prática de Sistemas de TI Funcionais.)

- **Integração de componentes** — Todos os sistemas de TI são segregados internamente em componentes e subcomponentes coesos e fracamente acoplados. Esses são integrados usando padrões padrão (veja ponto de vista #4 abaixo) para entregar as funções externamente úteis do sistema.

A imagem abaixo ilustra esse enquadramento:

![1_3RtjdjHqylQ18CN8N9WmGw](https://github.com/user-attachments/assets/d758ba0e-a9ea-4ed2-b1a8-e1ce9f679682)

**Hierarquia técnica de funções**: A integração é cara e deve ser o mais simples possível. O quão difícil e propenso a problemas será depende da maturidade dos sistemas de TI (ou seja, aplicações). Quando sistemas/serviços cliente e servidor se comunicam como parte de um processo de negócio, algumas ou todas as seguintes funções podem ser necessárias.

1. **Retentando** — o servidor não responde na primeira tentativa
2. **Mensagens** — o servidor não pode ser contatado diretamente
3. **Gerenciamento de carga** (fila, balanceamento, pooling de conexão) — o servidor pode responder a um número limitado de solicitações por unidade de tempo
4. **Publicar-assinar** — o servidor possui informações que um ou mais consumidores podem obter enquanto estão atualizadas
5. **Transformação de objetos** — o cliente e o servidor trabalham com pacotes de dados suficientes, porém diferentes.
6. **Transformação de protocolo** — cliente e servidor não usam o mesmo protocolo de comunicação
7. **Conversão sincronizada** — o cliente espera uma resposta online enquanto o servidor é projetado para uma resposta offline ou espera uma resposta offline enquanto o servidor é projetado para uma resposta online.
8. **Fusão de funções ou dados** — o cliente deve ser atendido a partir de uma combinação de mais de uma operação ou repositório de informações.
9. **Roteamento** — o servidor correto deve ser alcançado com base em regras
10. **Orquestração** — uma sequência de operações deve ser realizada para responder ao cliente, e a lógica está em um único lugar. (Coreografia é um conceito relacionado, onde a lógica de ação e sequência são distribuídas nos serviços participantes; no entanto, sua capacidade funcional é limitada, e geralmente há um orquestrador centralizado de algum tipo, mesmo que seja apenas um conjunto de regras de referência passivo.)
11. **Gerenciamento de versões** — diferentes clientes precisam de versões diferentes da mesma operação
12. **Segurança** (veja ponto de vista #6 abaixo) — o cliente e o servidor precisam ser protegidos de uma ou mais maneiras

Quanto mais dessas necessidades os sistemas cliente e servidor atendem internamente, menos o arquiteto de integração precisa fornecê-las externamente. Em outras palavras, a arquitetura da aplicação e da informação influenciam significativamente a complexidade e o custo da arquitetura de integração para construir e operar.

Normalmente, haverá algumas funções de integração externas que precisamos atender. Mas quanto mais direta e simples a integração, melhor.

**Padrões e plataformas de soluções de integração intermediária**: Os padrões de solução de integração externa são os seguintes, em ordem crescente de escopo. Tecnicamente, eles não são padrões arquitetônicos, e alguns se sobrepõem funcionalmente. Então, compreenda as diferenças deles e use os termos com cuidado.

1. **RPC** — uma chamada de procedimento remoto (RPC) é quando um programa de computador faz com que um procedimento (sub-rotina) seja executado em um espaço de endereçamento diferente (comumente em outro computador em uma rede compartilhada), codificado como se fosse uma chamada de procedimento comum (local), para simplificar a programação e não precisar lidar com detalhes de rede, protocolo e sistema operacional, etc.

2. **Integração intra-app** — interações entre as camadas de UI, aplicação, domínio e repositório de um sistema (termos DDD; ou UI, lógica de negócio e camadas de banco de dados em terminologia mais antiga), por exemplo, entre a interface e a camada de lógica de negócios (usando protocolos HTTP(s)) e entre a lógica de negócio e a camada de banco de dados (usando TNS/TTC sobre protocolos TCP/IP para o Oracle DB).

3. **API de Leitura (DAL)** — uma API de leitura ou Camada de Acesso a Dados é uma camada comum de integração em Fontes de Dados Operacionais (ODS), Bancos de Dados de Sistemas de Informação de Gestão (MIS DBs) e camadas de negócios de BI acessadas por transações de leitura OLTP e OLAP.

4. **API** — Uma Interface de Programação de Aplicações é uma interface de software para comunicação entre sistemas de TI. Uma API geralmente suporta múltiplas operações. O projeto é guiado pela padronização das assinaturas de funções e protocolos de rede, e um documento de especificação da API é publicado. APIs frequentemente possuem várias versões disponíveis para diferentes clientes. A descoberta dinâmica e a vinculação de APIs e operações por clientes durante a execução também podem ser suportadas.

5. **API GW** — um API Gateway realiza uma combinação de padrões arquitetônicos como fachada, adaptador, mediador e (reverso) proxy. Ele recebe chamadas de clientes e as roteia para os serviços que estão por detrás dele, enquanto fornece funções como roteamento, limitação de taxa, transformação de protocolo, agregação, segurança, versionamento, logs, etc.

6. **Sistemas de Mensagens** — o padrão de integração de mensagens permite que os sistemas sejam acoplados de forma fraca por meio da comunicação assíncrona, tornando a comunicação mais confiável porque os dois sistemas não precisam funcionar simultaneamente. O sistema de mensagens é responsável por transferir dados de um sistema para outro, para que possam focar nas informações que precisam compartilhar e não gerenciar a interação ativamente. É como um serviço de cartas postal.

7. **Sistemas de Fila (de Mensagens)** — o padrão de fila estende o padrão de comunicação assíncrona da Mensagem, fornecendo um pipeline onde múltiplas mensagens podem ser armazenadas sequencialmente por sistemas clientes ou servidores até que sejam consumidas, geralmente em um sistema de Primeiro Entrado, Primeiro a Sair (FIFO), ou se tornem obsoletas. Mensagens de solicitação são colocadas em filas pelos sistemas clientes e captadas e atendidas com mensagens em filas de resposta pelos sistemas de serviço. Filas aumentam a confiabilidade e o throughput líquido e reduzem a perda de dados. Esse acoplamento frouxo permite o desenvolvimento independente e ágil dos sistemas. Gerenciar as filas e seu conteúdo, envelhecimento, escalonamento, registro, etc., são funções fornecidas pela plataforma de fila de mensagens. É como fazer fila para comprar um ingresso para um filme.

8. **Sistemas de Publicação-Assinatura** — o padrão de publicação é um padrão de comunicação assíncrono e fracamente acoplado para que um sistema de serviço disponibilize informações ou funções às quais clientes interessados possam se inscrever. É como publicar jornais e assinar por leitores interessados.

9. **ESBs** — Um Barramento de Serviços Empresariais combina múltiplas funções de integração, como mensagens, fila, publicação-assinatura, roteamento, transformação de protocolo, transformação de objetos, etc., em uma única plataforma de software. Elas são uma das plataformas EAI mais comuns (veja abaixo).

10. **Plataformas EAI** — de modo geral, as plataformas de Integração de Aplicações Empresariais podem fornecer todas as 12 funções de integração abordadas na seção de Hierarquia de Funções Técnicas acima e os tipos de solução 2 a 9 acima.

11. **Gerentes de Fluxo de Trabalho** — Plataformas de fluxo de trabalho integram os sistemas e as pessoas para a iniciação, roteamento, suporte à decisão, ações manuais, tarefas automatizadas, coordenação e monitoramento da sequência de etapas realizadas por sistemas e humanos juntos para uma tarefa de negócio.

12. **Gerentes de Processos de Negócios** — Plataformas BPM automatizam a integração dinâmica dos processos de negócios para fornecer resultados bem definidos, repetíveis, eficientes e confiáveis. Eles geralmente cobrem serviços de descoberta, análise e otimização.

**Diretrizes**: O que é necessário para a integração surge organicamente da arquitetura de aplicações e informações e dos processos e fluxos de trabalho de negócios que eles atendem. Mas, às vezes, há uma decisão a ser tomada se devemos refatorar aplicações para melhor integração ou usar uma plataforma externa.

O teste de tornasol mostrado abaixo nos ajuda a identificar a necessidade de apoio externo. Se a pontuação for baixa, é recomendável refatorar as candidaturas.

![1_PK-NK06VqiotZH4pAYFX1w](https://github.com/user-attachments/assets/af65c83d-26d1-47af-a9fb-8a851c2426d8)

**Ponto de Vista 3: Padrões de integração de aplicativos**: Desde o início, os padrões de design de aplicações incluíram padrões de integração. Alguns desses fatores estão alinhados com o pensamento arquitetônico; Podemos nos adaptar e adotá-los. O livro 'Gang of Four' sobre Padrões de Design de Aplicações aborda os seguintes temas arquitetonicamente relevantes, que são brevemente descrevidos. Como arquiteto de aplicações e integração, aprenda e use esses padrões.

- **Facade** — Fornece uma interface unificada para um conjunto de interfaces em um subsistema. A Facade define uma interface de nível superior que torna o subsistema mais fácil de usar. Por exemplo, uma fachada de API para Order reúne as interfaces de múltiplos subsistemas subjacentes, como ManageStock, CheckPayment, FulfilOrder, etc.

- **Adapter** — Converte a interface de uma classe em outra interface que os clientes esperam. O adaptador permite que classes trabalhem juntas que, de outra forma, não poderiam por causa de interfaces incompatíveis. Em termos arquitetônicos, pense em sistema, aplicação, componente ou subcomponente em vez de classe. Por exemplo, um PaymentGWAdapter preenche um campo de tipo cliente obrigatório exigido por uma interface de sistema de pagamento com um valor padrão para um cliente que não o fornece.

- **Proxy** — Fornece um substituto ou substituto para outro objeto controlar o acesso a ele. Funcionalmente, eles podem ser ainda divididos em Proxy Remoto (representação local de uma API remota), Proxy Virtual (fornece cache e acesso backend sob demanda), Proxy de Proteção (acesso de controle baseado em funções e regras) e Proxy Auxiliar (fornece serviços adicionais como contagem, registro, etc.). Por exemplo, uma CDN (rede de entrega de conteúdo) usa um proxy reverso para segurança, balanceamento de carga e escalabilidade.

- **Observer** (também conhecido como Publicar-Assinar) — Define uma dependência de um para muitos entre objetos para que todos os seus dependentes sejam notificados e atualizados automaticamente quando um objeto muda de estado. (O padrão de Arquitetura Orientada a Eventos é um caso de um padrão de integração de aplicação por observador ou publicação-assinatura.) Por exemplo, se o cronograma de voo de uma companhia aérea (assunto) mudar e vários portais de viagem (observadores) precisarem saber disso, um padrão de Observador ou Publicar-Assinar os integra usando notificações, solicitações, etc.

- **Mediator** — Define um objeto que encapsula como um conjunto de objetos interage. Mediador promove o acoplamento frouxo ao impedir que objetos se refiram explicitamente uns aos outros e permitir que você varie sua interação de forma independente. Por exemplo, uma plataforma de comércio eletrônico se comunica com vários gateways de pagamento por meio de um mediador para que todos possam mudar de forma independente.

- **Camada Anticorrupção** (esse padrão vem do DDD) — Quando sistemas baseados em diferentes modelos são combinados, a necessidade do novo sistema se adaptar à semântica do outro sistema pode levar à corrupção do modelo do novo sistema. Crie uma camada isolante para fornecer aos clientes funcionalidades em termos do modelo de domínio deles. A camada se comunica com o outro sistema por meio de sua interface existente, exigindo pouca ou nenhuma modificação no outro sistema. Internamente, a camada se desloca em ambas as direções conforme necessário entre os dois modelos. Por exemplo, um aplicativo de banco móvel comunica-se com um sistema bancário central legado por meio de uma ACL que separa a verificação de crédito das ordens combinadas em uma única função no sistema legado.

**Diretrizes**: Adote o <a href="https://medium.com/analysts-corner/domain-driven-architecture-design-for-excellent-it-systems-ii-primer-5ae6c6b8f7de">Design de Arquitetura Orientado por Domínio</a>, pois ele leva naturalmente aos contextos limitados, arquiteturas de subdomínio e mapas de contexto que orientam a escolha dos padrões de integração intra e inter-sistema.

**Ponto de Vista 4: Integração horizontal das camadas dos sistemas**

**Integração horizontal na camada UI**: As integrações horizontais na camada de UI estão aumentando, impulsionadas pela tendência de 'montar' aplicações combinando serviços prontos para uso, como buscas de produtos, portais de comércio eletrônico, gateways de pagamento, etc. Vamos considerar isso nos três tipos típicos de interfaces.

1. **Aplicações Estáticas de Página Única (SPAs)** — São aplicativos mais simples, onde toda a funcionalidade está contida em uma única página, totalmente atendida por um ou mais sistemas backend. Por exemplo, Gmail, Google Maps, Twitter, Facebook, etc. A integração de interface horizontal é menos comum em SPAs.
2. **Aplicações Multi Page Estáticas (SMPAs)** — Cada página nessas interfaces fornece um conjunto coeso de funcionalidades do usuário, por exemplo, uma interface ERP. Existem diferentes páginas para contas de usuário, pedidos, suporte, etc. Cada página pode ser bastante independente das outras e conectada a um componente backend separado ou a sistemas parceiros 'white label'. Eles estão integrados de forma frouxa em um portal web ou aplicativo móvel, mas o visual e a sensação são consistentes em todas as páginas.
3. **Aplicações Dinâmicas Multi Página (DMPAs)** — Nessas aplicações, existe um conjunto central de páginas conectadas aos componentes principais do backend, mas as tarefas do usuário também percorrem páginas povoadas por sistemas em outros domínios da mesma empresa ou por sistemas de parceiros, todos os quais podem não ser 'white label'. Por exemplo, um site de comércio eletrônico. Nesses casos, a aparência e a sensação das páginas externas podem ser um pouco ou muito diferentes e mudar com o tempo. Também pode variar entre versões web e mobile da mesma tarefa.

A maior parte da integração horizontal da camada de interface é realizada pela integração horizontal da camada de aplicação (DDD) conforme abaixo, incluindo projetos como portais com uma coleção de portlets de diferentes sistemas.

**Integração horizontal na camada de aplicação**: Eric Evans define a camada de aplicação para DDD como 'Define os trabalhos que o software deve realizar e objetos de domínio expressivos para resolver problemas. As tarefas pelas quais essa camada é responsável são significativas para o negócio ou necessárias para a interação com as camadas de aplicação de outros sistemas. Essa camada é mantida fina. Ele não contém regras de negócio ou conhecimento, mas apenas coordena tarefas e delega trabalho para colaborações de objetos de domínio na camada seguinte. Não possui um estado que reflita a situação do negócio, mas pode ter um estado que reflita o progresso de uma tarefa para o usuário ou para o programa.'

Por sua natureza, a camada de aplicação pode se integrar horizontalmente a sistemas externos, desde que haja pouca ou nenhuma necessidade de preparar os dados para a camada de apresentação ou de persistir dados conforme as regras de negócio no backend. Esse tipo de integração horizontal da camada de aplicação (por exemplo, Javascript rodando no navegador) está aumentando, impulsionado pela tendência de 'montar' aplicações combinando serviços prontos a usar, como catálogos de produtos e serviços, eKYC, verificações de crédito, APIs de pagamento, etc. Um exemplo de padrão para isso é o CORS - Cross-Origin Resource Sharing.

**Integração horizontal na camada de domínio**: Esse ainda é o padrão de integração horizontal mais comum. Objetos da camada de domínio podem ser criados especificamente para chamar principalmente sistemas externos, preparar a resposta para as camadas de aplicação e UI, e atualizar o estado do negócio no armazenamento persistente na camada de infraestrutura. Objetos de negócios focados em domínio também podem precisar fazer chamadas externas como parte de seu processamento.

**(Infraestrutura) Integração horizontal da camada de persistência**: A integração horizontal de repositórios de dados persistentes na camada de infraestrutura é necessária e inevitável. Por favor, veja este artigo meu para entender as motivações para integrações de dados → Padrões e Progressão do Repositório de Dados Corporativos.

O arquiteto de integração deve considerar os seguintes aspectos para otimizar o design da integração e selecionar os métodos, protocolos e tecnologias apropriados.

- Os dados podem se mover em forma bruta, modificada ou enriquecida entre sistemas
- Pode ser um subconjunto (geralmente) ou todos os dados originais
- Modificações ou transformações podem ser feitas na fonte, no caminho ou no sistema receptor
- Ele pode se mover em tempo real, quase em tempo real ou com atraso (também podemos falar disso como online vs offline; ou tempo real vs lote)
- Pode ser o dado unitário ou agregado (estes últimos por tamanho ou tempo)
- Requisitos de criptografia, compressão e segurança

A imagem abaixo ilustra o ponto de vista horizontal.

![1_NLhrGlQLUu8hiyAJmxRbdw](https://github.com/user-attachments/assets/3ec0a018-7e6f-4998-8294-45cc32e937ba)

**Diretrizes**: O arquiteto de integração deve considerar cuidadosamente como tornar a experiência do usuário intuitiva e fluida por meio dos padrões de solução nos pontos de vista #2 e #5, além da gestão de capacidade e desempenho.

**Ponto de Vista 5: Padrões de integração sem estado para aplicações web e digitais**: No mundo da web e dos serviços digitais, ser 'sem estado' é apresentado como uma solução mágica para componentes não persistirem dados ou não se importarem com o passado e o futuro, e magicamente alcançarem alto desempenho, escalabilidade e desenvolvimento ágil. Mas nenhum sistema ou tarefa empresarial útil pode ser sem estado. Seria informe ou preso no tempo e não teria muita utilidade. (Para mais informações, veja este excelente artigo.)

Mas a ideia por trás do equívoco de 'apatridia' é útil quando a desambiguamos. Ela permite que arquiteturas entreguem rapidamente serviços digitais de negócios ao montar serviços web. E aproveita a distribuição cada vez mais igualitária do poder de processamento entre servidores e dispositivos do usuário.

Um modelo proeminente para arquiteturas sem estado é o REST — Transferência de Estado Representacional. Funciona bem com o modelo de arquitetura em camadas do DDD. (Por favor, veja o livro de Vernon 'Implementing DDD' para mais informações sobre isso.)

Vamos analisar a justificativa por trás da apatridia em termos das três decisões arquitetônicas típicas (veja →As 3 Decisões Arquitetônicas Mais Importantes)

1. **Decisão sobre a Arquitetura de Colocação de Funções**:
**Problema**: Para o mundo digital, web e móvel, como podemos construir serviços backend e parceiros como enxames de unidades de servidores idênticas que crescem suavemente (de algumas para pontuações) com o número de clientes (milhares a centenas de milhões)?
**Pensamento Arquitetônico**: Se os sistemas de serviço mantêm o estado em tempo real do usuário e da tarefa, a interface deve permanecer no mesmo backend até que a tarefa seja concluída. Isso desperdiça recursos em todo o ecossistema do ecospero, limitando o número de clientes que podem ser atendidos e escalando rapidamente com o número de clientes ativos.

E se transferirmos essa responsabilidade em tempo real sobre o conhecimento do usuário e do estado da tarefa (por exemplo, logado, check-out, etc.) para as camadas de UI e Aplicação (terminologia DDD)? Assim, podemos aliviar a camada de domínio nos sistemas primários e parceiros da necessidade de um estado. Deixe que eles gerenciem apenas o estado de negócio não em tempo real e offline (por exemplo, papel do usuário, status do inventário, etc.) e persistam na camada de infraestrutura.

Quando diferenciamos o estado do usuário/tarefa do estado de negócio e sua natureza em tempo real versus não em tempo real dessa forma, toda a vantagem da apatridia se encaixa.

**Decisão**: Faça da instância cliente da interface o componente fixo ou 'fixo' do ecossistema para manter o contexto da sessão e do estado. Aliviar os componentes do servidor e as aplicações/serviços do ecossistema de suporte da necessidade de persistir ou ficarem pegajosos por meio de conhecer ou ter um estado em tempo real.

2. **Decisão sobre a Arquitetura do Repositório de Informação**: Existem três tipos de informação envolvidos.

1. **Informações de estado em tempo real** — Estado do usuário e da tarefa que muda rapidamente conforme o caso de uso avança, por exemplo, logado, finalizado no pagamento, desconectado, etc. Essa é uma informação temporária e transitória. Mantenha na camada de aplicação cliente (termo DDD) perto da memória.
2. **Informações de contexto em tempo real** — Informações ambientais e de usuário que mudam menos rapidamente conforme o caso de uso, por exemplo, tipo de dispositivo, sistema operacional, geolocalização, usuário anônimo ou identificado, companhia aérea selecionada, etc. Mantenha isso na camada de aplicação cliente (termo DDD) em lojas locais semi-permanentes como cookies, etc.
3. **Informações não em tempo real e de longo prazo do Estado dos Negócios** — Informações empresariais que precisam ser mantidas por minutos a anos, por exemplo, usuários, contas, perfis, pedidos, estoque, pagamentos, histórico de serviço, mídia, etc. Mantenha em caches do lado do servidor, RDBMS, arquivos, Hadoop e outros repositórios de armazenamento apropriados.
Portanto, vemos que a necessidade de informação e seu armazenamento permanece em arquiteturas focadas sem estado. Clientes e sistemas de cache gravam dados temporários na memória ou em armazenamento local em disco.

E a maioria dos serviços backend e parceiros armazena dados de longo prazo em bancos de dados centrais. Esses bancos de dados centrais ainda podem ser um ponto de disponibilidade e problemas de desempenho. No entanto, o compromisso é aceitável pela sua relação custo-benefício, já que os dados de longo prazo são volumosos e não podem ser facilmente replicados como os componentes de lógica de negócios da camada de domínio.

3. **Método de integração Decisão de arquitetura**

**Problema**: (1) Como os clientes com estado devem interagir com backends sem estado e sistemas parceiros? (2) Como os sistemas backend sem estado devem interagir com outros sistemas sem estado?

**Interação com estado**: Essas interações ocorrem entre a camada de aplicação cliente e os componentes sem estado do backend. Informações indicadoras de estado exigidas pelo backend da camada de domínio sem estado ou componentes parceiros são incluídas na chamada de API com estado pelo cliente. Por exemplo, na chamada abaixo solicitando um token de autorização, um token de autenticação válido é necessário e incluído na forma do valor `client_id`.

```url
https://MyDomainName.my.salesforce.com/services/oauth2/authorize?response_type=token&client_id=3MVG9lKcPoNINVBKV6EgVJiF.snSDwh6_2wSS7BrOhHGEJkC_&redirect_uri=http%3A%2F%2F2www.example.org%2Fqa%2Fsecurity%2Foauth%2Fuseragent_flow_callback.jsp&scope=api%20id%20web
```

**Interação sem estado**: Na camada de domínio DDD, os componentes interagem sem estado com componentes de outros domínios e sistemas externos. Com base em solicitações da camada de aplicação cliente, as informações são adquiridas pelos componentes do cliente a partir de componentes do servidor na forma de recursos HyperMedia que compreendem informações e hiperlinks para escolhas de ações adicionais. As informações e escolhas são então retornadas ao cliente (aplicações DDD e camadas de UI) para apresentação e próximos passos.

Aqui está um exemplo de uma requisição e uma resposta RESTful sem estado com informações e opções válidas de URI para ação de próximo estado. Ela mostra a essência das informações de 'representação' e 'transferência de estado' que se tornam as escolhas de informação e ações da interface ao longo da camada de aplicação. Este é o projeto Hypermedia as the Engine of Application State (HATEOAS) do padrão da arquitetura REST.

```http
GET /accounts/12345 HTTP/1.1
Host: bank.example.com
```

```http
HTTP/1.1 200 OK

{
    "account": {
        "account_number": 12345,
        "balance": {
            "currency": "usd",
            "value": 100.00
        },
        "links": {
            "deposits": "/accounts/12345/deposits",
            "withdrawals": "/accounts/12345/withdrawals",
            "transfers": "/accounts/12345/transfers",
            "close-requests": "/accounts/12345/close-requests"
        }
    }
}
```

Veja esta imagem para uma ilustração dessa arquitetura geral típica de integração web.

![1_ymzSEsfc5PXuaIOvSljiTg](https://github.com/user-attachments/assets/7209d6df-4f35-4962-aaa1-58eacf107bf4)

**EDA - Orientado por Eventos**: O aspecto de integração da arquitetura é essencialmente uma variação do padrão de integração public-subscribe que suporta o uso assíncrono do modelo REST, essencial na maioria das grandes soluções digitais. Os principais aspectos do EDA são: diferenciar eventos de notificações e tópicos, enviar em vez de sondar/puxar mudanças, catalogar eventos, classificar interações sincronizadas/assíncronas, refatorar aplicativos para publicar/assinar, linguagem Ubiquitous Orientada por Domínio para semântica de tópicos, brokers de eventos, malhas de eventos e preferência por coreografia em vez de orquestração. A ilustração abaixo mostra o conceito em um nível geral.

![1_DxXRWDHEAFpL2ibS7cWWRg](https://github.com/user-attachments/assets/08f7336e-6b21-49b8-9cda-14d8005b0810)

**Diretrizes**: A arquitetura de aplicações digitais/web e da informação mais adequada deve ser decidida para os componentes e repositórios de dados com estado e sem estado. Depois, as decisões sobre a arquitetura de integração virão naturalmente. Interações RESTful seriam a norma, usando cargas úteis JSON, XML e HTML.

**Arquitetura do Sistema DDD REST — uma visão geral**: A combinação das arquiteturas DDD e REST resulta no interessante modelo prático de aplicação e arquitetura de integração ilustrado abaixo. Estude-a com atenção e considere a web digital, arquitetura móvel e frameworks de desenvolvimento de software existentes.

![1_8IYc-rMI40qYL6BEy_93xQ](https://github.com/user-attachments/assets/09292308-0e26-4551-a122-de44516dcc90)

**Ponto de Vista 6: Padrões de Segurança de Integração**: De modo geral, há três áreas que uma empresa precisa garantir:

- Informações empresariais nas lojas
- Informações do usuário nas lojas
- Qualquer tipo de informação em voo

A terceira é de particular preocupação para o arquiteto da integração. Quando pessoas ou sistemas se comunicam, precisamos assegurar cinco coisas a eles:

1. Eles não podem ser ouvidos ou espionados (privacidade, fornecida por redes privadas e criptografia)
2. Eles estão conversando com uma pessoa ou sistema que conhecem (autenticação, fornecida por 1/2/3 fatores)
3. A pessoa ou sistema tem direito à informação ou ação solicitada (autorização, fornecida pelos papéis)
4. Se algo der errado, isso pode ser investigado (não repudiação e outros detalhes fornecidos pela contabilidade)
5. Ataques são prevenidos ou resistidos durante a comunicação (proteção contra vários tipos de ameaças)

Os mecanismos de integração devem atender às necessidades de segurança acima, que podemos abreviar como PAAAP.

Essas necessidades aparecem nos canais de interação humano-sistema e sistema para sistema, conforme abaixo.

1. **De humano para máquina** — teclado, mouse, caneta stylus, toque, fala e biometria.
2. **Máquina a máquina** — As sete camadas de rede OSI, de cima a baixo: Aplicação, Apresentação, Sessão, Transporte, Rede, Enlace de Dados e Física.

Sendo um ensaio de arquitetura, não discutiremos os mecanismos e tecnologias do PAAAP. O leitor interessado encontrará facilmente a informação em outro lugar. A tabela abaixo resume os padrões típicos de soluções de segurança para entregar PAAAP em cada camada.

(Por favor, note que as camadas OSI e as soluções de segurança não são arquitetônicas nem imutáveis. Use a tabela apenas para pensamento de aspectos e princípios.)

![1_V9i3Chyj_75savQGGh4tzA](https://github.com/user-attachments/assets/ddc32509-eab0-4a73-8e81-1b200884366f)

**Diretrizes**: Considere os padrões de segurança da organização, os frameworks de segurança da indústria como o SABSA, as arquiteturas de referência de segurança (por exemplo, AWS, Cisco) e a necessidade particular de cada interface no escopo da solução para decidir a arquitetura, o design e a tecnologia de segurança.

> [!Note]
> Esses padrões e pontos de vista da arquitetura de integração resistirão ao teste do tempo. Gosto de estudar e descrever ideias estáveis pelo seu valor prático. Veja as formas fundamentais pelas quais as coisas interagem; Tudo flui a partir daí. Vá em frente e arquitete, arquiteto.

O termo 'micro' em Microserviços, embora indicativo do tamanho de um serviço, não é o único critério que torna uma aplicação um Microserviço. Quando as equipes migram para uma arquitetura baseada em microserviços, elas buscam aumentar sua agilidade — implantando recursos de forma autônoma e frequente. É difícil definir uma única definição concisa desse estilo arquitetônico. Gostei dessa breve definição:

> "arquitetura orientada a serviços composta por elementos frouxamente acoplados que possuem contextos limitados." — Adrian Cockcroft

Embora isso defina uma heurística de design de alto nível, a arquitetura de microserviços possui algumas características únicas que a diferenciam da arquitetura orientada a serviços de antigamente. Algumas dessas características, abaixo. Esses e alguns outros são bem documentados — <a href="https://martinfowler.com/articles/microservices.html">o artigo de Martin Fowler</a> e Building Microservices, de Sam Newman, para citar alguns.

## [Microservices] Hexagonal architecture (Ports & Adapters)
<img src="https://img.shields.io/badge/Spring_Boot-3.10.7-limegreen?style=flat&logo=Spring&logoColor=white"> <img src="https://img.shields.io/badge/Kotlin-16-indigo?style=flat&logo=Kotlin&logoColor=white">  <img src="https://img.shields.io/badge/.NET-10-indigo?style=flat&logo=.NET&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-339933?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/RabbitMQ-16-orange?style=flat&logo=RabbitMQ&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-16.17-blue?style=flat&logo=PostgreSQL&logoColor=white"> <img src="https://img.shields.io/badge/MongoDB-16-lime?style=flat&logo=MongoDB&logoColor=white">

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/7c9bb501-d7cd-4b94-88c1-ae67cd8e07f8" align="right" height="77">

A **arquitetura hexagonal** é um design de software, também conhecida como Arquitetura de **Portas e Adaptadores (Ports and Adapters)**, na qual é uma abordagem de design que promove a separação de preocupações e a independência da lógica central da aplicação em relação aos detalhes técnicos e de infraestrutura. A Arquitetura Hexagonal, também conhecida como Arquitetura de Portas e Adaptadores, é uma abordagem de design de sistema destinada a desacoplar a lógica de negócios principal de um software de suas interações externas. 

A imagem representa visualmente essa arquitetura, colocando as **entidades principais** (lógica de negócios) no centro do sistema, protegidas de dependências externas, como bancos de dados, APIs e filas de mensagens. O **núcleo** se comunica com o mundo exterior por meio de **portas** (interfaces), que atuam como limites que definem o que o sistema central espera em relação à entrada e saída.

A arquitetura Hexagonal, também conhecida como Arquitetura de Portas e Adaptadores, foca em isolar a lógica central da aplicação (domínio) de detalhes de implementação externos, propõe separar o núcleo (core) da aplicação (domínio) das interfaces externas (como UI, banco de dados, APIs) através de portas (interfaces) e adaptadores (implementações). 

Ao redor do núcleo estão adaptadores que interagem com componentes externos. Esses adaptadores implementam a funcionalidade exigida pelas portas. Por exemplo, solicitações HTTP ou interações com um banco de dados são tratadas por adaptadores específicos, que convertem os dados em um formato que as entidades principais podem processar. Isso fica evidente na imagem, onde diferentes sistemas externos, como HTTP, SQS (fila de mensagens), DB (banco de dados), API REST e API GRPC, são conectados por meio de camadas que processam solicitações e respostas.

A arquitetura hexagonal foi inventada por Alistair Cockburn em 2005, em uma tentativa de evitar armadilhas estruturais conhecidas no design de software orientado a objetos (OOP), como dependências indesejadas entre camadas e a contaminação do código da interface do usuário com a lógica de negócios. O conceito de Arquitetura Hexagonal foi proposto por Alistair Cockburn, em meados dos anos 90, em um artigo postado na primeira wiki que foi desenvolvida, chamada WikiWikiWeb (cujos artigos tratavam principalmente de temas relacionados com Engenharia de Software).

Os objetivos de uma Arquitetura Hexagonal são parecidos com os de uma Arquitetura Limpa. Mas, para reforçar, a ideia é construir sistemas que favorecem reusabilidade de código, alta coesão, baixo acoplamento, independência de tecnologia e que são mais fáceis de serem testados. A arquitetura hexagonal, também conhecida como arquitetura de portas e adaptadores, pode ser combinada com outras arquiteturas e designs de software para criar sistemas mais robustos e flexíveis como a Arquitetura em Camadas (N-Tier/ Layered Architecture), SOA - Arquitetura Orientada a Serviços, Microservices, DDD - Domain-Driven Design, Arquitetura Limpa e CQRS - Command Query Responsibility Segregation.

Uma <a href="https://medium.com/codex/clean-architecture-for-dummies-df6561d42c94">Arquitetura Hexagonal</a> divide as classes de um sistema em dois grupos principais:

<img src="https://github.com/user-attachments/assets/a83de780-4af3-4860-9433-381fce97116e" align="right" height="377">

- **Classes de domínio**, isto é, diretamente relacionadas com o negócio do sistema.

- **Classes relacionadas com infraestrutura**, tecnologias e responsáveis pela integração com sistemas externos (tais como bancos de dados).

Além disso, em uma Arquitetura Hexagonal, classes de domínio não devem depender de classes relacionadas com infraestrutura, tecnologias ou sistemas externos. A vantagem dessa divisão é desacoplar esses dois tipos de classes.

Assim, as classes de domínio não conhecem as tecnologias – bancos de dados, interfaces com usuário e quaisquer outras bibliotecas – usadas pelo sistema. Consequentemente, mudanças de tecnologia podem ser feitas sem impactar as classes de domínio. Talvez ainda mais importante, as classes de domínio podem ser compartilhadas por mais de uma tecnologia. Por exemplo, um sistema pode ter diversas interfaces (Web, mobile, etc).

Em uma arquitetura hexagonal, a comunicação entre as classes dos dois grupos é mediada por adaptadores, isto é, por classes que implementam o padrão de projeto de mesmo nome que estudamos no Capítulo 6. Iremos explicar melhor o papel dos adaptadores logo a seguir.

Visualmente, a arquitetura é representada por meio de dois hexágonos concêntricos (veja figura). No hexágono interno, ficam as classes do domínio (ou classes de negócio, se você preferir). No hexágono externo, ficam os adaptadores. Por fim, as classes de interface com o usuário, classes de tecnologia ou de sistemas externos ficam fora desses dois hexágonos.

Assim, o nome hexagonal tem sua origem na figura acima. Cockburn justifica o uso de um hexágono do seguinte modo:

> **"** Cada face do hexágono representa um motivo pelo qual o sistema deve se comunicar com o mundo exterior. É por isso que são hexágonos concêntricos e não círculos concêntricos.

Dentre os motivos que requerem comunicação com o mundo exterior podemos citar os seguintes: interagir com seus usuários (por meio de algum tipo de interface, seja ela gráfica, Web, mobile, terminal, etc), persistir informações, enviar informações para outros sistemas, etc.

Em uma Arquitetura Hexagonal, o termo **porta** (port) designa as interfaces usadas para comunicação com as classes de domínio (veja que interface aqui significa interface de programação; por exemplo, uma interface de Java).

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/34885cef-b23b-4b69-8bf1-307006294132" align="right" height="377">

Existem dois tipos de portas:

- **Portas de entrada**: são interfaces usadas para comunicação de fora para dentro, isto é, quando uma classe externa precisa chamar um método de uma classe de domínio. Logo, essas portas declaram os serviços providos pelo sistema, isto é, serviços que o sistema oferece para o mundo exterior.

- **Portas de saída**: são interfaces usadas para comunicação de dentro para fora, isto é, quando uma classe de domínio precisa chamar um método de uma classe externa. Logo, essas portas declaram os serviços requeridos pelo sistema, isto é, serviços do mundo exterior que são necessários para o funcionamento do sistema.

O importante é que as portas são independentes de tecnologia. Portanto, elas estão localizadas no hexágono interior.

Por outro lado, os sistemas externos, normalmente, usam alguma tecnologia, seja ela de comunicação (REST, gRPC, GraphQL, etc), de bancos de dados (SQL, noSQL, etc), de interação com o usuário (Web, mobile, etc), etc.

Daí a necessidade de componentes localizados no hexágono mais externo da arquitetura – os adaptadores –, os quais atuam de um dos dois modos a seguir:

Eles recebem chamadas de métodos vindas de fora do sistema e encaminham essas chamadas para métodos adequados das portas de entrada.

<img src="https://github.com/user-attachments/assets/b73cb80b-0150-468e-850f-8bd59658e9cb" align="right" height="377">

Eles recebem chamadas vindas de dentro do sistema, isto é, das classes de domínio, e as direcionam para um sistema externo, tais como um banco de dados, um outro sistema da organização ou mesmo de terceiros.

A arquitetura hexagonal desempenha um papel significativo no projeto do sistema por vários motivos, particularmente no contexto de capacidade de manutenção, escalabilidade e flexibilidade. Aqui estão as principais razões pelas quais é importante:

- **Separação de preocupações**: a arquitetura impõe uma separação clara entre a lógica de negócios principal e os sistemas externos, como bancos de dados, APIs ou interfaces de usuário. Ao isolar o núcleo, ele garante que a lógica de negócios não esteja entrelaçada com a infraestrutura ou preocupações externas. Isso leva a um código mais limpo e modular, mais fácil de entender e manter.

- **Adaptabilidade e flexibilidade**: Um dos principais benefícios da arquitetura hexagonal é sua capacidade de se adaptar a mudanças em sistemas externos sem exigir mudanças na lógica de negócios principal. Por exemplo, se uma empresa decidir mudar de um banco de dados relacional para um banco de dados NoSQL, apenas o adaptador responsável pela interação do banco de dados precisa ser modificado. A lógica central permanece inalterada. Isso torna o sistema à prova de futuro e capaz de evoluir com as mudanças tecnológicas.

- **Estabilidade aprimorada**: como dependências externas, como bancos de dados ou APIs, são abstraídas, a lógica principal pode ser facilmente testada por unidade sem a necessidade de simulações ou stubs complexos. O uso de portas e adaptadores permite simular interfaces para sistemas externos, permitindo que o núcleo seja testado isoladamente. Isso leva a uma maior cobertura de teste e a um código mais confiável e livre de bugs.

- **Desenvolvimento desacoplado**: Diferentes equipes podem trabalhar de forma independente em várias partes do sistema. Uma equipe pode trabalhar na lógica de negócios principal, enquanto outra se concentra no desenvolvimento de adaptadores para APIs, bancos de dados ou outros sistemas externos. Essa natureza dissociada permite o desenvolvimento paralelo, acelerando o processo de desenvolvimento.

- **Componentes intercambiáveis**: A arquitetura hexagonal facilita a substituição ou integração de novos componentes sem afetar o sistema principal. Se uma nova API for introduzida ou se uma mais antiga for descontinuada, o adaptador que manipula essa API pode ser trocado sem perturbar a lógica de negócios central. Isso é especialmente útil em sistemas grandes e distribuídos, onde diferentes componentes estão em constante evolução.

A arquitetura hexagonal, também conhecida como arquitetura de portas e adaptadores, consiste em vários componentes-chave que trabalham juntos para criar um sistema flexível, desacoplado e sustentável. Aqui estão os principais componentes da Arquitetura Hexagonal:

<table>
	<tr>
		<td><img src="https://github.com/user-attachments/assets/945d2d87-6b9f-4700-81e2-cd95451070f5" height="477"></td>
		<td><img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/8dd1424b-090d-4ce5-9227-a704d680f5e4" height="477"></td>
	</tr>
</table>

1. **Entidades** (Core Business Logic): No coração da Arquitetura Hexagonal estão as Entidades, que representam a lógica de negócios principal e as regras do aplicativo. Essas entidades são completamente independentes de sistemas externos e permanecem isoladas de preocupações como bancos de dados ou interfaces de usuário. O objetivo é garantir que a lógica de negócios seja encapsulada e possa operar independentemente de como os dados são recebidos ou persistidos.

2. **Portas** (interfaces): As portas são as interfaces que definem como os sistemas externos se comunicam com a lógica principal. Essas portas atuam como limites entre o núcleo e o mundo exterior. Existem dois tipos de portas:
   - **Portas de entrada**: Defina como o mundo externo (como uma interface com o usuário, API ou fila de mensagens) pode interagir com o sistema principal. Eles são responsáveis por receber informações e acionar a lógica de negócios no núcleo.
   - **Portas de saída**: Defina como o sistema central interage com sistemas externos (como bancos de dados ou APIs externas) para enviar ou receber dados. Essas portas abstraem os detalhes de comunicação e garantem que o núcleo interaja apenas com componentes externos por meio dessas interfaces.

3. **Adaptadores** (Implementações de Portas): Adaptadores são a implementação das portas. Eles são responsáveis por traduzir dados externos (como solicitações HTTP, consultas de banco de dados ou mensagens de filas) em algo que o núcleo possa entender e vice-versa. Os adaptadores permitem que diferentes sistemas externos interajam com o sistema central sem que o núcleo esteja diretamente ciente das especificidades do sistema externo.
   - **Adaptadores de entrada**: Manipule a comunicação de fontes externas, como controladores HTTP, componentes de interface do usuário ou sistemas de mensagens, e converta-os em um formato compreendido pelo núcleo por meio de portas de entrada.
   - **Adaptadores de saída**: lidam com a comunicação com serviços externos ou bancos de dados, como implementações de repositório, APIs externas ou sistemas de armazenamento de dados. Eles pegam os dados do núcleo, processam-nos conforme necessário e os enviam para os sistemas externos apropriados.

4. **Serviços de Aplicação** (Interagentes/Casos de Uso) Os Serviços de Aplicativos, também conhecidos como Interagentes ou Casos de Uso, atuam como intermediários entre as entidades (lógica de negócios principal) e as camadas externas (portas e adaptadores). Esses serviços coordenam o fluxo de dados entre portas de entrada (por exemplo, solicitações de usuários) e portas de saída (por exemplo, fontes de dados). Eles contêm a lógica do aplicativo que orienta o processo de negócios, mas permanecem separados das principais regras de negócios.

Por exemplo, um Interactor pode obter a entrada do usuário de um formulário da Web (por meio de um adaptador de entrada), processá-la por meio de regras de negócios e, em seguida, persistir os resultados usando um repositório (por meio de um adaptador de saída).

![0_qLwWGERvZjcqs0ii](https://github.com/user-attachments/assets/3372d7a2-4d5e-4f72-b0c9-aa3374bfb780)

5. **Repositórios** (camada de persistência): Os repositórios são usados para gerenciar a persistência de dados. Eles fornecem uma camada entre a lógica principal e o sistema de armazenamento de dados (como um banco de dados). Os repositórios geralmente são implementados como adaptadores de saída que interagem com o banco de dados por meio de portas de saída. Eles encapsulam a lógica necessária para recuperar e armazenar dados em sistemas de armazenamento externos, permitindo que a lógica principal permaneça independente do banco de dados.

6. **Camada de transporte**: A camada de transporte lida com a comunicação entre usuários ou sistemas externos e o aplicativo. Isso pode incluir o tratamento de solicitações HTTP, filas de mensagens ou outras formas de operações de entrada/saída. A camada de transporte interage com os adaptadores de entrada para encaminhar solicitações ao sistema principal. Na Arquitetura Hexagonal, essa camada é desacoplada da lógica de negócios, permitindo que o sistema suporte vários mecanismos de comunicação (por exemplo, API REST, WebSocket, etc.).

7. **Sistemas Externos** (Infraestrutura): Os sistemas externos incluem bancos de dados, APIs, filas de mensagens e outros componentes de infraestrutura com os quais o aplicativo interage. Na arquitetura hexagonal, esses sistemas são conectados à lógica principal por meio de adaptadores e portas de saída, garantindo que o sistema central não tenha conhecimento dos detalhes do sistema externo.

A arquitetura hexagonal (arquitetura de portas e adaptadores) oferece várias vantagens no design do sistema, tornando-a uma escolha popular para a criação de sistemas flexíveis, sustentáveis e escaláveis. Aqui estão as principais vantagens:

- Separação de preocupações: A arquitetura hexagonal separa claramente a lógica de negócios principal de sistemas externos, como bancos de dados, APIs ou interfaces de usuário. Isso torna a lógica principal independente de como os dados são inseridos, armazenados ou exibidos, permitindo um código modular mais limpo.

- Flexibilidade e adaptabilidade: Ao desacoplar a lógica de negócios principal dos sistemas externos, a arquitetura permite flexibilidade na integração de novas tecnologias ou na substituição das antigas. Por exemplo, você pode alternar de um banco de dados SQL para um banco de dados NoSQL ou de uma API REST para uma API GraphQL, simplesmente alterando o adaptador correspondente, sem tocar na lógica principal.

- Estabilidade aprimorada: Como a lógica principal é isolada de sistemas externos, ela pode ser facilmente testada por unidade sem a necessidade de simular ou eliminar dependências complicadas, como bancos de dados ou serviços da Web. Os testes se tornam mais diretos e focados na funcionalidade principal, levando a uma melhor cobertura e sistemas mais confiáveis.

- Manutenção: A arquitetura hexagonal incentiva a modularidade, tornando o código mais fácil de entender e manter. Cada componente, seja a lógica principal, adaptadores ou portas, tem uma função bem definida e pode ser mantido separadamente. Isso reduz a chance de introduzir bugs ao modificar uma parte do sistema, pois as alterações são localizadas.

- Extensibilidade: novos recursos ou componentes podem ser adicionados ao sistema sem alterar a lógica principal existente. Por exemplo, se você precisar adicionar um novo tipo de interface (por exemplo, um novo sistema de mensagens ou API), basta criar um novo adaptador e porta para ele, deixando a lógica principal inalterada. Isso torna a arquitetura altamente extensível.

- Desenvolvimento paralelo: Diferentes equipes podem trabalhar em diferentes partes do sistema de forma independente. Uma equipe pode se concentrar no desenvolvimento da lógica de negócios principal, enquanto outras equipes trabalham em adaptadores específicos para
sistemas externos, como bancos de dados, APIs ou filas de mensagens. Esse desacoplamento permite um desenvolvimento mais rápido e maior colaboração.

Embora a arquitetura hexagonal ofereça inúmeros benefícios, ela também apresenta certos desafios no design do sistema. Esses desafios precisam ser considerados cuidadosamente ao implementar essa arquitetura:

1. Maior complexidade no início: a arquitetura hexagonal introduz camadas adicionais, como portas, adaptadores e serviços de aplicativos, o que pode tornar o projeto inicial mais complexo. Os desenvolvedores podem precisar escrever mais código clichê para criar interfaces (portas) e adaptadores, fazendo com que o sistema pareça mais complexo do que arquiteturas mais simples, especialmente para aplicativos pequenos ou diretos.

2. Curva de aprendizado: Para equipes não familiarizadas com a arquitetura, pode haver uma curva de aprendizado íngreme. Entender como estruturar o sistema usando portas, adaptadores e a separação de preocupações pode levar tempo, e os desenvolvedores precisam se familiarizar com novos padrões e princípios de design. Isso pode retardar o processo de desenvolvimento inicialmente.

3. Sobrecarga para aplicativos simples: Para aplicativos pequenos e simples, a arquitetura hexagonal pode introduzir complexidade desnecessária. Os benefícios do desacoplamento, da capacidade de teste e da modularidade podem não valer a sobrecarga adicional de projetar o sistema de maneira hexagonal. Aplicativos mais simples podem ser melhor atendidos com arquiteturas menos complexas, como MVC ou arquitetura em camadas.

4. Dificuldade em gerenciar vários adaptadores: À medida que o sistema cresce, pode ser necessário oferecer suporte a várias interfaces externas, como diferentes APIs, bancos de dados ou interfaces de usuário. O gerenciamento desses adaptadores pode se tornar complicado, pois cada um requer sua própria implementação. Manter o controle de vários adaptadores e mantê-los pode aumentar a complexidade do sistema.

5. Mais abstrações para gerenciar: A arquitetura hexagonal envolve várias camadas de abstração - portas, adaptadores, entidades, interagentes - cada uma responsável por diferentes aspectos do sistema. Embora essas abstrações sejam essenciais para o desacoplamento, às vezes elas podem dificultar os problemas de depuração e rastreamento, pois você precisa navegar por várias camadas para entender o fluxo de dados e a lógica.

A implementação da arquitetura hexagonal requer uma estratégia cuidadosa para garantir que o sistema mantenha seus benefícios de flexibilidade, desacoplamento e capacidade de manutenção. Aqui estão as principais estratégias para implementar com sucesso a arquitetura hexagonal no projeto do sistema:

1. Comece com a Lógica de Domínio Principal (Entidades): Defina a lógica de negócios principal: comece implementando a lógica de negócios principal (entidades). A parte central da Arquitetura Hexagonal é o modelo de domínio, que deve permanecer independente de sistemas externos, como bancos de dados, APIs ou interfaces de usuário. Isso garante que as regras de negócios estejam no centro do sistema e não sejam afetadas por alterações na infraestrutura.

2. Foco no DDD (Design Controlado por Domínio): o uso dos princípios do DDD ajuda a moldar um modelo de domínio avançado que reflete os requisitos de negócios. Isso garante que a lógica principal seja autossuficiente e possa ser reutilizada em diferentes contextos.

3. Projete as portas (interfaces): Identifique as portas de entrada e saída: Depois que a lógica principal for estabelecida, defina as portas de entrada (como o mundo externo interage com o sistema) e as portas de saída (como o sistema interage com sistemas externos, como bancos de dados ou serviços externos).

4. Dependências externas abstratas: as portas devem definir interfaces que abstraem os detalhes de dependências externas, como bancos de dados, APIs ou filas de mensagens. Isso ajuda a manter a lógica principal isolada de quaisquer detalhes específicos da infraestrutura.

5. Adaptadores de implemento (conectando sistemas externos): Desenvolver adaptadores para portas de entrada: Implemente adaptadores de entrada que convertem entradas externas (como solicitações HTTP, comandos CLI ou eventos de filas de mensagens) no formato exigido pela lógica principal. Por exemplo, use um controlador HTTP como um adaptador de entrada para lidar com solicitações REST e roteá-las para o sistema núcleo.

6. Desenvolver adaptadores para portas de saída: Implemente adaptadores de saída que se conectam a sistemas externos (como um banco de dados ou APIs externas). Esses adaptadores lidam com a comunicação com esses sistemas externos, mas permanecem abstraídos da lógica de negócios principal.

7. Isolar infraestrutura: mantenha a lógica de infraestrutura (por exemplo, interações de banco de dados ou clientes de API) contida nos adaptadores de saída, garantindo que a lógica principal não esteja ciente das especificidades do sistema externo.

8. Aproveite a injeção de dependência: Desacoplar núcleo dos adaptadores: use a injeção de dependência para injetar os adaptadores na lógica principal. Isso garante que o sistema principal dependa apenas de abstrações (portas) e não de implementações concretas (adaptadores).

9. Injetar adaptadores por meio de construtores ou fábricas: implemente a injeção de adaptador usando construtores ou fábricas, garantindo que a lógica principal permaneça testável e adaptável. Esse padrão dá suporte à troca de adaptadores diferentes com impacto mínimo na lógica principal.

10. Serviços de aplicativos de design (interactianos): Coordenar casos de uso: use serviços de aplicativos ou interagentes para implementar os principais casos de uso do aplicativo. Esses serviços atuam como intermediários entre as portas de entrada (solicitações do usuário) e as portas de saída (fontes de dados ou APIs externas). Mantenha a lógica de negócios central: certifique-se de que os interagentes não contenham a lógica de negócios por conta própria, mas coordenem as interações entre as principais regras de negócios e o mundo exterior.

11. Encapsular o acesso a dados em repositórios: Lógica de persistência abstrata: Implemente repositórios como adaptadores de saída que gerenciam interações de banco de dados. Os repositórios encapsulam a lógica de acesso a dados, permitindo que a lógica principal permaneça independente das especificidades do banco de dados.

12. Use repositórios orientados por interface: defina repositórios como interfaces na camada central e implemente a lógica real de acesso a dados na camada de infraestrutura (usando ORMs, consultas SQL etc.).

Casos de uso da arquitetura hexagonal: A arquitetura hexagonal é particularmente benéfica em uma variedade de casos de uso de projeto de sistema em que flexibilidade, desacoplamento e capacidade de manutenção são cruciais.

Abaixo estão alguns dos principais casos de uso em que a Arquitetura Hexagonal pode ser aplicada:

- Construindo aplicativos da Web flexíveis: No desenvolvimento de aplicativos da Web, a arquitetura hexagonal permite separar a lógica de negócios das preocupações de infraestrutura, como estruturas da Web ou bancos de dados. Isso torna o aplicativo mais flexível para se adaptar a alterações, como troca de estruturas, integração com novas tecnologias de front-end ou alteração de mecanismos de armazenamento de dados.

- Arquitetura de microsserviços: em microsserviços, diferentes serviços geralmente interagem entre si, bancos de dados ou APIs de terceiros. A Hexagonal Architecture garante que os microsserviços sejam isolados, com o núcleo de cada serviço sendo completamente desacoplado de suas dependências. Isso também permite que os serviços sejam facilmente substituídos ou dimensionados sem afetar a lógica de negócios principal.

- Sistemas orientados a eventos: os sistemas orientados a eventos dependem muito da comunicação assíncrona por meio de filas de mensagens (como RabbitMQ ou AWS SQS). O HexagonalArchitecture permite que a lógica de negócios principal permaneça independente de se os eventos vêm de HTTP, WebSocket ou filas de mensagens, pois cada tipo de interação pode ser tratado por diferentes adaptadores de entrada.

- Sistemas com várias interfaces de usuário: quando um aplicativo precisa oferecer suporte a várias interfaces de usuário (por exemplo, web, móvel, desktop, CLI), a arquitetura hexagonal permite que a lógica de negócios principal seja compartilhada em todas as plataformas. Adaptadores diferentes podem ser criados para cada tipo de interface do usuário sem duplicar a lógica principal.

- Desenvolvimento orientado a testes (TDD) e testes unitários: a arquitetura hexagonal é particularmente adequada para TDD e testes unitários porque a lógica de negócios principal é isolada das preocupações com a infraestrutura. O modelo de portas e adaptadores permite simular facilmente sistemas externos, tornando os testes de unidade mais simples de escrever e manter.

A arquitetura hexagonal, também conhecida como arquitetura de portas e adaptadores, foi aplicada com sucesso em vários projetos do mundo real em diferentes domínios. Aqui estão alguns exemplos notáveis:

- **Shopify**: A lógica de negócios principal da Shopify é dissociada de vários gateways de pagamento, provedores de remessa e outros serviços por meio de adaptadores. Isso permite que os comerciantes alternem entre diferentes opções de pagamento e integrem vários serviços sem afetar as principais funcionalidades da plataforma.

- **PayPal**: o PayPal usa a Hexagonal Architecture para separar sua lógica principal de processamento de transações dos vários serviços externos com os quais interage, como diferentes APIs bancárias, sistemas de detecção de fraudes e interfaces de usuário. Isso permite que o PayPal se adapte perfeitamente às mudanças nos regulamentos ou integrações.

- **WordPress**: O WordPress implementa a Arquitetura Hexagonal permitindo que os plug-ins interajam com suas principais funcionalidades sem acoplá-las fortemente. Isso permite que os desenvolvedores estendam o CMS com vários plug-ins (para SEO, análises, etc.) que atuam como adaptadores para a lógica principal.

- **Netflix**: A Netflix utiliza a Hexagonal Architecture para gerenciar seus vários microsserviços para entrega de conteúdo, recomendações de usuários e processamento de pagamentos. Cada serviço pode interagir com sistemas externos (como redes de distribuição de conteúdo) por meio de adaptadores, permitindo que eles sejam dimensionados de forma independente.

- **Epic Systems**: A Epic usa a Hexagonal Architecture para desacoplar seu sistema de gerenciamento clínico de vários sistemas externos (como laboratórios, farmácias e outros prestadores de serviços de saúde). Isso garante que as mudanças nos sistemas externos não interrompam as principais funcionalidades de gerenciamento de integridade.

<table>
	<tr>
		<td><img height="879" alt="Architecture" src="https://github.com/user-attachments/assets/700cc7a0-1977-43fd-9b1a-626cde1ddba7" /></td>
		<td><img height="879" alt="Architecture" src="https://github.com/user-attachments/assets/e78463f5-0a30-4b92-a9a6-6831c5582098" /></td>
		<td><img height="879" alt="Architecture" src="https://github.com/user-attachments/assets/bc7c8b07-3835-489e-9c1f-7489f41d462f" /></td>
		<td><img height="879" alt="Architecture" src="https://github.com/user-attachments/assets/bba31259-d365-49be-b4ea-d4e79c02bdf0" /></td>
	</tr>
</table>

Em conclusão, a Arquitetura Hexagonal é uma abordagem de design poderosa que aumenta a flexibilidade e a capacidade de manutenção dos sistemas de software. Ao separar a lógica de negócios principal das dependências externas, ele permite que os desenvolvedores se adaptem facilmente às mudanças e integrem novas tecnologias sem interromper o aplicativo principal. Essa arquitetura promove melhores práticas de teste e simplifica o processo de desenvolvimento. Seja aplicada a aplicativos da web, microsserviços ou integrações de sistemas legados, a Hexagonal Architecture oferece uma maneira estruturada de criar soluções resilientes e escaláveis que podem evoluir com as necessidades de usuários e empresas.

<img width="1200" height="844" alt="0_nQxQ1mNs8cgAHHK1" src="https://github.com/user-attachments/assets/483b9254-07d8-409d-99e8-042a57a2d0ee" />

## [Microservices] Tomato architecture
<img src="https://img.shields.io/badge/Jira-Pomodoro-tomato?style=flat&logo=Jira&logoColor=white"> <img src="https://img.shields.io/badge/ClickUp-Pomodoro-tomato?style=flat&logo=ClickUp&logoColor=white"> <img src="https://img.shields.io/badge/Trello-Pomodoro-tomato?style=flat&logo=Trello&logoColor=white"> <img src="https://img.shields.io/badge/Asana-Pomodoro-tomato?style=flat&logo=Asana&logoColor=white"> <img src="https://img.shields.io/badge/Redmine-Pomodoro-tomato?style=flat&logo=Redmine&logoColor=white"> <img src="https://img.shields.io/badge/Clockify-Pomodoro-tomato?style=flat&logo=clockify&logoColor=white">

<img src="https://em-content.zobj.net/source/microsoft-teams/363/tomato_1f345.png" height="77" align="right">

A **Tomato Architecture** é uma evolução pragmática das arquiteturas **Clean**, **Onion** e **Hexagonal**, criada para lidar com a realidade de sistemas modernos distribuídos, orientados a eventos, altamente integrados, com múltiplos modelos de escrita/leitura, APIs, filas, streams e domínios que mudam ao longo do tempo. É uma tentativa de pegar o melhor das arquiteturas clássicas e torná-las realmente práticas no dia a dia, evitando o excesso de abstração e o “purismo arquitetural” que muitas vezes torna Clean/Hexagonal difíceis de aplicar em escala. Se Clean/Hexagonal são teorias sobre pureza, Tomato é prática sobre sobrevivência e evolução de sistemas reais.

A Tomato Architecture nasce da percepção de que sistemas reais são “vivos”, orgânicos, mudam de forma, crescem de maneira desigual e possuem partes que amadurecem em ritmos diferentes, exatamente como um tomate crescendo em camadas, com áreas mais verdes e áreas mais vermelhas coexistindo. A ideia central é que o software não precisa nascer 100% Clean, Onion ou Hexagonal. Ele pode amadurecer aos poucos, aplicando princípios de isolamento de domínio somente onde isso realmente traz benefício concreto.

É uma arquitetura baseada em **maturidade por camadas**, e não apenas em separação por dependências. Enquanto Onion e Hexagonal colocam regras fixas para quem depende de quem, a <a href="https://www.sivalabs.in/blog/tomato-architecture-pragmatic-approach-to-software-design/">Tomato</a> introduz o conceito de **maturidade arquitetural**, permitindo que cada módulo esteja em um nível diferente, variando do mais simples ao mais sofisticado conforme sua importância no domínio.

*Como ela evolui Clean, Onion e Hexagonal*: O Clean Architecture define camadas puras e independentes. O Onion reforça o papel do domínio no centro e a separação rígida de infraestrutura. O Hexagonal enfatiza portas e adaptadores, abrindo comportamentos para o mundo externo via interfaces. A <a href="https://tomato-architecture.github.io/">Tomato</a> olha para tudo isso e diz: “Ótimo, mas e na prática?”. Então ela reduz a complexidade desnecessária e cria uma evolução mais realista:

Ela mantém a ideia de **domínio como núcleo**, mas flexibiliza o que está em volta. Ou seja, você não precisa criar dezenas de ports e adapters para operações triviais, e pode aceitar integrações diretas quando o custo de um isolamento extremo não compensa. Ela também permite que partes do sistema funcionem sem domínio formal, algo impossível no Clean tradicional, reconhecendo que em sistemas modernos alguns módulos são apenas orquestração, queries, relatórios ou transformações simples. Além disso, ela mistura CQRS, Event-Driven e Domain Events como mecanismos naturais, não como plugins opcionais — algo que Clean/Onion falam pouco.

O conceito central: **“maturidade arquitetural por tomate”**: Em vez de dividir o sistema rigidamente em camadas concêntricas (como na Onion) ou por portas/plugues (como no Hexagonal), a Tomato o divide em **fatias de maturidade**. Cada parte do sistema pode estar em um nível diferente:

<img height="266" align="right" src="https://github.com/user-attachments/assets/fdac4440-d039-4361-9a5e-27b4659d277e" />

- **Tomate Verde**: Módulos simples, CRUDs, endpoints de infraestrutura, autenticação, configurações, health checks, integração simples. Nada de complexidade desnecessária. Apenas o essencial.

- **Tomate Meio Maduro**: Serviços que começam a ter regras de negócio, leves validações, pequenas entidades, alguns eventos. Começa a se aproximar de DDD, mas sem as camadas rígidas.

- **Tomate Maduro**: Partes realmente críticas do domínio, onde invariantes são fortes, lógica complexa existe, múltiplos agregados interagem, e onde faz sentido aplicar DDD tático completo (Aggregates, Domain Services, Value Objects, Domain Events).

> [!Note]
> Lembra o **Rotten Tomatoes**, e essa associação não é coincidência, porque o próprio nome Tomato Architecture brinca com essa ideia de camadas, maturidade e gradação do mesmo jeito que o Rotten Tomatoes faz ao avaliar filmes. Mas, conceitualmente, a semelhança é ainda mais interessante do que parece à primeira vista. A lógica do Rotten Tomatoes é baseada na mistura de opiniões, contextos diferentes, níveis de qualidade distintos e perspectivas que se combinam para avaliar e criar um resultado final coerente. Isso é exatamente o espírito que a Tomato Architecture incorpora na engenharia de software. Ela parte da premissa de que um sistema grande nunca é inteiramente homogêneo, nunca nasce perfeito e nunca se mantém estático. Ele vai acumulando partes de qualidade diferente, algumas mais maduras, outras mais imaturas, e tudo isso convive ao mesmo tempo dentro da mesma aplicação — assim como os tomates verdes e vermelhos num mesmo cacho.

Isso resolve o maior problema das arquiteturas puristas: a ideia de que “tudo é Clean” ou “tudo é Hexagonal”. No Tomato, apenas o que realmente precisa ser maduro, é maduro.

Por que o nome “Tomato”? A metáfora é proposital. Um tomate tem:

* um **centro forte e uniforme** (o domínio maduro),
* camadas ao redor com texturas e resistências diferentes,
* partes verdes coexistindo com partes vermelhas,
* amadurecimento progressivo,
* e uma forma natural de crescimento, não simétrica.

A arquitetura assume que **sistemas reais são assim**:

![tomato-architecture](https://github.com/user-attachments/assets/a080719a-4aef-4bf9-ab41-f9d647082f8c)

*Como funciona na prática*: A Tomato organiza o sistema em **domínios**, cada um com seu nível de maturidade. Dentro de cada domínio:

* A API expõe comandos e queries.
* Para leitura, usa modelos diretos, rápidos e orientados a performance.
* Para escrita, pode usar agregados, serviços de domínio e eventos.
* Infrastructure não é demonizada — é utilizada de forma prática.
* Barramentos de evento são tratados como parte natural do domínio.

## [Microservices] Throttling
**Throttling** é o conceito utilizado para controlar a quantidade de solicitações ou operações que podem ser realizadas em um determinado período de tempo. O termo é comumente aplicado em contextos de redes, APIs, sistemas de computação e infraestrutura, com o objetivo de limitar o consumo excessivo de recursos para evitar sobrecarga, garantir estabilidade e manter a qualidade do serviço.

Em sistemas distribuídos, throttling pode ser implementado de diversas maneiras. Quando se trata de APIs, por exemplo, uma implementação típica de throttling seria limitar o número de requisições que um usuário ou cliente pode fazer dentro de um intervalo de tempo específico, como "até 1000 requisições por hora". Caso o limite seja atingido, o sistema pode retornar um erro (geralmente o código HTTP 429 "Too Many Requests"), informando que o cliente precisa esperar antes de tentar novamente.

Esse controle é fundamental para evitar abusos, preservar a performance e prevenir falhas no sistema, que poderiam ocorrer se muitas requisições fossem enviadas em um curto espaço de tempo. O throttling também pode ser usado como uma estratégia de proteger recursos como largura de banda, processamento de CPU, ou banco de dados, onde um número excessivo de requisições pode afetar negativamente o desempenho de toda a aplicação ou rede.

Além disso, throttling também pode ser utilizado em serviços de streaming, onde limita-se a taxa de transmissão de dados, ou em sistemas de filas, onde se controla a quantidade de mensagens processadas ao mesmo tempo, garantindo que o sistema não seja sobrecarregado.

Em alguns cenários, o throttling pode ser combinado com outras técnicas, como backoff exponencial, que aumenta progressivamente o tempo de espera entre as tentativas, permitindo que o sistema recupere sua capacidade de resposta antes de permitir novas operações.

No contexto de redes e protocolos de comunicação, o throttling também pode ser usado para limitar o tráfego de dados e prevenir congestionamento, ajustando a taxa de transmissão de pacotes com base na capacidade do link de rede ou do servidor.

Essa técnica de controle pode ser fundamental para manter a integridade e a escalabilidade dos sistemas, ajudando a garantir que todos os usuários ou clientes tenham uma experiência consistente e estável, sem que um único usuário ou processo sobrecarregue os recursos disponíveis. Throttling é uma técnica utilizada para limitar a taxa de requisições ou operações em um sistema, com o objetivo de controlar o consumo de recursos e evitar sobrecarga. Em contextos de desenvolvimento web ou sistemas distribuídos, throttling serve para regular a quantidade de chamadas que um serviço pode receber em um determinado período de tempo, protegendo-o contra picos de tráfego que poderiam degradar o desempenho ou até mesmo levar a falhas no sistema. Em vez de simplesmente rejeitar todas as requisições que ultrapassem o limite, o throttling "engatinha" a resposta, controlando a velocidade com que elas são processadas, o que permite uma experiência mais estável tanto para o provedor quanto para o consumidor do serviço.

Essa técnica é frequentemente aplicada em APIs, onde é comum definir limites, por exemplo, de 1000 requisições por minuto por usuário, garantindo que ninguém consiga sobrecarregar o sistema com chamadas excessivas. O throttling pode ser implementado em diferentes níveis: na camada de rede, diretamente no servidor, em proxies reversos ou dentro do próprio código da aplicação. Além disso, ele não impede que o cliente faça as requisições; em vez disso, pode, por exemplo, retornar um código de status HTTP 429 (Too Many Requests) quando o limite é alcançado, informando que o usuário deve aguardar um pouco antes de tentar novamente. Assim, o throttling é uma estratégia importante para manter a resiliência, a segurança e a previsibilidade de sistemas complexos.

## [Microservices] PF - Pipe-filter 
No contexto de microsserviços, o padrão **Pipe-Filter (PF)** é uma abordagem arquitetônica que organiza o processamento de dados como um fluxo modular, onde cada etapa de transformação ou manipulação é encapsulada em um componente independente chamado **Filter**, e a comunicação entre esses componentes é feita através de canais estruturados chamados **Pipes**. Esse modelo é inspirado no conceito de pipelines do Unix, onde a saída de um comando (Filter) é direcionada para a entrada do próximo, permitindo a composição de operações complexas a partir de partes simples e reutilizáveis.  

A principal vantagem do Pipe-Filter em microsserviços é a **descentralização do processamento**. Cada Filter pode ser implementado como um microsserviço autônomo, responsável por uma única tarefa específica, como validação, transformação de formato, enriquecimento de dados ou até mesmo chamadas a serviços externos. Por exemplo, em um sistema de processamento de pedidos, um Filter pode validar os dados do cliente, outro pode calcular impostos, e um terceiro pode enviar uma confirmação por e-mail. Os Pipes, por sua vez, são os mecanismos que conectam esses Filters, podendo ser implementados com filas de mensagens (como RabbitMQ ou Kafka), chamadas HTTP/REST, ou até mesmo eventos em um barramento de serviços (Service Bus).  

Essa arquitetura promove **baixo acoplamento** e **alta coesão**, já que cada Filter não precisa conhecer os detalhes internos dos outros – ele apenas consome dados de um Pipe, processa conforme sua regra, e envia o resultado para o próximo Pipe. Isso facilita a manutenção, pois um Filter pode ser modificado ou substituído sem impactar o fluxo geral, desde que mantenha o contrato de entrada e saída. Além disso, o modelo Pipe-Filter é escalável horizontalmente: Filters que demandam mais recursos podem ser replicados para lidar com carga maior, enquanto outros permanecem como instâncias únicas.  

No entanto, o padrão também apresenta desafios. Se os Pipes não forem gerenciados corretamente, podem se tornar gargalos de desempenho, especialmente se houver serialização excessiva de etapas (onde um Filter precisa aguardar o término do anterior). Outro risco é a complexidade de monitoramento, já que um fluxo distribuído exige rastreabilidade entre os microsserviços (com soluções como OpenTelemetry ou logs correlacionados) para diagnosticar falhas ou latências. Além disso, a falta de um orquestrador central pode dificultar a recuperação de erros em cenários onde um Filter falha e os dados precisam ser reprocessados.  

Em resumo, o Pipe-Filter em microsserviços é uma arquitetura poderosa para fluxos de dados previsíveis e modulares, ideal para cenários como ETL (Extract, Transform, Load), processamento de pagamentos ou pipelines de CI/CD. Ele equilibra flexibilidade e simplicidade, mas requer atenção ao design dos Pipes e à resiliência dos Filters para evitar fragilidades no sistema distribuído.

## [Microservices] Blackboard
No contexto de microsserviços, o **Blackboard** (ou "quadro negro") é um padrão de arquitetura inspirado no modelo cognitivo de resolução de problemas, onde múltiplos componentes colaboram de forma assíncrona para processar dados compartilhados em um espaço comum. Ele funciona como um repositório centralizado e temporário de informações, onde diferentes serviços podem ler, escrever e atualizar dados conforme necessário, sem depender de comunicação direta entre si. Essa abordagem é especialmente útil em cenários complexos e dinâmicos, onde a ordem de processamento ou as regras de negócio podem mudar frequentemente.  

A ideia principal do Blackboard é permitir que microsserviços independentes contribuam para uma solução maior de forma incremental, sem acoplamento rígido. Por exemplo, em um sistema de recomendação de produtos, um serviço pode calcular preferências do usuário, outro pode analisar estoque em tempo real, e um terceiro pode aplicar regras de promoção. Todos esses serviços interagem com um Blackboard (como um banco de dados em memória, um message broker ou até um cache distribuído), onde os dados intermediários são armazenados e evoluem até que uma resposta final seja gerada.  

Uma das vantagens desse padrão é a flexibilidade: novos serviços podem ser adicionados ao ecossistema sem impactar os existentes, desde que saibam como ler e escrever no Blackboard. Além disso, ele facilita a paralelização de tarefas, já que múltiplos processos podem trabalhar nos mesmos dados simultaneamente. Ferramentas como **Redis**, **Apache Kafka** ou até bancos de dados compartilhados são frequentemente usadas para implementar esse padrão, dependendo da necessidade de velocidade, persistência ou escalabilidade.  

No entanto, o Blackboard também introduz desafios. Como os dados são compartilhados de forma descentralizada, pode ser difícil garantir consistência imediata (requerendo mecanismos como transações distribuídas ou modelos de eventual consistency). Outro risco é a falta de rastreabilidade: sem um orquestrador claro, identificar qual serviço falhou ou como os dados evoluíram pode se tornar complexo.  

Em resumo, o Blackboard em microsserviços é uma solução poderosa para cenários onde a colaboração assíncrona e a evolução gradual dos dados são necessárias. Ele promove desacoplamento e escalabilidade, mas exige cuidados com monitoramento e governança de dados para evitar que a arquitetura se torne caótica ou difícil de manter.

## [Microservices] Interpreter
No contexto de microsserviços, o **Interpreter** pode ser entendido como um componente ou padrão de design que processa e executa lógica específica em tempo real, muitas vezes dentro de um serviço individual ou no gerenciamento de comunicação entre serviços. Diferente de um interpretador tradicional de linguagens de programação, aqui ele atua mais como um mecanismo que traduz, valida ou executa regras de negócio dinamicamente, sem exigir reimplantações constantes dos serviços.  

Um exemplo comum é o uso de interpretadores para processar scripts ou regras de negócio armazenadas em bancos de dados ou configurações externas. Imagine um microsserviço de pedidos que precisa aplicar diferentes políticas de desconto conforme a região do cliente. Em vez de codificar cada regra diretamente no serviço, um interpretador pode ler essas regras em formato de script (como Lua, JavaScript ou uma DSL – Domain-Specific Language) e aplicá-las sob demanda. Isso permite que as regras sejam alteradas sem a necessidade de modificar e reimplantar o microsserviço, aumentando a flexibilidade do sistema.  

Outro uso frequente é em gateways de API ou orquestradores de microsserviços, onde um interpretador pode processar transformações de payload, validações de contratos ou até mesmo rotear requisições com base em condições dinâmicas. Ferramentas como o **GraphQL**, por exemplo, utilizam interpretadores para resolver queries em tempo real, consultando apenas os microsserviços necessários com base na solicitação do cliente.  

Além disso, em arquiteturas baseadas em eventos (Event-Driven), interpretadores podem ser empregados para decodificar mensagens de filas (como Kafka ou RabbitMQ) e tomar decisões com base no conteúdo. Por exemplo, um serviço de logística poderia usar um interpretador para analisar eventos de rastreamento e disparar ações específicas, como notificações ou ajustes em rotas, sem acoplamento rígido entre os serviços envolvidos.  

A vantagem principal dessa abordagem é a desacoplamento e a agilidade: regras complexas ou lógicas voláteis podem ser gerenciadas externamente, enquanto os microsserviços mantêm uma base estável. Por outro lado, o uso excessivo de interpretadores pode introduzir overhead de desempenho e desafios na depuração, já que a execução dinâmica pode dificultar o rastreamento de erros.  

Em resumo, no universo de microsserviços, o Interpreter atua como um facilitador para operações dinâmicas e adaptáveis, reduzindo a rigidez do código e permitindo que sistemas distribuídos evoluam com menor fricção. Seu uso deve ser balanceado entre flexibilidade e complexidade, garantindo que a manutenibilidade do sistema não seja comprometida.
