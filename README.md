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

**Crie equipes multifuncionais com responsabilidades claras, para ajudar a orquestrar o trabalho entre as equipes**: Uma equipe multifuncional responsável por toda a funcionalidade de microsserviços pode ser um grande benefício para o seu projeto. Essa equipe deve consistir em membros de todas as equipes baseadas em funções e é responsável por orquestrar as várias partes do aplicativo, ou seja, interface do usuário, desenvolvimento, banco de dados e até mesmo controle de qualidade. Se houver duas versões do aplicativo, ou seja, web e mobile, os desenvolvedores de ambas as equipes devem estar presentes nessa equipe. O principal benefício desse tipo de equipe é que fica fácil resolver bugs, desenvolver novos recursos e implantá-los no ambiente de produção.

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

Aqui estão algumas das plataformas de orquestração que já foram comprovadas:

- K8s (Kubernetes)
- AKS (Azure Kubernetes Services)
- ECS (Serviços de Contêineres Elásticos da Amazon)
- Azure Container Apps

Essas plataformas podem ser úteis para gerenciar o provisionamento e implantação de contêineres, balanceamento de carga, escalabilidade, preocupações com comunicação em rede, etc.

Use um sistema de monitoramento eficaz: A arquitetura de microserviços ajuda você a realizar uma enorme escalabilidade de milhares de serviços modulares e oferece potencial para maior velocidade e métodos organizados de monitoramento. É importante, no entanto, revisar todos os seus microserviços e verificar regularmente se eles estão funcionando como desejado e utilizando eficientemente os recursos disponíveis. Dependendo dessas observações, você pode tomar as atitudes apropriadas caso as expectativas não estejam sendo atendidas.

Essa comunicação é muito simples, mas ao mesmo tempo os componentes são altamente acoplados uns aos outros e difíceis de separar e escalar de forma independente.

## [Microservices] Sistemas reativos
<img src="https://img.shields.io/badge/Spring_Boot-3.10.7-gold?style=flat&logo=Spring&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-gold?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/RabbitMQ-16.17.0-gold?style=flat&logo=RabbitMQ&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-16.17.0-gold?style=flat&logo=PostgreSQL&logoColor=white"> <img src="https://img.shields.io/badge/MongoDB-16.17.0-gold?style=flat&logo=MongoDB&logoColor=white"> <img src="https://img.shields.io/badge/Docker-16.17.0-gold?style=flat&logo=Docker&logoColor=white">

<img height="77" align="right" src="https://github.com/user-attachments/assets/b0a85aed-004e-41d8-aad6-8cd4919b2b77" />

Com cada vez mais conexões, mais dados e usuários mais exigentes, manter a responsividade de um sistema de microsserviços tem se tornado uma tarefa dolorosa. Por sorte, isso não precisa ser assim. É para amenizar essa dor que existem os **sistemas reativos**. Sistemas criados como reativos são muito mais flexíveis, desacoplados e escaláveis, o que os torna mais fáceis para desenvolver e mais abertos a mudanças. 

Os sistemas reativos são um design de software, eles são projetados para serem mais responsivos, resilientes, elásticos e orientados por mensagens. Esse paradigma de design é especialmente relevante para sistemas distribuídos e modernos, onde a escalabilidade e a capacidade de lidar com falhas são cruciais. O contexto descrito está relacionado ao paradigma de programação reativa. Estamos destacando os desafios de manter a responsividade e a eficiência em sistemas de microsserviços diante do aumento de conexões, volume de dados e demandas dos usuários, e apresenta os sistemas reativos como uma solução para esses problemas.

A **programação reativa** é um estilo de design de software que foca em responder a eventos de forma assíncrona e não bloqueante. No caso de sistemas distribuídos e modernos, como os de microsserviços, a programação reativa é extremamente útil.

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

Um **API Gateway** é um componente essencial em arquiteturas modernas, especialmente em sistemas baseados em microserviços. Ele atua como um intermediário entre clientes e um conjunto de serviços backend, gerenciando todas as solicitações que entram no sistema. Sua principal função é receber, rotear, transformar e controlar as solicitações de API, além de retornar respostas apropriadas aos clientes. Padrão de API gateway: seu balcão único para microsserviços.

