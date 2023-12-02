# Compare orquestradores de contêineres Apache Mesos vs. Kubernetes

### O que é Apache Mesos?
Apache Mesos é uma plataforma de código aberto usada para gerenciar clusters de servidores. Ele foi introduzido em 2009, antes que os contêineres começassem a ganhar ampla adoção após o lançamento do Docker em 2013.

O Mesos pega uma carga de trabalho definida pelo usuário -- conhecida como tarefa -- e a executa em um cluster de servidores. Embora o Mesos possa executar contêineres, ele também pode executar aplicativos não conteinerizados.

### Apache Mesos vs. Kubernetes: As principais diferenças
Apesar da popularidade do Kubernetes, nem sempre é a melhor escolha em comparação com orquestradores rivais como Mesos. Em vez de ver o Kubernetes como melhor ou pior do que alternativas, é mais útil entender as diferenças fundamentais em como cada plataforma opera.

### Tipos de carga de trabalho
O Mesos suporta qualquer tipo de carga de trabalho -- conteinerizada ou não -- enquanto o Kubernetes é projetado especificamente para aplicativos em contêineres.

É tecnicamente possível executar aplicativos não conteinerizados no Kubernetes implantando-os em uma VM e executando-os dentro de um cluster Kubernetes com um complemento, como o KubeVirt. Mas fazer isso requer configuração extra e mais ferramentas, enquanto o Mesos pode executar aplicativos não conteinerizados prontos para uso.

### Rede
Em comparação com o Kubernetes, a rede no Mesos é mais fácil de configurar, mas menos flexível.

O Kubernetes suporta plug-ins de gerenciamento de rede compatíveis com a CNI (Container Network Interface). Dependendo de suas necessidades e nível de complexidade de rede, você pode escolher entre uma variedade de plug-ins de rede Kubernetes.

O Mesos não usa plugins de rede por padrão. Em vez disso, ele usa recursos de rede internos que podem atribuir portas a cargas de trabalho na definição, mas não fornecem controle granular sobre a configuração da rede. Embora o Mesos agora ofereça suporte à CNI, ele é menos maduro e nem todos os plugins da CNI são compatíveis com o Mesos.


## Razões para escolher Mesos vs. Kubernetes
Então, por que uma organização escolheria Mesos em vez de Kubernetes?

Primeiro, o Mesos existe há mais tempo do que o Kubernetes e, portanto, é um pouco mais maduro. O Mesos também pode ser mais fácil de configurar do que o Kubernetes -- desde que ele suporte seus requisitos de rede e armazenamento com base em seus recursos nativos. A capacidade da Mos de executar aplicativos não conteinerizados nativamente também é uma vantagem, especialmente para organizações que desejam implantar uma variedade de tipos de aplicativos.

Por outro lado, o Kubernetes é uma escolha melhor do que o Mesos para organizações que procuram se beneficiar das centenas de complementos e integrações de código aberto fornecidas pela comunidade Kubernetes. Escolher o Kubernetes também torna mais fácil encontrar engenheiros com a experiência certa para dar suporte aos seus clusters.