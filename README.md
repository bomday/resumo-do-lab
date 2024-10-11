# Resumo do Lab

## Conceitos Gerais

💡 Pode-se controlar os serviços pelo desktop ou celular (com limitações)
</br>
💡 Princípio de pagar pelo que usa (Economiza custos) - “**Pay as you go**”
</br>
💡 Comparação AWS X AZURE: [Comparação entre os serviços do AWS e do Azure - Azure Architecture Center | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/architecture/aws-professional/services)

### CapEx X OpEx

**CapEx** → Despesa de Capital. Gasto inicial em Infra Física. O valor dessas despesas se reduz com o tempo.

**OpEx** → Despesas Operacionais. Gastos operacionais. Você paga pelo que usa, continuamente.

### Conceitos de Cloud

```
-> Alta disponibilidade
-> Escalabilidade
-> Agilidade
-> Distribuição Geográfica
-> Recuperação de desastres
-> Resource Pooling (Usuários não acessam recursos de outros clientes)
```

## **Modelos de Cloud**

### Quais são os diferentes tipos de serviços de computação em nuvem?

Os **tipos de computação em nuvem são modelos de implantação de serviço que permitem a seleção do nível de controle sobre as informações e tipos de serviço** que precisam ser fornecidos. Há **três tipos principais** de serviços de computação em nuvem, às vezes chamados de pilha de computação em nuvem, pois são compilados um sobre o outro.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/7327b09c-cc90-4779-843c-102f9a2c4587/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/fbbf6409-aeea-4775-91b3-2bd5b31ed495/Untitled.png)

O primeiro tipo de computação em nuvem é a [infraestrutura como serviço (IaaS)](https://azure.microsoft.com/pt-br/overview/what-is-iaas/), usada para acesso à recursos de computação e armazenamento baseados na Internet. Sendo a categoria mais básica entre os tipos de computação em nuvem, a IaaS permite que você alugue uma infraestrutura de TI (servidores e máquinas virtuais, armazenamento, redes e sistemas operacionais) de um provedor de nuvem em uma base paga conforme o uso.

O segundo tipo de computação em nuvem é a [plataforma como serviço (PaaS)](https://azure.microsoft.com/pt-br/overview/what-is-paas/), que dá aos desenvolvedores as ferramentas necessárias para criar e hospedar aplicativos Web. A PaaS foi desenvolvida para proporcionar aos usuários o acesso aos componentes necessários para desenvolver e operar rapidamente aplicativos Web ou móveis na Internet, sem se preocupar com a configuração ou gerenciamento da infraestrutura subjacente dos servidores, armazenamento, redes e bancos de dados.

```
**Principais serviços:**

- CDN
- Cosmos DB
- Azure SQL Databases
- Azure Database for MySQL
- Storage
- Synapse Analytics
```

```
**Outros Frameworks:**

- ASP.NET
- .NET
- Java
- Node.js
- PHP
- Python
```

O terceiro tipo de computação em nuvem é o [software como serviço (SaaS)](https://azure.microsoft.com/pt-br/overview/what-is-saas/), usado para aplicativos baseados na Web. O SaaS é um método de entrega de aplicativos de software na Internet, no qual os provedores de nuvem hospedam e gerenciam os aplicativos de software, fazendo com que seja simples ter o mesmo aplicativo em todos seus dispositivos de uma só vez por meio da nuvem. Ex.: OneDrive, Xbox Live e Microsoft 365.

A Azure é excelente nos 3 tipos.

## Computação *Serverless*

Sobrepondo o PaaS, a computação sem servidor permite que os desenvolvedores criem aplicativos com rapidez, **eliminando a necessidade de gerenciar a infraestrutura**.

A questão do *serverless* basicamente é a seguinte: eu não vou me preocupar em qual hardware, onde, como ele vai rodar. Nada disso me importa, é totalmente transparente.

Em qual servidor ele vai rodar? Quanto de memória? É totalmente transparente. Nós vamos, lógico, definir alguns princípios mínimos para que ele execute e ele vai usar o hardware necessário, ele vai gerenciar esse hardware para mim.

A alocação de infra será feita automaticamente, inclusive a escala disso. Você pode escalar isso automaticamente, sem você ter que, por exemplo, ampliar o teu parque de máquinas virtuais. Você tinha que estar preparado para isso.

Com o *serverless* isso é totalmente transparente. Coloquei meu código, se ele vai precisar de 30 computadores ou um computador para rodar, é totalmente transparente para nós.

Eles são **sistemas altamente escaláveis e dirigidos por eventos**, onde utilizam os recursos apenas quando a função específica é usada.

## **Tipos de Cloud**

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/58c3541f-13af-4212-a814-cc6d6eb0c1f7/Untitled.png)

### **O que é nuvem privada?**

Uma nuvem privada consiste em recursos de computação em nuvem usados exclusivamente por uma única empresa ou organização. A nuvem privada pode estar localizada fisicamente no datacenter local da sua organização ou pode ser hospedada por um provedor de serviços terceirizado. Mas em uma nuvem privada, os serviços e a infraestrutura são sempre mantidos na rede privada e o hardware e o software são dedicados unicamente à sua organização.

Dessa forma, com a nuvem privada é mais fácil para que a organização personalize seus recursos a fim de atender a requisitos de TI específicos. As nuvens privadas geralmente são usadas por órgãos governamentais, instituições financeiras e outras organizações de grande porte com operações críticas para os negócios, que buscam melhorar o controle sobre seu ambiente.

Vantagens de uma nuvem privada:

- **Maior flexibilidade** – sua organização pode personalizar seu ambiente de nuvem para atender a necessidades de negócios específicas.
- **Maior controle** – os recursos não são compartilhados com outros usuários, portanto, é possível um nível maior de controle e privacidade.
- **Maior escalabilidade** –nuvens privadas geralmente oferecem mais escalabilidade em comparação com a infraestrutura local.

### **O que é uma nuvem pública?**

As nuvens públicas (providas por alguém e utilizada por outras pessoas) são a maneira mais comum de implantação da computação em nuvem. Os recursos de nuvem (como servidores e armazenamento) pertencem a um provedor de serviço de nuvem terceirizado, são operados por ele e entregues pela Internet. Com uma nuvem pública, todo o hardware, software e outras infraestruturas de suporte são de propriedade do provedor de nuvem e gerenciadas por ele. O Microsoft Azure é um exemplo de nuvem pública.

Em uma nuvem pública, você compartilha os mesmos dispositivos de hardware, de armazenamento e de rede com outras organizações ou "locatários" da nuvem e acessa serviços e gerencia sua conta usando um navegador da Web. As implantações de nuvem pública geralmente são usadas para fornecer email baseado na Web, aplicativos de escritório online, armazenamento e ambientes de desenvolvimento e teste.

Vantagens das nuvens públicas:

- **Redução de custos** – não há necessidade de comprar hardware ou software e você paga somente pelos serviços que usa.
- **Sem manutenção** – seu provedor de serviços fornece a manutenção.
- **Escalabilidade quase ilimitada** – recursos sob demanda estão disponíveis para atender às suas necessidades de negócios.
- **Alta confiabilidade** – uma ampla rede de servidores assegura contra falhas.

### Computação em nuvem híbrida

Uma nuvem híbrida é um tipo de computação em nuvem que combina uma infraestrutura local ou nuvem privada com uma nuvem pública. As nuvens híbridas permitem que os dados e aplicativos se movam entre os dois ambientes.

Muitas organizações adotam a abordagem de nuvem híbrida devido a exigências comerciais, por exemplo, para atender a requisitos regulatórios e de soberania de dados, aproveitar ao máximo o investimento em tecnologia local ou lidar com problemas envolvendo latência baixa.

A nuvem híbrida está evoluindo para incluir cargas de trabalho de borda também. A computação de borda traz a potência de computação da nuvem para dispositivos IoT, mais perto de onde os dados residem. Ao mover as cargas de trabalho para a borda, os dispositivos gastam menos tempo se comunicando com a nuvem, o que reduz a latência e permite a eles até mesmo operar de maneira confiável por períodos offline estendidos.

A microsoft oferece a Microsoft Azure Stack para facilitar a implementação de um modelo híbrido.

## **Benefícios de Cloud**

### **1. Flexibilidade**

Para executar com eficácia uma estratégia de transformação digital, uma empresa precisará girar seu processo de negócios várias vezes. A computação em nuvem poupa uma organização do trabalho de investir em vários recursos de TI, fornecendo recursos de computação, infraestrutura, banco de dados e plataformas em trânsito. Isso permite que uma empresa seja ágil e flexível.

### **2. Custo-benefício**

Juntamente com a flexibilidade de ajustar os requisitos, a nuvem oferece um modelo de serviço escalável, em que uma empresa paga apenas pelos recursos usados. Assim, não apenas economiza o custo de capital na compra e no gerenciamento da infraestrutura de TI, mas também ajuda as empresas a dimensionar seus recursos com base nos requisitos.

### **3. Segurança**

Se o seu banco de dados é armazenado internamente, você enfrenta constantemente o risco de perder informações críticas devido a violações de dados, desligamentos inesperados do sistema, desastres, ataques de cibercriminosos etc.

No caso de hospedagem em nuvem, você pode criar facilmente vários backups de seus dados. Isso é especialmente benéfico ao lidar com Big Data, pois as chances de falhas do sistema aumentam significativamente nesse caso.

### **4. Prototipagem rápida**

Para que a transformação digital funcione e a cultura de inovação seja implantada, uma empresa precisa inovar, testar e repetir continuamente.

O cloud computing pode fornecer às empresas uma plataforma em que podem facilmente criar, testar e implantar aplicativos sem a necessidade de configurar uma infraestrutura complexa. Assim, durante a fase de transformação, uma empresa pode experimentar vários aplicativos em diferentes plataformas.

Deploy de novas versões vai permitir entrega contínua com muito menos probabilidade de problemas. 

### **5. Melhor colaboração**

A transformação digital exige que uma empresa se adapte a uma cultura de inovação e criatividade e deixe a antiga cadeia hierárquica de comandos. A computação em nuvem permite que os arquivos sejam acessados de qualquer lugar e a qualquer momento.

Também é possível controlar o nível de autoridade do usuário, garantindo assim a delegação ideal. No geral, ajuda a criar uma atmosfera de colaboração e trabalho em equipe na empresa.

Todos esses benefícios sugerem claramente que, se você criar uma cultura de inovação em sua empresa, a nuvem é uma solução lógica e ideal.

### **6. Disponibilidade**

Alto Service Level Agreement (SLA) → Porcentagem de garantia para que o sistema esteja disponível. 

Vai ser mais difícil que quedas de energia, falhas na aplicação, quedas de máquinas virtuais , quedas de rede, problemas no banco de dados, entre outros problemas ocorram. Já não vai depender da capacidade de você e da sua empresa, já que é um serviço externo. 

Qual a indisponibilidade aceitável?

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/e955b551-c1d1-4a38-85c9-a62293273337/image.png)

### **7. Escalabilidade**

2 tipos de escala (Pode adicionar ou retirar): 

- Scale UP → Vertical, Adiciona CPU, Adiciona Memória, Adição de Discos…
- Scale Out → Horizontal, Duplica VM, Duplicar Database Servers…

Automatiza monitoramento e controle dos processos, realizando ações a partir dos indicadores.

Como escalar:

- Baseado em Consumo
- Baseada em hora do dia

## Infraestrutura: Regiões AZ (Parte Física Azure)

1. Geografia
2. Região
3. Zona de disponibilidade

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/b844835c-53aa-4200-b3cd-ceef64438141/Untitled.png)