Você está cansado de gerenciar vários pontos de entrada para seus microsserviços? O padrão API Gateway está aqui para salvar o dia! Atuando como um único ponto de entrada para todas as solicitações do cliente, o API Gateway simplifica o acesso aos seus microsserviços, oferecendo comunicação perfeita entre clientes e serviços.

Vamos falar sobre Padrões de Design da arquitetura de Microsserviços, que é o padrão de **Agregação de Gateway** (Gateway Aggregation Pattern). Como você sabe, aprendemos práticas e padrões e os adicionamos à nossa caixa de ferramentas de design. E usaremos esses padrões e práticas ao projetar a arquitetura de microsserviços.

Em sistemas distribuídos, sem um API Gateway, os clientes teriam que se comunicar diretamente com cada microserviço, o que aumentaria a complexidade, exigiria lógica adicional para lidar com autenticação, balanceamento de carga e agregação de dados, além de expor os serviços internos diretamente à internet. O API Gateway resolve esses problemas centralizando essas responsabilidades.

Você precisa aprender onde e quando aplicar o padrão de agregação de gateway na arquitetura de microsserviços com o design de um sistema de aplicativos de comércio eletrônico com os seguintes princípios KISS, YAGNI, SoC e SOLID.

O API Gateway é um servidor que lida com muitas funcionalidades em um único local para os clientes interagirem. Ele também funciona como um proxy reverso entre seus aplicativos cliente e a arquitetura de microsserviços de back-end.

O padrão de agregação de gateway é semelhante ao roteamento de gateway, mas além disso, oferece agregação de serviços. Basicamente, o padrão de agregação de gateway oferece o uso de um serviço de gateway que fornece para agregar várias solicitações internas a microsserviços internos com a exposição de uma única solicitação ao cliente.

Por que você deve se preocupar com o API Gateway? Primeiro, ajuda a agregar respostas de vários microsserviços, reduzindo o número de viagens de ida e volta entre clientes e serviços. Isso resulta em melhor desempenho e experiência do usuário. Em segundo lugar, ele permite que você implemente preocupações transversais, como autenticação, registro e limitação de taxa em um único local, promovendo consistência e reduzindo a redundância.

Imagine a conveniência de ter um hub central que cuida de todas essas responsabilidades! De acordo com um estudo da RapidAPI, 68% dos desenvolvedores que adotaram o API Gateway relataram segurança aprimorada e gerenciamento simplificado de seus microsserviços.

Algumas soluções populares do API Gateway incluem Amazon API Gateway, Kong e Azure API Management. Essas ferramentas fornecem uma variedade de recursos, como cache, limitação e monitoramento, para ajudá-lo a gerenciar seus microsserviços com eficiência.

Esse padrão deve ser usado se o aplicativo cliente tiver que invocar vários microsserviços de back-end diferentes para executar sua lógica. Vamos olhar para a imagem:

<table>
	<tr>
		<td><img height="377" src="https://github.com/user-attachments/assets/6049c51f-5d11-46cd-bb90-ae1e2e6aea27" /></td>
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

<img src="https://github.com/user-attachments/assets/4e8e1f10-ad97-4b15-b570-36eeee8967ac" align="right" height="477">

1. **Roteamento de solicitações**: Ele direciona solicitações para o serviço backend apropriado com base no caminho, método HTTP ou outros critérios.
   
2. **Autenticação e autorização**: Pode validar tokens de acesso, certificados ou outras credenciais antes de encaminhar solicitações aos serviços backend.

3. **Transformação de dados**: Permite manipular solicitações e respostas, como converter formatos (JSON para XML, por exemplo) ou adicionar/remover campos.

4. **Agregação de respostas**: Para solicitações que requerem dados de múltiplos serviços, o API Gateway pode consolidar essas respostas antes de retornar ao cliente.

5. **Limitação de taxa e controle de acesso**: Garante que o sistema não seja sobrecarregado, implementando políticas de limite de solicitações por usuário ou IP.

6. **Monitoramento e métricas**: Coleta dados de uso e desempenho para fornecer insights sobre o funcionamento das APIs.

7. **Segurança e proteção**: Oferece proteção contra ataques comuns, como DDoS e injeções maliciosas, ao atuar como uma camada de firewall para APIs.

Um exemplo prático é em uma aplicação de e-commerce: o API Gateway pode expor uma única API para os clientes acessarem, enquanto internamente roteia solicitações para microserviços como autenticação, catálogo de produtos, carrinho de compras e pagamentos.

Ferramentas populares para implementação de API Gateways incluem **Kong**, **NGINX**, **AWS API Gateway**, **Apigee**, **Traefik** e **Istio** (quando usado em conjunto com service meshes). Em resumo, o API Gateway é uma peça fundamental para simplificar a gestão, aumentar a segurança e otimizar a performance de APIs em arquiteturas modernas.

<img width="1381" height="890" alt="1_NAwTMDfUtNv3YB1Mebm1xA" src="https://github.com/user-attachments/assets/be3e0ab6-fd21-4d5a-9a52-03b094a1d828" />

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

## [Microservices] CQRS - Command-query responsability segregation
<img src="https://img.shields.io/badge/Spring_Boot-3.10.7-gold?style=flat&logo=Spring&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-16.17.0-gold?style=flat&logo=Node.js&logoColor=white"> <img src="https://img.shields.io/badge/RabbitMQ-16.17.0-gold?style=flat&logo=RabbitMQ&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-16.17.0-gold?style=flat&logo=PostgreSQL&logoColor=white"> <img src="https://img.shields.io/badge/Apache_Cassandra-16.1-gold?style=flat&logo=Apache-Cassandra&logoColor=white"> <img src="https://img.shields.io/badge/MongoDB-16.17.0-gold?style=flat&logo=MongoDB&logoColor=white"> <img src="https://img.shields.io/badge/Docker-16.17.0-gold?style=flat&logo=Docker&logoColor=white">

<img src="https://github.com/user-attachments/assets/ae249146-7dec-47c3-86a1-beb52b42c23e" height="277" align="right">

O **CQRS (Command-Query Responsibility Segregation)** é um padrão arquitetural que separa as operações de escrita **comandos** (`command`) das operações de leitura **consultas** (`query`) em um sistema, atribuindo responsabilidades distintas para cada uma delas. Em vez de usar o mesmo modelo de dados e lógica para lidar tanto com as atualizações quanto com as consultas, o CQRS propõe que esses dois aspectos sejam tratados de maneira independente, o que permite otimizações específicas para cada cenário. 

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

## [Microservices] SAGA
<img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/Medium-Saga-blue?style=flat&logo=Medium&logoColor=white"> <img src="https://img.shields.io/badge/DEV-Saga-blue?style=flat&logo=dev.to&logoColor=white"> <img src="https://img.shields.io/badge/GitBook-Saga-blue?style=flat&logo=GitBook&logoColor=white"> <img src="https://img.shields.io/badge/Confluence-Saga-blue?style=flat&logo=Confluence&logoColor=white">

<img src="https://github.com/user-attachments/assets/54637f6c-1d52-43e8-bfbd-f59840a423b8" align="right" height="77">

O padrão **Saga** é uma abordagem para gerenciar transações distribuídas em uma arquitetura de microsserviços. Em sistemas distribuídos, uma **transação** (transaction) pode envolver múltiplos microsserviços, o que torna o uso de transações tradicionais (como as que utilizam o protocolo de commit em duas fases) impraticável devido à complexidade e ao impacto na performance. O padrão Saga oferece uma maneira de garantir a consistência dos dados e a execução das transações em tais sistemas. O padrão Saga é frequentemente associado ao conceito de Long-Running Transactions (LRTs).

> SAGA pode ser descrito como uma sequência de transações que podem ser intercaladas com outras transações.