- Mínimo 3 Zonas de Disponibilidade para se criar uma Região AZ;
- Mínimo uma Região por geografia (normalmente, são duas);
- Cria “Cópias” em tempo quase instantâneo para caso uma Zona se torne indisponível os dados não sejam perdidos;
- As zonas são interligadas por fibras de baixa latência (redes com tempos de resposta rápidos);
- Regiões separadas por longas distâncias;
- Brasil é um país caro para manter nuvem;
- É interessante pagar por regiões onde se concentrem maior parte dos seus clientes para estar mais próxima do seu cliente;
- Alguns produtos só estão disponíveis em regiões ou zonas de disponibilidade específicas.

- Serviços suportados pelas zonas de disponibilidade:
    1. VMs (com ou sem Scale Stes)
    2. Azure Kubernets Services
    3. Managed Disks
    4. Zonal Redudant Storage
    5. Standart Load Balancers
    6. Standart IP Address
    7. VPN Gateway
    8. Route Gateway
    9. Azure Firewall
    10. Data Explore
    11. Azure SQL Database
    12. Azure Cash For Redis
    13. Cosmos DB
    14. Event Hubs
    15. Service Bus (Premium Tier)
    16. Event Grid
    17. AD Domain Services
    18. APP Services
    

Existem 2 Categorias de serviços que suportam **Availability Zones**:

- Zonal Services
- Zone Redundant Services

### Exemplos de Zonal Services:

- Máquinas Virtuais
- Discos usados nessas Máquinas Virtuais
- IPs públicos atribuídos a essas máquinas Virtuais.

Se você quer Alta Disponibilidade(HA) para serviços dos tipos Zonal Services, você precisa explicitamente fazer o Deploy desses Serviços em mais de 1 zona. Isso porque os IPs e discos de uma máquina virtual são automaticamente configurados para a mesma zona de disponibilidade da Máquina Virtual criada.

### Exemplos de Zone Redundant Services:

- Redundant Storage
- SQL Databases.

No caso do storage a Feature que o faz Zone Redundant é o ZRS.

## Infraestrutura: Grupo de Recursos (Parte Virtual Azure)

- Quando você utiliza um serviço da Azure, você tem que associá-lo a um grupo de recursos para gerenciamento;
- Um recurso só pode pertencer a um grupo de recursos;
- Criação de grupos depende da organização do seu negócio;

Exemplos: 

1. Cria grupo de servers onde pode acessar lista de todos os servers gerenciados.
2. Criar grupo por estado onde vê o que cada estado tem.
- Com esses grupos você consegue acompanhar os custos gerados por cada um;
- ARM (Azure Resource Manager): Aplicação/Serviço/Software que gerencia todos os recursos e sabe as informações de cada um deles. É uma ferramenta de deploy e gerenciamento de serviços. Utiliza a notação JSON para realizar deploys;
- Benefícios ARM: Deploy de múltiplos recursos de uma vez, Reproduz deploys de forma consistente, Cria templates declarativos (fácil de entender) e setup de dependências.

## **Precificação**

[Azure Pricing Overview | Microsoft Azure](https://azure.microsoft.com/en-us/pricing/) 

- Pricing by Product (Por produto)
- Pricing Calculator (Estimativas)
- TCO Calculator (Comparativo)

Planos de suporte: [Azure Support Plans Comparison | Microsoft Azure](https://azure.microsoft.com/en-us/support/plans/)

## Opções de pagamento - VMs

- Pay as you go (sob demanda) **MAIOR VALOR**
- Reserved Virtual Machines Instances (reserva)
- Spot Princing (Usar capacidade ociosa das VMs e podem ser interrompidas pela Microsoft a qualquer momento - bom se você vai usar em serviços que não precisam de disponibilidade 24h) **MENOR VALOR**

## Serviços de Computação

Existe várias ferramentas que realizam o provimento de computação.

- Azure Virtual Machines
- Azure App Services (Serviço para provisionar sua aplicação sem administrar infraestrutura)
- Azure Container Instances (Docker etc roda sem orquestração - para serviços maiores se utiliza o Kurbenets)
- Azure Kubernets Service (Serviço para orquestrar e gerenciar conjunto de containers)
- Windows Virtual Desktop (Provisão de estações de trabalhos ex.: equipe trabalha com linux mas precisa usar windows as vezes, ent pega um serviço desse para desktops virtuais. Não necessariamente terá o windows instalado no aparelho)

- Azure Functions (Serveless - crio código, faço deploy e azure irá rodar ela automaticamente)
    
    → Event-Trigger é algo que vai gatilhar a execução da função (código) gerando a Azure Function
    
    [Gatilhos e associações no Azure Functions | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/azure-functions/functions-triggers-bindings)
    

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/15bc9fd2-c7f2-4dc2-9e04-62e81d32a07a/Untitled.png)

## Rede

É o bloco de construção fundamental, ou seja, é a base para que possamos fazer a nossa rede privada dentro da Azure. Ele chama de VNet que é uma abreviação. A VNet vai habilitar vários tipos de recursos, inclusive, a questão de VM e tudo o mais para que tenhamos a comunicação entre elas, entra a internet, entre até mesmo a rede *On-Premise*.
VNet, as Virtual Network são as bases, são propriamente a rede que vamos criar dentro da Azure para poder trabalhar e colocar efetivamente as nossas coisas lá dentro.

### Tipos

1) Rede Virtual (VNet criada dentro da Rede)

2) Load Balancer (faz *health check* validando a saúde do seu *backend*) → Layer 4 (IP e porta)

Na Azure, existem os **públicos e privados (internos)**.

**Imagem ao lado representa o load balancer público:** Tenho um *Load Balancer*, chegou o acesso na porta 80, o nosso acesso HTTP. Chegou à requisição e qual é a responsabilidade do seu *Load Balancer*? Entregar o tráfego para o *pool* de máquinas que tem aqui atrás.

Posso ter um ***Load Balancer* na frente da minha aplicação para os meus endereços internos**. Tenho um servidor que fala com a minha aplicação, isso na minha rede interna, e quero balancear essa aplicação. 

Antes não era possível balanceamento no protocolo ICMP: [General availability: Inbound ICMPv4 pings are now supported on Azure Load Balancer | Azure updates | Microsoft Azure](https://azure.microsoft.com/en-us/updates/general-availability-inbound-icmpv4-pings-are-now-supported-on-azure-load-balancer/)

Standard Public Load Balancer now supports inbound ICMP pings on IPv4 frontends. Previously, to determine reachability of a Load Balancer’s frontend, a TCP-based ping tool like Psping would need to be used.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/e234bf56-98df-4d1f-a68a-d996e2933e24/Untitled.png)

3) VPN Gateway (Pode conectar diretamente pra Azure através de uma VPN, estendendo a LAN para a nuvem)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/53848409-d96e-41c0-84f3-16c23ccf6748/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/12d24a9a-f50a-4b38-a42c-8f4a70a7968b/Untitled.png)

4) Application Gateway → Layer 7 (trabalhar dentro do HTTP e olhar cabeçalho, olhar a URL e coisas desse tipo) 

Recebe um tráfico e direciona, por exemplo, tenho dois servidores atrás desse Application Gateway, posso direcionar tudo o que for imagem para um servidor e o resto das páginas estáticas, os HTML e tudo o mais direciona para outro servidor

[Recursos do Gateway de Aplicativo do Azure | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/application-gateway/features)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/3fbfbbfc-8daa-462f-988f-4c10e58d848d/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/71b172b5-2d58-48d8-b079-29fe1f07635d/Untitled.png)

5) ExpressRoute (conecto diretamente a minha estrutura, o *On-Premise* com a nuvem através de um link dedicado) https://docs.microsoft.com/pt-br/azure/vpn-gateway/design

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/534b7a1c-8a68-4219-bd9a-5470f7f5e4cf/Untitled.png)

6) Content Delivery Network (CDN) (Ganha performance) [Azure Content Delivery Network POP locations by region | Microsoft Learn](https://learn.microsoft.com/en-us/azure/cdn/cdn-pop-locations)

CDN vai oferecer aos desenvolvedores uma solução global para entrega rápida com alta bandar, largura de banda, para que o nosso conteúdo possa ser entregue aos usuários rapidamente.

Como funciona? Colocamos isso em ***cash***. Mais fácil para usuário buscar uma informação de um servidor que já está próximo dele, em *cash*, do que ele vir até o servidor de origem. Até pela questão física, ele tem proximidade com esse servidor e ele vai pegar o dado mais rápido.

No caso do Azure CDN você também pode acelerar **conteúdo dinâmico**. Esse meu conteúdo dinâmico é provisionado através do que a Azure chama de POPs. Esses POPs são pontos de acesso.

São pontos de acesso da própria rede que compõe a infraestrutura da Azure. Já acesso um servidor que já está dentro da Azure e esse servidor tem a conexão muito mais rápida porque já está tudo na nuvem da Azure. É muito mais rápido do que eu fazer a ponta do meu cliente direto com o meu servidor de aplicação.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/7b095ca6-eec7-40fc-ae19-36191668c7f8/Untitled.png)

**OBS.:** 

→ On-premise refere-se a um tipo de ambiente de TI onde todos os sistemas, servidores e dados estão localizados dentro da infraestrutura da própria empresa. 

**→ Load Balancer e Application Gateway são serviços parecidos em níveis diferentes**

**→ Express Route e VPN também são serviços parecidos. Precisou de link direto? "ExpressRoute". Posso baratear esse custo. Não quero ter um link direto e posso e tenho a opção de transacionar as informações pela internet, uso o VPN.** 

### Conceitos Rede Virtual/VNet

- Espaço de Endereçamento (Atribuição dos IPs dentro de uma rede)
- Subnets (funcionamento dessa Virtual Network posso dizer que é bem similar ao funcionamento de uma rede normal)
- Regiões (Ter redes por regiões - independentes ou com comunicação)
- Assinaturas (dentro de uma assinatura posso ter várias redes)

## **Azure Big Data**

### Estilo de arquitetura de Big Data

Uma arquitetura de Big Data foi projetada para lidar com ingestão, processamento e análise de dados grandes ou complexos demais para sistemas de banco de dados tradicionais.

Soluções de Big Data normalmente envolvem um ou mais dos seguintes tipos de carga de trabalho:

- Processamento em lote de fontes Big Data em repouso.
- Processamento em tempo real de Big Data em movimento.
- Exploração interativa de Big Data.
- Análise preditiva e machine learning.

A maioria das arquiteturas de Big Data inclui alguns ou todos os seguintes componentes:

- **Fontes de dados**: todas as soluções de Big Data começam com uma ou mais fontes de dados. Os exemplos incluem:
    - Armazenamentos de dados de aplicativo, como bancos de dados relacionais.
    - Arquivos estáticos produzidos por aplicativos, como arquivos de log do servidor Web.
    - Fontes de dados em tempo real, como dispositivos IoT.
- **Armazenamento de dados**: dados de operações de processamento em lote normalmente são armazenados em um repositório de arquivos distribuído que pode conter amplos volumes de arquivos grandes em vários formatos. Esse tipo de repositório geralmente é chamado *data lake*. As opções para implementar esse armazenamento incluem contêineres de blobs ou Azure Data Lake Store no Armazenamento do Azure.
- **Processamento em lote**: como os conjuntos de dados são muito grandes, geralmente uma solução de Big Data deve processar arquivos de dados usando trabalhos de lote de execução longa para filtrar, agregar e preparar os dados para análise. Normalmente, esses trabalhos envolvem ler arquivos de origem, processá-los e gravar a saída para novos arquivos. Opções incluem executar trabalhos de U-SQL no Azure Data Lake Analytics, usar trabalhos Hive, Pig ou de Mapear/Reduzir personalizados em um cluster HDInsight Hadoop ou usar programas de Java, Scala ou Python em um cluster HDInsight Spark.
- **Ingestão de mensagens em tempo real**: se a solução inclui fontes em tempo real, a arquitetura deve incluir uma maneira de capturar e armazenar mensagens em tempo real para processamento de fluxo. Isso pode ser um armazenamento de dados simples, em que as mensagens de entrada são removidas para uma pasta para processamento. No entanto, muitas soluções precisam de um repositório de ingestão de mensagens para atuar como buffer de mensagens e dar suporte a processamento de expansão, entrega confiável e outras semânticas de enfileiramento de mensagem. Opções incluem Hubs de Eventos do Azure, Hubs de IoT do Azure e Kafka.
- **Processamento de fluxo**: depois de capturar mensagens em tempo real, a solução deve processá-las filtrando, agregando e preparando os dados para análise. Os dados de fluxo processados são gravados em um coletor de saída. O Azure Stream Analytics oferece um serviço de processamento de fluxo gerenciado baseado em consultas SQL em execução perpétua que operam em fluxos não associados. Você também pode usar tecnologias de streaming Apache de software livre, como Storm e Spark Streaming em um cluster HDInsight.
- **Armazenamento de dados analíticos**: muitas soluções de Big Data preparam dados para análise e então veiculam os dados processados em um formato estruturado que pode ser consultado usando ferramentas analíticas. O armazenamento de dados analíticos usado para atender a essas consultas pode ser um data warehouse relacional estilo Kimball, como visto na maioria das soluções de BI (business intelligence) tradicionais. Como alternativa, os dados podem ser apresentados por meio de uma tecnologia NoSQL de baixa latência, como HBase ou um banco de dados Hive interativo que oferece uma abstração de metadados sobre arquivos de dados no armazenamento de dados distribuído. O Azure Synapse Analytics fornece um serviço gerenciado para armazenamento de dados em larga escala baseado em nuvem. O HDInsight dá suporte a Hive interativo, HBase e Spark SQL, que também pode ser usado para veicular dados para análise.
- **Análise e relatório**: a meta da maioria das soluções de Big Data é gerar insights sobre os dados por meio de análise e relatórios. Para capacitar os usuários a analisar os dados, a arquitetura pode incluir uma camada de modelagem de dados, como um cubo OLAP multidimensional ou um modelo de dados tabular no Azure Analysis Services. Também pode dar suporte a business intelligence de autoatendimento, usando as tecnologias de modelagem e visualização do Microsoft Power BI ou do Microsoft Excel. Análise e relatórios também podem assumir a forma de exploração de dados interativos por cientistas de dados ou analistas de dados. Para esses cenários, muitos serviços do Azure dão suporte a blocos de anotações analíticos, como Jupyter, permitindo que esses usuários aproveitem suas habilidades existentes com Python ou R. Para exploração de dados em larga escala, você pode usar o Microsoft R Server, seja no modo autônomo ou com Spark.
- **Orquestração**: a maioria das soluções de Big Data consiste em operações de processamento de dados repetidos, encapsuladas em fluxos de trabalho, que transformam dados de origem, movem dados entre várias origens e coletores, carregam os dados processados em um armazenamento de dados analíticos ou efetuam o push dos resultados diretamente para um relatório ou painel. Para automatizar esses fluxos de trabalho, você pode usar uma tecnologia de orquestração, como Azure Data Factory ou Apache Oozie e Sqoop.

O Azure inclui muitos serviços que podem ser usados em uma arquitetura de Big Data. Eles se enquadram em aproximadamente duas categorias:

- Serviços gerenciados, incluindo o Azure Data Lake Store, Azure Data Lake Analytics, Azure Synapse Analytics, Azure Stream Analytics, Hub de Eventos do Azure, Hub IoT do Azure e Azure Data Factory.
- Tecnologias de software livre baseadas na plataforma Apache Hadoop, incluindo HDFS, HBase, Hive, Pig, Spark, Storm, Oozie, Sqoop e Kafka. Essas tecnologias estão disponíveis no Azure no serviço Azure HDInsight.

Essas opções não se excluem mutuamente e muitas soluções combinam tecnologias de software livre com serviços do Azure.

### Quando usar essa arquitetura

Considere este estilo de arquitetura quando você precisar:

- Armazenar e processar dados em volumes muito grandes para um banco de dados tradicional.
- Transformar dados não estruturados para análise e relatório.
- Capturar, processar e analisar fluxos não associados de dados em tempo real ou com baixa latência.
- Usar Azure Machine Learning ou Serviços Cognitivos da Microsoft.

### Benefícios

- **Opções de tecnologia**. Você pode combinar gerenciados serviços do Azure e tecnologias Apache em clusters HDInsight para aproveitar recursos ou investimentos em tecnologia existentes.
- **Desempenho por meio de paralelismo**. Soluções de Big Data aproveitam paralelismo, possibilitando soluções de alto desempenho dimensionadas para grandes volumes de dados.
- **Escala elástica**. Todos os componentes da arquitetura de Big Data dão suporte a provisionamento de expansão para que você possa ajustar sua solução para cargas de trabalho grandes ou pequenas e pagar somente pelos recursos que usa.
- **Interoperabilidade com soluções existentes**. Os componentes da arquitetura de Big Data também são usados para processamento IoT e soluções de BI empresariais, permitindo que você crie uma solução integrada entre cargas de trabalho de dados.

### Desafios

- **Complexidade**. Soluções de Big Data podem ser extremamente complexas, com vários componentes para lidar com a ingestão de dados de várias fontes de dados. Pode ser um desafio criar, testar e solucionar problemas de processos de Big Data. Além disso, pode haver um grande número de definições de configuração em vários sistemas que devem ser usados para otimizar o desempenho.
- **Conjunto de qualificações**. Muitas tecnologias de Big Data são altamente especializadas e usam frameworks e idiomas que não são típicos de arquiteturas de aplicativo mais gerais. Por outro lado, as tecnologias de Big Data estão gerando novas APIs que se baseiam em linguagens mais estabelecidas. Por exemplo, a linguagem U-SQL no Azure Data Lake Analytics baseia-se em uma combinação de Transact-SQL e C#. Da mesma forma, APIs com base em SQL estão disponíveis para Hive, HBase e Spark.
- **Maturidade da tecnologia**. Muitas das tecnologias usadas em Big Data estão em evolução. Embora tecnologias Hadoop centrais, como Hive e Pig, tenham se estabilizado, tecnologias emergentes, como Spark, apresentam grandes alterações e aprimoramentos a cada nova versão. Serviços gerenciados, como Azure Data Lake Analytics e Azure Data Factory, são relativamente jovens em comparação a outros serviços do Azure e provavelmente evoluirão ao longo do tempo.
- **Segurança**. Soluções de Big Data normalmente se baseiam em armazenar todos os dados estáticos em um data lake centralizado. Proteger o acesso a esses dados pode ser desafiador, especialmente quando os dados devem ser ingeridos e consumidos por vários aplicativos e plataformas.