Nos aprofundamos no intrincado mundo das transações distribuídas através das lentes do padrão SAGA, uma estratégia fundamental para gerenciar a consistência de dados em arquiteturas de microsserviços descentralizadas. Com o brilho dos microsserviços, o SAGA é quase a solução ideal quando se trata de transações distribuídas, entender como lidar efetivamente com transações que abrangem vários serviços torna-se crucial. Esta discussão visa não apenas esclarecer os princípios fundamentais dos SAGAs, mas também fornecer insights práticos sobre sua aplicação estratégica, garantindo interações robustas e sem erros dentro de seus serviços.

Uma compreensão fundamental dos microsserviços é essencial para compreender totalmente as nuances das SAGAs. Recomenda-se que os leitores tenham familiaridade com os vários mecanismos de comunicação empregados em arquiteturas de microsserviços. Para aqueles que buscam aprofundar seus conhecimentos, convido você a ler meu post detalhado no blog, <a href="https://medium.com/@joudwawad/a-guide-to-communication-styles-in-microservices-architecture-9a8ae4bc21b2">"Um Guia para Estilos de Comunicação na Arquitetura de Microsserviços"</a>, que oferece uma análise aprofundada sobre esse assunto.

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/be0e8414-d158-4c2e-bd18-65718528780d">

Da arquitetura monolítica à arquitetura de microsserviços, quase todas as solicitações tratadas por um aplicativo empresarial são executadas em uma transação de banco de dados. Os desenvolvedores de aplicativos corporativos usam estruturas e bibliotecas que simplificam o gerenciamento de transações. Algumas estruturas e bibliotecas fornecem uma API programática para iniciar, confirmar e reverter transações explicitamente. Outras estruturas, como a estrutura Spring, fornecem um mecanismo declarativo.

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

## [Microservices] Event-bus
<img src="https://em-content.zobj.net/source/microsoft-teams/400/bus_1f68c.png" align="right" height="77">

Um **event-bus** é um mecanismo de comunicação baseado em eventos que funciona como um canal central por onde diferentes partes de um sistema enviam e recebem mensagens sem depender diretamente umas das outras. Em vez de um componente chamar o outro de forma direta, criando acoplamento e dependências rígidas, tudo passa pelo barramento: um serviço “publica” um evento e qualquer outro serviço interessado “ouve” esse evento e reage a ele. Isso produz um fluxo muito mais solto, assíncrono e escalável, porque nada precisa saber quem vai consumir a informação; basta emitir o acontecimento e deixar o barramento cuidar da distribuição.

A função essencial do event-bus é organizar essa comunicação assíncrona. Ele recebe eventos — que podem representar mudanças de estado, ações do usuário, comunicação entre microsserviços ou notificações internas — e encaminha tudo para os assinantes corretos. Em sistemas distribuídos, isso significa que um backend pode emitir um evento de “pedido criado”, por exemplo, e vários serviços podem reagir de formas diferentes: um calcula frete, outro atualiza estoque, outro envia e-mail. Nada disso exige que esses serviços se conheçam diretamente, porque o event-bus faz o papel de conector invisível entre todos eles.

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

## [Microservices] Outbox Pattern
<img height="177" align="right" src="https://github.com/user-attachments/assets/ea001cdf-436e-41ce-a04c-cb74872359bc" />

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

> A arquitetura Onion pode ser utilizada em uma arquitetura de microsserviços. Na verdade, muitos dos princípios da Onion Architecture se alinham bem com os objetivos e práticas de desenvolvimento de microsserviços. A Onion Architecture pode ser uma abordagem eficaz para estruturar microsserviços, promovendo um design desacoplado, testável e fácil de manter. Ao aplicar os princípios da Onion Architecture, cada microsserviço pode ser desenvolvido de forma independente, mantendo a lógica de negócios centralizada e livre de dependências externas desnecessárias.

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

## [Microservices] DDD - Domain-Driven Design

## [Microservices] Hexagonal architecture (Ports & Adapters)

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