### Práticas recomendadas

- **Aproveitar o paralelismo**. A maioria das tecnologias de processamento de Big Data distribui a carga de trabalho em várias unidades de processamento. Isso exige que os arquivos de dados estáticos sejam criados e armazenados em um formato divisível. Sistemas de arquivos distribuídos, como HDFS, podem otimizar o desempenho de leitura e gravação, e o processamento real é executado por vários nós de cluster em paralelo, o que reduz o tempo de trabalho geral.
- **Dados de partição**. O processamento em lotes geralmente ocorre em um agendamento recorrente , por exemplo, semanal ou mensal. Arquivos de dados de partição e estruturas de dados como tabelas, com base em períodos de temporais que correspondem à agenda de processamento. Isso simplifica a ingestão de dados e o agendamento de trabalho, além de tornar mais fácil solucionar problemas de falhas. Além disso, o particionamento de tabelas usadas em consultas Hive, U-SQL ou SQL pode melhorar significativamente o desempenho da consulta.
- **Aplicar semântica de esquema na leitura**. Usar um data lake permite combinar o armazenamento de arquivos em vários formatos, sejam estruturados, semiestruturados ou não estruturados. Use semântica de *esquema na leitura*, que projeta um esquema nos dados quando os dados estão sendo processados, não quando estão armazenados. Isso integra flexibilidade à solução e evita gargalos durante a ingestão de dados causados pela verificação de tipo e a validação de dados.
- **Processar dados no local**. Soluções de BI tradicionais geralmente usam um processo ETL (extração, transformação e carregamento) para mover dados para um data warehouse. Com maiores volumes de dados e uma maior variedade de formatos, soluções de Big Data geralmente usam variações de ETL, como TEL (transformação, extração e carregamento). Com essa abordagem, os dados são processados no armazenamento de dados distribuídos, transformando-os na estrutura necessária, antes de mover os dados transformados para um armazenamento de dados analíticos.
- **Equilibrar custos de tempo e utilização**. Para trabalhos de processamento em lotes, é importante considerar dois fatores: custo unitário de nós de computação e custo por minuto de usar esses nós para concluir o trabalho. Por exemplo, um trabalho em lotes pode levar oito horas com quatro nós de cluster. No entanto, pode ser que o trabalho use todos os quatro nós somente durante as primeiras duas horas, sendo apenas dois nós necessários depois disso. Nesse caso, executar todo o trabalho em dois nós aumentaria o tempo total do trabalho, mas não o duplicaria, de modo que o custo total seria menor. Em alguns cenários de negócios, um tempo de processamento mais longo pode ser preferível ao custo mais alto de usar recursos de cluster subutilizados.
- **Separar os recursos de cluster**. Ao implantar clusters HDInsight, você normalmente alcança um melhor desempenho provisionando recursos de cluster separados para cada tipo de carga de trabalho. Por exemplo, embora clusters do Spark incluam Hive, se você precisar executar amplo processamento com Hive e Spark, deverá considerar implantar clusters Spark e Hadoop dedicados separados. Da mesma forma, se você estiver usando HBase e Storm para processamento de fluxo de baixa latência e Hive para processamento em lotes, considere clusters separados para Storm, HBase e Hadoop.
- **Orquestrar a ingestão de dados**. Em alguns casos, aplicativos de negócios existentes podem gravar arquivos de dados para processamento em lote diretamente em contêineres do Azure Storage Blob, em que podem ser consumidos pelo HDInsight ou pelo Azure Data Lake Analytics. No entanto, você geralmente precisará orquestrar a ingestão de dados de fontes de dados externas ou locais para o data lake. Use um fluxo de trabalho de orquestração ou um pipeline, como aqueles compatíveis com Azure Data Factory ou Oozie, para fazer isso de maneira previsível e gerenciável centralmente.
- **Limpar dados confidenciais cedo**. O fluxo de trabalho de ingestão de dados deve remover dados confidenciais no início do processo para evitar armazená-los no data lake.

### Arquitetura do IoT

O IoT (Internet das Coisas) é um subconjunto especializado de soluções de big data. O diagrama a seguir mostra uma possível arquitetura lógica de IoT. O diagrama enfatiza os componentes da arquitetura do streaming de eventos.

O **gateway de nuvem** consome eventos de dispositivo no limite da nuvem, usando um sistema de mensagens de latência baixa e confiável.

Os dispositivos podem enviar eventos diretamente para o gateway de nuvem, ou por meio de um **gateway de campo**. Um gateway de campo é um software ou dispositivo especializado, geralmente colocado com dispositivos, que recebe eventos e os encaminha para o gateway de nuvem. O gateway de campo também pode pré-processar os eventos de dispositivo brutos executando funções, como filtragem, agregação ou transformação de protocolo.

Após a ingestão, os eventos passam por um ou mais **processadores de fluxo** que podem encaminhar os dados (por exemplo, para armazenamento) ou executar análise e outros tipos de processamento.

A seguir estão alguns tipos comuns de processamento. (Esta lista certamente não é exaustiva.)

- Gravando os dados de evento para armazenamento menos acessado, para arquivamento ou análise de processo em lote.
- Análise de caminho mais acessado, analisando o fluxo de eventos (quase) em tempo real, para detectar anomalias, reconhecer padrões em janelas de tempo ou disparar alertas quando ocorre uma condição específica no fluxo.
- Tratamento de tipos especiais de mensagens que não são de telemetria de dispositivos, como notificações e alarmes.
- Machine Learning.

As caixas destacadas em cinza mostram os componentes de um sistema de IoT que não estão diretamente relacionadas ao streaming de evento, mas são incluídos aqui para fins de integridade.

- O **registro do dispositivo** é um banco de dados dos dispositivos provisionados, incluindo os IDs de dispositivo e metadados do dispositivo, como localização.
- A **API de provisionamento** é uma interface externa comum para provisionar e registrar dispositivos novos.
- Algumas soluções IoT permitem que **mensagens de comando e controle** sejam enviadas aos dispositivos.

## **Azure Machine Learning?**

### O que é o Azure Machine Learning?

O Azure Machine Learning é um serviço de nuvem para acelerar e gerenciar o ciclo de vida dos projetos de machine learning. Profissionais de machine learning, cientistas de dados e engenheiros podem usá-lo em seus fluxos de trabalho cotidianos para: treinar e implantar modelos e gerenciar MLOps.

Você pode criar um modelo no Azure Machine Learning ou usar um modelo criado de uma plataforma de código aberto, como Pytorch, TensorFlow ou scikit-learn. As ferramentas do MLOps ajudam você a monitorar, treinar e reimplantar modelos.

O Azure Machine Learning é para indivíduos e equipes que implementam MLOps nas respectivas organizações para colocar modelos de machine learning em produção em um ambiente de produção seguro e auditável.

Os cientistas de dados e os engenheiros de ML encontrarão ferramentas para acelerar e automatizar seus fluxos de trabalho cotidianos. Os desenvolvedores de aplicativos encontrarão ferramentas para integrar modelos em aplicativos ou serviços. Os desenvolvedores de plataforma encontrarão um conjunto robusto de ferramentas, com suporte das APIs duráveis do Azure Resource Manager, para a criação de ferramentas avançadas de ML.

As empresas que trabalham na nuvem do Microsoft Azure encontrarão elementos familiares de segurança e RBAC (controle de acesso baseado em função) para infraestrutura. Você pode configurar um projeto para negar o acesso a dados protegidos e selecionar operações.

## Azure CLI (comandos)

Você faz criação e gestão dos produtos da azure por meio de linhas de comando.

### Comandos

[az | Microsoft Learn](https://learn.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest) 

### Instalar

[Como instalar a CLI do Azure | Microsoft Learn](https://learn.microsoft.com/pt-br/cli/azure/install-azure-cli) 

## Azure Virtual Machines

- Computador baseado em software
- São emulações de computadores físicos
- Contém: processador virtual, memória, armazenamento e recursos de rede
- Oferecem infra como serviço (IaaS)
- Se não estiver ustilizando, desliga a máquina e não será cobrado por ela
- Máquina virtual → guest & computador físico → host
- Downtimes (Tipos de indisponibilidades):
    - Planned Maintenance: Atualizações Microsoft (SO, Patchs e Drivers)
    - Unplanned Maintenance: Falhas detectadas pelo Health Check da Microsoft. Quando ocorre, a Microsoft busca mover as VMs para um outro hardware, quase invisível. Só é mais perceptível se esse movimento de VMs falhar (Unexpected Downtime)
    - Unexpected Downtime: Você pode se proteger pagando mais. A Microsoft implementa as proteções por meio dos Availability Sets (Protege contra falhas de hardware ao criar duas entidades, Fault Domains (Como se fossem Rack Servers) e Updated Domains (Como se fossem hosts físicos), dentro do Availability Set criado na Azure). Se implementar, vai precisar do **LOAD BALANCER** para direcionar uso para diferentes VMs. Implementar os **SCALE SETS** faz você conseguir diminuir ou aumentar quantidade de acordo com uso.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/f920b0b2-e9be-4b82-a495-bd60f8454c60/Untitled.png)

## Tamanho

Tamanho: [Visão geral dos tamanhos de máquinas virtuais - Azure Virtual Machines | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/virtual-machines/sizes/overview?tabs=breakdownseries%2Cgeneralsizelist%2Ccomputesizelist%2Cmemorysizelist%2Cstoragesizelist%2Cgpusizelist%2Cfpgasizelist%2Chpcsizelist) 

- Proprósito geral (máquinas de uso geral)
- Otimizada para computação (máquinas para processamento)
- Otimizada para memória (máquinas para memória)
- Otimizada para armazenamento (máquinas para armazenamento)
- GPU (circuito eletrônico capaz de realizar cálculos matemáticos em alta velocidade. Edição de vídeo e ****Machine learning utilizam GPU)
- Computador de alta performance

## Azure App Service

- Não administra infra
- Faz gestão do código

## Azure Storage

## Storage Account

[Visão geral da conta de armazenamento - Azure Storage | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-overview)

Uma conta de armazenamento da Azure terá todos os objetos de dados dos seus serviços de armazenamento (Storage Services abaixo). Fornece a separação e organização de diferentes armazenamentos. 

## Storage Services

- Blob - *Binary Large Object*. São os arquivos ou, como no nome, os objetos (arquivos imagem, arquivo de log, arquivo de vídeo, arquivo de texto, arquivos em geral). Esses objetos guardamos dentro de um container e aí consegue fazer o armazenamento de cada.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/4a519c99-ce0b-42c8-be81-66f28382b5c0/Untitled.png)

- Disk - Podemos ampliar essa quantidade de disco aumentando o Storage, a capacidade de armazenamento, principalmente na parte da VM.

[Escolha um tipo de disco para VMs IaaS do Azure – discos gerenciados - Azure Virtual Machines | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/virtual-machines/disks-types) 

[Anexação de um disco de dados a uma VM do Linux - Azure Virtual Machines | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/virtual-machines/linux/attach-disk-portal)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/2a48cb49-0a29-4d86-bd9c-3fe90513bd89/Untitled.png)

- File - Serviço de *file share.* Montamos um *file server share* com o servidor de compartilhamento e aí todas as nossas estações, todos os nossos serviços vão lá e buscam diretamente desse *share* (ponto de compartilhamento).
- Archive - Classe de armazenamento. Você vai precisar fazer um armazenamento de longo período para preservar os seus dados, entra essa questão do *archive* que no final das contas é colocar o seu objeto lá no Storage.

## Redundância

https://learn.microsoft.com/pt-br/azure/storage/common/storage-redundancy#zone-redundant-storage

O Armazenamento do Azure sempre armazena várias cópias dos seus dados para protegê-los contra eventos planejados e não planejados. A redundância garante que sua conta de armazenamento atenda às suas metas de disponibilidade e durabilidade mesmo diante de falhas.

### **Fatores que ajudam a determinar qual opção de redundância você deve escolher:**

1. Como os dados são replicados dentro da região primária
2. Se os dados são ou não replicados para uma segunda região que está geograficamente distante da região primária, como proteção contra desastres regionais (replicação geográfica).
3. Se o aplicativo requer acesso de leitura aos dados replicados na região secundária quando a região primária ficar não disponível por algum motivo (replicação geográfica com acesso de leitura).

### **Redundância na região primária**

O Armazenamento do Azure oferece duas opções de como os dados são replicados na região primária:

- O **armazenamento com redundância local (LRS)** copia seus dados de forma síncrona ***três vezes em um único local físico*** na região primária. O LRS é a opção de replicação **menos dispendiosa**, mas **não é recomendada para aplicativos que exigem alta disponibilidade ou durabilidade**.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/8824153e-d486-40f7-94fc-5e402c7f6163/Untitled.png)

<aside>
💡 **O LRS é uma boa opção para os seguintes cenários:**

Seu aplicativo armazena dados que possam ser facilmente reconstruídos.

Seu aplicativo está restrito a replicar dados somente em uma região. Em alguns casos, as regiões emparelhadas nas quais os dados são replicados geograficamente podem estar dentro de outra região. Para mais informações sobre pares de regiões, consulte Regiões do Azure.

Seu cenário estiver usando discos não gerenciados do Azure. É possível criar uma conta de armazenamento para discos não gerenciados do Azure que usam GRS, mas isso não é recomendável devido a possíveis problemas de consistência em relação à replicação geográfica assíncrona.

</aside>

- O **Armazenamento com redundância de zona (ZRS)** copia seus dados de forma síncrona em ***três zonas de disponibilidade do Azure na região primária***. Para **aplicativos que exigem alta disponibilidade**, a Microsoft recomenda **usar o ZRS na região primária e também replicar para uma região secundária**.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/fb5650fe-6b9b-4141-ad1c-4d570b5a273b/Untitled.png)

<aside>
💡 O ZRS fornece desempenho excelente, baixa latência e resiliência para seus dados se eles ficarem temporariamente indisponíveis. No entanto, o ZRS, por si só, pode não proteger totalmente seus dados contra um desastre regional em que várias zonas são permanentemente afetadas. O [GZRS (armazenamento com redundância de zona geográfica)](https://learn.microsoft.com/pt-br/azure/storage/common/storage-redundancy#geo-zone-redundant-storage) usa o ZRS na região primária e também replica geograficamente seus dados para uma região secundária. O GZRS está disponível em muitas regiões e é recomendado para proteção contra desastres regionais.

</aside>

### **Redundância em uma região secundária**

As opções de redundância podem ajudar a fornecer **alta durabilidade para seus aplicativos**. Copiar sua conta de armazenamento para uma região secundária garante que seus **dados permaneçam duráveis** durante uma interrupção regional completa ou um desastre no qual a região primária não é recuperável.

Quando você cria uma conta de armazenamento, **pode selecionar a região primária** para a conta. A **região secundária** emparelhada é **determinada com base na região primária** e **não pode ser alterada**. 

O Armazenamento do Azure oferece duas opções de como os dados são replicados na região primária:

- O **armazenamento com redundância geográfica (GRS)** copia seus dados de forma síncrona ***três vezes em um único local físico na região primária usando o LRS***. Em seguida, ele copia os dados de forma assíncrona para um único local físico na região secundária. ***Na região secundária, seus dados são copiados de forma síncrona três vezes usando o LRS***.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/c209acd5-c25e-4ae3-91e4-8665753a2a77/Untitled.png)

<aside>
💡 O GRS oferece durabilidade para recursos de armazenamento de, pelo menos, 99,99999999999999% (dezesseis noves) ao ano.

</aside>

- O **armazenamento com redundância de zona geográfica (GZRS)** copia seus dados de forma síncrona em ***três zonas de disponibilidade do Azure na região primária usando o ZRS.*** Em seguida, ele copia os dados de forma assíncrona para um único local físico na região secundária. ***Na região secundária, seus dados são copiados de forma síncrona três vezes usando o LRS.***

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/b2f65284-b4eb-488a-8be5-537a66e17eae/Untitled.png)

<aside>
💡 O GZRS é projetado para fornecer durabilidade de, pelo menos, 99,99999999999999 % (dezesseis noves) dos objetos em determinado ano.

</aside>

## **Parâmetros de durabilidade e disponibilidade**

| Parâmetro | LRS | ZRS | GRS/RA-GRS | GZRS/RA-GZRS |
| --- | --- | --- | --- | --- |
| Porcentagem de durabilidade dos objetos em um determinado ano | pelo menos 99,999999999% (onze noves) | pelo menos 99,9999999999% (doze noves) | pelo menos 99,99999999999999% (dezesseis noves) | pelo menos 99,99999999999999% (dezesseis noves) |
| Disponibilidade para solicitações de leitura | Pelo menos 99,9% (99% para camadas de armazenamento de arquivos/frio/esporádico) | Pelo menos 99,9% (99% para a camada de armazenamento/frio/esporádico) | Pelo menos 99,9% (99% para camadas de armazenamento de arquivos/frio/esporádico) para GRSPelo menos 99,99% (99,9% para camadas de armazenamento de arquivos/frio/esporádico) para RA-GRS | Pelo menos 99,9% (99% para a camada de acesso esporádico/frio) para o GZRSPelo menos 99,99% (99.9% para a camada de acesso esporádico/frio) para o RA-GZRS |
| Disponibilidade para solicitações de gravação | Pelo menos 99,9% (99% para camadas de armazenamento de arquivos/frio/esporádico) | Pelo menos 99,9% (99% para a camada de armazenamento/frio/esporádico) | Pelo menos 99,9% (99% para camadas de armazenamento de arquivos/frio/esporádico) | Pelo menos 99,9% (99% para a camada de armazenamento/frio/esporádico) |
| Número de cópias de dados mantidos em nós separados | Três cópias em uma única região | Três cópias em zonas de disponibilidade separadas em uma única região | Total de seis cópias, incluindo três na região primária, e três na região secundária | Total de seis cópias, incluindo três em zonas de disponibilidade separadas na região primária, e três cópias com redundância local na região secundária |

## **Cenário de durabilidade e disponibilidade durante interrupções**

| Cenário de interrupção | LRS | ZRS | GRS/RA-GRS | GZRS/RA-GZRS |
| --- | --- | --- | --- | --- |
| Um nó dentro de um data center se torna indisponível | Sim | Sim | Sim | Yes |
| Um data center inteiro (zonal ou não zonal) fica indisponível | Não | Sim | Sim1 | Sim |
| Uma interrupção ocorre em toda a região primária | Não | Não | Sim1 | Sim1 |
| O acesso de leitura na região secundária estará disponível se a região primária ficar indisponível | Não | Não | Sim (com RA-GRS) | Sim (com RA-GZRS) |

## **Serviços de Armazenamento do Azure com suporte**

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/027e95e9-d949-409a-be06-908c18f29c16/Untitled.png)

## Tipos de conta de armazenamento suportados

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/1752dae2-50dd-4350-92bb-08b7c9b230dd/Untitled.png)

## Access Tiers

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/6214944c-0480-41a4-a29d-bc86470a805a/Untitled.png)

## Azure Databases

- Cosmos DB - Banco de dados NoSQL totalmente gerenciável, considerado um PaaS. É multi região, independente e faz redundância transparente dos dados em várias regiões.
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/8979f76c-0eca-4d97-9f71-c9388b599f9d/Untitled.png)
    
- Azure SQL - uma família (***Azure SQL Database, Azure SQL Managed Instance (ocorre em instância e é autogerenciada), SQL Server on Azure VMs (ocorre em instância, mas não é autogerenciada)***) que gerencia, traz segurança e possui produtos inteligentes.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/a022f281-e91e-45ba-b8ba-e50e6b201712/Untitled.png)

- MySQL
- PostgreSQL
    
    ### **O Banco de Dados do Azure para PostgreSQL**
    
    O que é o Banco de Dados do Azure para PostgreSQL?
    
    O Banco de Dados do Azure para PostgreSQL é um serviço de banco de dados relacional no Microsoft Cloud com base no mecanismo de banco de dados [PostgreSQL Community Edition](https://www.postgresql.org/) (disponível sob a licença GPLv2). O Banco de Dados do Azure para PostgreSQL fornece:
    
    - Alta disponibilidade interna.
    - Proteção de dados usando backups automáticos e restauração pontual por até 35 dias.
    - Manutenção automatizada para hardware, sistema operacional e mecanismo de banco de dados subjacentes para manter o serviço seguro e atualizado.
    - Desempenho previsível, com preços pré-pagos inclusivos.
    - Dimensionamento elástico em segundos.
    - Segurança de nível corporativo e conformidade líder do setor para proteger dados confidenciais em repouso e em movimento.
    - Monitoramento e automação para simplificar o gerenciamento e o monitoramento para implantações em larga escala.
    - Experiência de suporte líder do setor.
    
    Esses recursos não precisam de quase nenhuma administração e todos são fornecidos sem nenhum custo adicional. Eles permitem que você se concentre no método RAD e em acelerar seu tempo de colocação no mercado, em vez de alocar tempo e recursos preciosos ao gerenciamento de máquinas virtuais e de infraestrutura. Além disso, você pode continuar desenvolvendo seu aplicativo com a plataforma e as ferramentas de software livre de sua escolha e pode fornecê-lo com a velocidade e a eficiência que sua empresa exige, tudo isso sem precisar aprender novas habilidades.
    
    ### Modelos de implantação
    
    O Banco de Dados do Azure para PostgreSQL desenvolvido com o PostgreSQL community edition está disponível em três modos de implantação:
    
    - Servidor único
    - Servidor Flexível (versão prévia)
    - Hiperescala (Citus)
- Database Migration Service - Serviço totalmente gerenciável com o objetivo de fazer migração de múltiplos databases para a plataforma da Azure com o menor tempo possível de indisponibilidade (online migrations). Existe o Data Migration Assistant (DMA) que ajuda na migração dos seus dados (migrar seu DB On Premise para a Nuvem da Azure) e o Database Migration Service (DMS) que pode migrar também servidores (infraestrutura).

## Azure Solutions

- IoT - Plataforma SaaS com proposta da Azure para controlar vários serviços IoT em um mesmo local. Existe a IoT Central para fazer todo esse gerenciamento, fornecendo uma interface de usuário e ferramentas para a visualização e análise de dados dos dispositivos conectados. Existe o Hub IoT que recolhe todos os dados e pode enviar dados também, conectando e gerenciando dispositivos IoT. IoT Central usa o IoT Hub para comunicação real com os dispositivos. Quando você cria um aplicativo no IoT Central, ele configura um IoT Hub subjacente automaticamente para gerenciar os dispositivos e as comunicações. ([What is Azure IoT Central - Azure IoT Central | Microsoft Learn](https://learn.microsoft.com/en-us/azure/iot-central/core/overview-iot-central))
    
    *(não precisa decorar os serviços)*
    

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/44ba5556-94c3-40c7-99f2-d1b45c64b643/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/2a9e6d53-eb58-4a78-a4d8-b92219969af3/Untitled.png)

### **A Internet das Coisas (IoT) do Azure**

### O que é a Internet das Coisas (IoT) do Azure?

A Internet das Coisas (IoT) do Azure é uma coleção de serviços cloud geridos pela Microsoft que ligam, monitorizam e controlam milhares de milhões de recursos de IoT. Em termos mais simples, uma solução IoT é composta por um ou mais dispositivos IoT que comunicam com um ou mais serviços de back-end alojados na cloud.

### Dispositivos IoT

Um dispositivo IoT é normalmente composto por uma placa de circuito com sensores ligados que usam Wi-Fi para se ligar à internet. Por exemplo:

- Um sensor de pressão numa bomba de óleo remota.
- Sensores de temperatura e humidade numa unidade de ar condicionado.
- Um acelerómetro num elevador.
- Sensores de presença numa sala.

Há uma grande variedade de dispositivos disponíveis de diferentes fabricantes para construir a sua solução. Para obter uma lista de dispositivos certificados para trabalhar com o Azure IoT Hub, consulte o [catálogo de dispositivos Azure Certified for IoT](https://devicecatalog.azure.com/). Para prototipagem, pode utilizar dispositivos como um [MXChip IoT DevKit](https://microsoft.github.io/azure-iot-developer-kit/) ou um [Raspberry Pi](https://www.raspberrypi.org/). O Devkit tem sensores incorporados para temperatura, pressão, humidade e um giroscópio, acelerómetro e magnetómetro. O Raspberry Pi permite-lhe anexar vários tipos diferentes de sensores.

A Microsoft fornece [SDKs](https://docs.microsoft.com/pt-pt/azure/iot-hub/iot-hub-devguide-sdks) de dispositivo de código aberto que pode usar para construir as aplicações que executam nos seus dispositivos. Estes [SDKs simplificam e aceleram](https://azure.microsoft.com/blog/benefits-of-using-the-azure-iot-sdks-in-your-azure-iot-solution/) o desenvolvimento das suas soluções IoT.

### Comunicação

Normalmente, os dispositivos IoT enviam telemetria dos sensores para serviços de back-end na nuvem. No entanto, outros tipos de comunicação são possíveis, como um serviço de back-end enviando comandos para os seus dispositivos. Seguem-se alguns exemplos de comunicação dispositivo-a-nuvem e nuvem-para-dispositivo:

- Um caminhão de refrigeração móvel envia temperatura a cada 5 minutos para um hub IoT.
- O serviço back-end envia um comando a um dispositivo para alterar a frequência a que envia telemetria para ajudar a diagnosticar um problema.
- Um dispositivo envia alertas com base nos valores lidos nos seus sensores. Por exemplo, um dispositivo que monitoriza um reator de lote numa instalação química, envia um alerta quando a temperatura excede um determinado valor.
- Os seus dispositivos enviam informações para visualização num painel de instrumentos para visualização por operadores humanos. Por exemplo, uma sala de controlo numa refinaria pode mostrar os volumes de temperatura, pressão e fluxo em cada tubo, permitindo aos operadores monitorizar a instalação.

Os [SDKs de Dispositivo IoT](https://docs.microsoft.com/pt-pt/azure/iot-hub/iot-hub-devguide-sdks) e o IoT Hub suportam protocolos de [comunicação comuns](https://docs.microsoft.com/pt-pt/azure/iot-hub/iot-hub-devguide-protocols) como HTTP, MQTT e AMQP.

Os dispositivos IoT têm características diferentes quando comparados com outros clientes, como navegadores e aplicações móveis. Os SDKs do dispositivo ajudam-no a enfrentar os desafios da ligação dos dispositivos de forma segura e fiável ao seu serviço back-end. Especificamente, os dispositivos IoT:

- São, frequentemente, sistemas incorporados sem nenhum operador humano (ao contrário de um telefone).
- Podem ser implementados em localizações remotas, onde o acesso físico é dispendioso.
- Podem apenas ser acessíveis através do back-end da solução.
- Podem recursos de processamento e um poder limitados.
- Podem ter uma conectividade de rede intermitente, lente ou dispendiosa.
- Podem ter de utilizar protocolos de aplicação proprietários, personalizados ou específicos da indústria.

### Serviços back-end

Numa solução IoT, o serviço back-end fornece funcionalidades como:

- Receber telemetria à escala dos seus dispositivos e determinar como processar e armazenar esses dados.
- Analisar a telemetria para fornecer insights, em tempo real ou após o facto.
- Envio de comandos da nuvem para um dispositivo específico.
- A provisionar dispositivos e a controlar quais os dispositivos que podem ligar à sua infraestrutura.
- Controlando o estado dos seus dispositivos e monitorizando as suas atividades.
- Gerir o firmware instalado nos seus dispositivos.

Por exemplo, numa solução de monitorização remota para uma estação de bombagem de óleo, a parte traseira da nuvem utiliza telemetria das bombas para identificar comportamentos anómalos. Quando o serviço de back-end identificar uma anomalia, pode enviar automaticamente um comando de volta ao dispositivo para tomar uma ação corretiva. Este processo gera um ciclo de comentários automatizado entre o dispositivo e a cloud, que aumenta significativamente a eficiência da solução.

- Big Data - Azure Data Lake Analytics é uma arquitetura de big data que lida com recolhimento, processamento e análise de dados que são muito complexos ou volumosos para serem lidados em sistemas databases tradicionais. *Escreve-se **queries** para transformar dados em informações*. Machine Learning é um serviço que auxilia desenvolvedores e cientistas de dados. Alguns serviços: MLOps (Machine Learning Operations com modelos para serem treinados), Cognitive Services (Com templates pré-treinados para serem utilizados) e Bot Services.
- DevOps - Alguns serviços: Azure Boards, Azure Pipelines, Azure Repos, Azure Test Plans e Azure Artifacts. [Azure DevOps Services | Microsoft Azure](https://azure.microsoft.com/en-us/products/devops/)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/6fc4cc73-aa41-4134-b452-c3b85aa95ea7/Untitled.png)

## Azure Security

### Azure Firewall

https://learn.microsoft.com/pt-br/azure/firewall/features

[Visão geral da arquitetura do Firewall do Azure Network Virtual Appliances - Azure Architecture Center | Microsoft Learn](https://learn.microsoft.com/pt-br/azure/architecture/networking/guide/network-virtual-appliances-architecture)

Fez as configurações, no lugar de você colocar no *rack*, você está usando Azure para cuidar desse ambiente, ganha o Firewall como serviço, como serviço dentro da Azure ele vai permitir não só proteger o acesso às informações internas dentro das tuas redes, as *VNets*.

As máquinas que estão rodando ali dentro banco de dados e todos os serviços da Azure, como também você consegue utilizá-lo para segregar todo tráfego que vai chegar no teu *On-premises*.

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/6c72abbb-bae1-4383-9959-811558295777/image.png)

O ambiente externo, o meu *On-premises*, o ambiente das linhas de *VNet*, essa ideia, é importante conceitualmente até do ponto de vista de aplicabilidade, que esse Firewall pode segregar os ambiente Azure e também o acesso *On-premise*. Conforme está descrito, Firewall nada, mas que, similar ao Firewall de rede que você colocaria no teu datacenter.

### Recursos:

1. Alta disponibilidade interna 
2. Zonas de Disponibilidades
3. Escalabilidade de nuvem sem restrições
4. Regras de filtragem de FQDN de aplicativo
5. Regras de filtragem de tráfego de rede
6. Marcas de FQDN
7. Marcas de serviço
8. Inteligência contra ameaças
9. Proxy DNS
10. DNS Personalizado
11. Regras do FQDN na rede
12. Implantação sem endereço IP público no modo de túnel forçado
13. Suporte a SNAT de saída
14. Suporte a DNAT de entrada
15. Vários endereços IP públicos
16. Registro em log do Azure Monitor
17. Túnel forçado
18. Categorias da Web
19. Certificações

### Network Security Groups (NSG)

O NSG é como um Firewall interno. Esse Firewall interno está atrelado diretamente ao teu recurso. Quando se cria uma máquina virtual, consegue criar NSG e, com ele, granular o acesso em termos de IP, porta e protocolo, isso é importante, para esse recurso. Eu posso granular e nessa mesma rede eu tenho outras máquinas que não têm essa restrição de acesso.

Então, NSG combinado com Firewall são complementares, por isso é importante ter em mente aquele conceito de defesa em profundidade, são camadas diferentes. Eu posso ter um Firewall segregando minha rede, lá dentro da minha rede tenho um NSG para filtrar o que chega na minha máquina virtual.

o ***Azure Firewall*** ele é um serviço *stateful* - controle total do estado da conexão, o detalhe que ele vai fornecer a segurança para a ***camada de rede e a camada de aplicação***. Proteção para rede e para a aplicação, diferentes assinaturas ou subscritos que temos da Azure e da VNet, o nosso ***NSG*** vai fazer a filtragem na ***camada de rede***, limitando tráfego e acesso a recursos que temos lá dentro.

### Azure DDoS Protection

Essa mitigação de ataque DDoS partindo na visão da Azure, tem a Azure *backbone*, como o meu acesso acontece por diversos pontos diferentes, você tem de imaginar o porte desse *backbone* o porte dessa rede, ele é muito mais forte, muito mais poderoso.

Quando um ataque chegar, ainda que passe alguma coisa desse ataque e caia lá no teu servidor, ele tem uma estrutura muito mais robusta para impedir esse atacante, a pessoa para derrubar uma Azure, uma AWS, um Google, qualquer provedor tem que ser algo de volume estratosférico.

Vai conseguir fazer e além de questão de banda e tudo mais, tem uma série de inteligência aplicada que faz com que esses ataques sejam neutralizados em grande parte, sejam mitigados.

Existem duas versões para esse serviço: o **serviço *Basic*** e o **serviço *Standard***, o básico já está embutido não precisa fazer absolutamente nada.

Eu coloquei uma máquina virtual, eu já desfruto do recurso básico, já estou usando a infraestrutura da Azure, a infraestrutura global para proteger, mitigar esse acesso. Se eu precisar ir um passo além, onde eu preciso monitorar, analisar, ver com detalhes o que está acontecendo, então, sim, contrato um plano que chama *standard*. 

Para implementar isso na minha infraestrutura, para proteger VM, recursos em geral, banco de dados, não importa qual o recurso, a questão da proteção DDoS é aplicável ao cenário em geral da Azure.

Então, nome do serviço, DDoS *protection*, divide no básico e *standard*, para mostrar duas fatos legais ([link](https://docs.microsoft.com/pt-br/azure/ddos-protection/ddos-protection-overview)).

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/97a978c5-f67e-42ac-a6c7-f46a3fb69cda/image.png)

### Azure Security Center

Central de segurança, onde consegue ter um *dashboard* mapeando alguns pontos importantes do ambiente de segurança. Ele vai gerar relatório, fazer acompanhamento, indicando inclusive correções.

### **Microsoft Defender para Nuvem**

### O que é o Microsoft Defender para Nuvem?

https://docs.microsoft.com/pt-br/azure/security-center/azure-defender 

O Defender para Nuvem é uma ferramenta para gerenciamento de postura de segurança e proteção contra ameaças. Ele fortalece a postura de segurança dos seus recursos de nuvem, e, com seus planos integrados do Microsoft Defender, o Defender para Nuvem protege as cargas de trabalho em execução no Azure, *em* *ambiente híbrido e em outras plataformas de nuvem*.

O Defender para Nuvem fornece as ferramentas necessárias para proteger seus recursos, acompanhar sua postura de segurança, proteger contra ataques cibernéticos e simplificar o gerenciamento de segurança. Como é nativamente integrado, a implantação do Defender para Nuvem é fácil, fornecendo *provisionamento automático simples para proteger seus recursos por padrão*.

O Defender para Nuvem preenche três necessidades vitais à medida que você gerencia a segurança de seus recursos e cargas de trabalho locais e na nuvem:

!https://img-c.udemycdn.com/redactor/raw/article_lecture/2023-08-01_08-35-14-d6a040c2ddcdad5ea112d9e964bc548c.png

Diretamente na tua máquina, no teu banco de dados, no teu *container* aplicações web. Qual é a proposta? Que ele fique lá dentro verificando se tem alguma vulnerabilidade, alguma falta de *pet*, bug, alguma coisa conhecida.

Ele vai alertar, vai notificar para que você possa fazer todas as medidas preventivas e as correções dos problemas ([link](https://docs.microsoft.com/pt-br/azure/security-center/azure-defender)).

### Azure Key Vault

Cofre digital. Para você armazenar uma senha, uma chave, eu posso gerar uma chave SSH e armazená-la - armazenar certificados, a proposta exatamente: tem um cofre digital para armazenar essas questões sensíveis do ponto de vista de segurança e tem integrações com os recursos.

Você pode ter a tua aplicação que vai lá no *key vault*, pega, tem acesso à chave para validar algum recurso. Existem dois tipos de serviço que é o ***standard*** e o ***premium***.

O *standard* é o cofre digital - um serviço via software e tudo mais, e tem a versão de hardware como chama o *HSM* que é um **módulo físico** para fazer essa proteção, tem toda a questão de conformidade, de não violação, tem toda uma temática sobre HSM e é construído exatamente para que você possa proteger tua informação.

Você tem essas duas opções, usar via software ou usar via hardware.

### **Microsoft Sentinel**

### O que é o Microsoft Sentinel?

O Microsoft Sentinel é uma solução escalonável e nativa de nuvem que oferece **SIEM (gerenciamento de eventos de informações de segurança)** e **SOAR (resposta automatizada para orquestração de segurança)** . O Microsoft Sentinel oferece análise inteligente de segurança e inteligência contra ameaças em toda a empresa, com uma solução para detecção de alertas, visibilidade de ameaças, procura proativa e resposta a ameaças.

O Microsoft Sentinel é sua visão geral da empresa, amenizando o estresse de ataques cada vez mais sofisticados, volumes crescentes de alertas e longos períodos para resolução.

- **Colete dados na escala de nuvem** de todos os usuários, dispositivos, aplicativos e infraestrutura, local e em múltiplas nuvens.
- **Detecte ameaças que ainda não foram descobertas** e [minimize falsos positivos](https://docs.microsoft.com/pt-br/azure/sentinel/false-positives) usando a análise e a inteligência contra ameaças incomparáveis da Microsoft.
- **Investigue ameaças com inteligência artificial** e busque por atividades suspeitas em escala, acessando anos de trabalho sobre segurança cibernética na Microsoft.
- **Responda a incidentes de forma rápida** com orquestração interna e automação de tarefas comuns.

Aproveitando a gama completa de serviços existentes do Azure, o Microsoft Sentinel incorpora nativamente bases comprovadas, como o Log Analytics e os Aplicativos Lógicos. O Microsoft Sentinel enriquece a investigação e a detecção com IA, além de oferecer o fluxo de inteligência da Microsoft contra ameaças e permitir que você use sua própria inteligência contra ameaças.

## Identity Services / Compliance

https://learn.microsoft.com/pt-br/azure/active-directory/fundamentals/compare

A Microsoft introduziu Active Directory Domain Services no Windows 2000 para dar às organizações a capacidade de gerir múltiplos componentes e sistemas de infraestrutura no local com uma única identidade por utilizador.

Microsoft Entra ID leva esta abordagem para o nível seguinte ao fornecer às organizações uma solução de Identidade como Serviço (IDaaS) para todas as suas aplicações na cloud e no local.

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/b57ad4a4-41d8-40dc-9bda-5fe9d0d00db6/image.png)

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/11bc71a8-3e4a-4e9b-a60b-fcab9d6ad7e6/image.png)

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/df2cf52b-6f43-4918-b6ab-934fa4d15761/image.png)

### Single Sign-On (SSO)

https://learn.microsoft.com/pt-br/entra/identity/enterprise-apps/plan-sso-deployment

Ao planejar sua implantação de SSO com seus aplicativos no Microsoft Entra ID, você precisa considerar as seguintes questões:

- Quais são as funções administrativas necessárias para gerenciar o aplicativo?
- O certificado do aplicativo Security Assertion Markup Language (SAML) precisa ser renovado?
- Quem precisa ser notificado sobre as alterações relacionadas à implementação do SSO?
- Quais licenças são necessárias para garantir o gerenciamento efetivo do aplicativo?
- As contas de usuário compartilhadas e de convidados são usadas para acessar o aplicativo?
- Entendo as opções de implantação de SSO?

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/9a3c9b83-8cad-46d7-b96f-29e6e5f0def8/c66c07ac-2c2e-44b7-b47b-2756a5692855/image.png)

### Azure AD MFA

Eu posso exigir do meu usuário do AAD que ele use o segundo fator de autenticação, isso é legal porque para que reforce muito a minha segurança.

### Azure Policy e Roles

Cada pessoa pode ter um cargo com permissões específicas. 

### Azure Monitor

Vários recursos, mas, por exemplo, uma VM consegue ver memória, processamento, disco, você tem em real time um detalhamento bem interessante do que está acontecendo e a partir disso pode tomar várias ações, alertas, traçar e monitorar.

**Exemplos**, o que o serviço é capaz de fazer. Detectar e diagnosticar problemas de aplicativos e dependências, analisar monitoramento do log *Analytics*. Para você fazer um diagnóstico mais profundo, dá suporte as operações de escala, você vai ver que quando ativa esse recurso, começa a olhar detalhes que muitas vezes, passa desapercebido. Criar visualizações dentro do *dashboard*, coletar dados de monitoração dos recursos utilizados pelo *monitor metrics.* 

Conceitualmente, é ferramenta onde você vai concentrar as informações, vai poder olhar essas informações do que está acontecendo e tomar algumas ações em cima disso.

Pode customizar e criar métricas.

### Service Health

Eles disponibilizam serviço que é o *Service Health* e eu deixei até sublinhado ele é 0800, ele não tem custo, é um serviço para você acompanhar o que está acontecendo lá na Azure.

No *Health service*, se no momento está acontecendo alguma coisa e ele está pegando as minhas inscrições, eu tenho duas regiões, posso botar todas, não tem nada acontecendo no momento, serviço tem todos.

Deixa criar alertas. 

## **Dicas do Exame**

### **PaaS vs IaaS**

Se você precisar migrar para o azure usando apenas ofertas de plataforma como serviço, você não deve usar as máquinas virtuais do Azure porque as máquinas virtuais do **Azure são ofertas IaaS, porque você está alugando hardware ao invés de comprar.**

https://azure.microsoft.com/en-us/overview/what-is-paas/

https://azure.microsoft.com/en-us/overview/what-is-iaas/

Os bancos de dados SQL do Azure são ofertas de PaaS. Ao usar bancos de dados SQL do Azure, o Azure gerencia a maioria das funções de DBA, como patch, backups e monitoramento.

Os bancos de dados SQL do Azure estão sempre em execução na versão estável mais recente inclusive com aplicação de patches do SQL Server com disponibilidade de 99,99%.

Uma solução PaaS não fornece acesso ao sistema operacional. O serviço Aplicativos Web do Azure fornece um ambiente para você hospedar seus aplicativos web. No backend, os aplicativos da web são hospedados em máquinas virtuais, entanto, você não tem acesso direto à máquina virtual ou ao sistema operacional.

### **Software as a Service**

Ao implementar uma solução de Software como Serviço (SaaS), você é responsável por configurar a solução SaaS. Todo o resto é gerenciado pelo provedor de nuvem.

O **SaaS requer o mínimo de gerenciamento.** O provedor de nuvem é responsável por gerenciar tudo, e o usuário final apenas usa o software. O software como serviço (SaaS) permite que os usuários se conectem e usem aplicativos baseados em nuvem pela Internet. Exemplos comuns são e-mail, calendário e ferramentas de escritório (como o Microsoft Office 365).

O SaaS fornece uma solução de software completa que você adquire no modelo Pay-as-you-Go de um provedor de serviços em nuvem. Você aluga o uso de um aplicativo para sua organização e seus usuários se conectam a ele pela Internet, geralmente com um navegador da web ou um app.

Toda a infraestrutura subjacente, middleware, software de aplicativo e dados de aplicativo estão localizados no data center do provedor de serviços. O provedor de serviços gerencia o hardware e o software e, com o contrato de serviço adequado, garante a disponibilidade e a segurança do aplicativo e também dos seus dados.

Com o cloud, você basicamente migra para um modelo **pay-as-you-go**, ou seja,  paga apenas pelo que usar, sem custos de CapEx. Por outro lado, você tem gerenciamento de autoatendimento. Você é responsável pela implantação e configuração dos recursos de cloud, como máquinas virtuais ou sites. O hardware subjacente que hospeda os recursos de nuvem é gerenciado pelo provedor de cloud.

Ao planejar a migração de um site para o Azure, você deve planejar o pagamento dos custos mensais de uso. Isso ocorre porque o Azure usa o modelo pay-as-you-go (**metered pricing**)

### **Elastic Computing**

**Elastic Computing** é a capacidade de expandir ou diminuir rapidamente os recursos de processamento, memória e armazenamento do computador para atender às demandas em constante mudança, sem se preocupar com o planejamento de capacidade e engenharia para uso de pico.

Normalmente controlada por ferramentas de monitoramento do sistema, **elastic computing** combina a quantidade de recursos alocados com a quantidade de recursos realmente necessários, sem interromper as operações. Com a elasticidade da nuvem, uma empresa evita pagar por capacidade não utilizada ou recursos ociosos e não precisa se preocupar em investir na compra ou manutenção de recursos e equipamentos adicionais.

### **Azure Site Recovery**

A recuperação de site do Azure ajuda a garantir a continuidade dos negócios, mantendo bussines applications e workloads em execução mesmo durante interrupções.

Azure site recovery quando aplicado em máquinas virtuais, replica workloads em execução de um site primário para um local secundário. Portanto, apesar do nome, o objetivo principal é **a tolerância a falhas.**

A **tolerância a falhas** é a capacidade de um sistema de continuar a funcionar no caso de falha de algum de seus componentes. As zonas de disponibilidade expandem o nível de controle que você tem para manter a disponibilidade dos aplicativos e dados em suas VMs.

**Zonas de disponibilidade** são locais físicos exclusivos em uma região do Azure. **Cada zona é composta por um ou mais data centers equipados com energia, refrigeração e rede independentes.**

Para garantir resiliência, **há um mínimo de três zonas separadas em todas as regiões habilitadas**. A separação física das zonas de disponibilidade dentro de uma região protege aplicativos e dados de falhas do data center.

Com as zonas de disponibilidade, o Azure oferece 99,99%  de disponibilidade. Ao arquitetar suas soluções para usar VMs replicadas em zonas, você pode proteger seus aplicativos e dados contra a perda de um data center. **Se uma zona for comprometida, os aplicativos e dados replicados estarão disponíveis instantaneamente em outra zona.**

### Conceitos de Cloud

```
-> Alta disponibilidade
-> Escalabilidade
-> Agilidade
-> Distribuição Geográfica
-> Recuperação de desastres
-> Resource Pooling (Usuários não acessam recursos de outros clientes)
```

### **Modelos de Cloud**

#### Quais são os diferentes tipos de serviços de computação em nuvem?

Os **tipos de computação em nuvem são modelos de implantação de serviço que permitem a seleção do nível de controle sobre as informações e tipos de serviço** que precisam ser fornecidos. Há **três tipos principais** de serviços de computação em nuvem, às vezes chamados de pilha de computação em nuvem, pois são compilados um sobre o outro.

O primeiro tipo de computação em nuvem é a [infraestrutura como serviço (IaaS)](https://azure.microsoft.com/pt-br/overview/what-is-iaas/), usada para acesso à recursos de computação e armazenamento baseados na Internet. Sendo a categoria mais básica entre os tipos de computação em nuvem, a IaaS permite que você alugue uma infraestrutura de TI (servidores e máquinas virtuais, armazenamento, redes e sistemas operacionais) de um provedor de nuvem em uma base paga conforme o uso.

O segundo tipo de computação em nuvem é a [plataforma como serviço (PaaS)](https://azure.microsoft.com/pt-br/overview/what-is-paas/), que dá aos desenvolvedores as ferramentas necessárias para criar e hospedar aplicativos Web. A PaaS foi desenvolvida para proporcionar aos usuários o acesso aos componentes necessários para desenvolver e operar rapidamente aplicativos Web ou móveis na Internet, sem se preocupar com a configuração ou gerenciamento da infraestrutura subjacente dos servidores, armazenamento, redes e bancos de dados.

##### Principais serviços:

```
- CDN
- Cosmos DB
- Azure SQL Databases
- Azure Database for MySQL
- Storage
- Synapse Analytics
```
##### Outros Frameworks:
```
- ASP.NET
- .NET
- Java
- Node.js
- PHP
- Python
```

O terceiro tipo de computação em nuvem é o [software como serviço (SaaS)](https://azure.microsoft.com/pt-br/overview/what-is-saas/), usado para aplicativos baseados na Web. O SaaS é um método de entrega de aplicativos de software na Internet, no qual os provedores de nuvem hospedam e gerenciam os aplicativos de software, fazendo com que seja simples ter o mesmo aplicativo em todos seus dispositivos de uma só vez por meio da nuvem. Ex.: OneDrive, Xbox Live e Microsoft 365.

A Azure é excelente nos 3 tipos.
