# Kubernetes

Kubernetes é um plataforma de código aberto, portável e extensiva para o gerenciamento de cargas de trabalho e serviços distribuídos em contêineres, que facilita tanto a configuração declarativa quanto a automação. Ele possui um ecossistema grande, e de rápido crescimento. Serviços, suporte, e ferramentas para Kubernetes estão amplamente disponíveis.

### Kubernetes Clusters
O Kubernetes coordena um cluster altamente disponível de computadores que estão conectados para trabalhar como uma única unidade. As abstrações no Kubernetes permitem implantar aplicativos em contêineres em um cluster sem vinculá-los especificamente a máquinas individuais. Para fazer uso desse novo modelo de implantação, os aplicativos precisam ser empacotados de uma forma que os desacople de hosts individuais: eles precisam ser conteinerizados. Os aplicativos em contêineres são mais flexíveis e disponíveis do que nos modelos de implantação anteriores, em que os aplicativos eram instalados diretamente em máquinas específicas como pacotes profundamente integrados ao host. O Kubernetes automatiza a distribuição e o agendamento de contêineres de aplicativos em um cluster de maneira mais eficiente. O Kubernetes é uma plataforma de código aberto e está pronto para produção.

Um cluster do Kubernetes consiste em dois tipos de recursos:

O Plano de Controle coordena o cluster  
Os nós são os trabalhadores que executam aplicativos

## O que o Kubernetes não é

O Kubernetes não é um sistema PaaS (plataforma como serviço) tradicional e completo. Como o Kubernetes opera no nível do contêiner, e não no nível do hardware, ele fornece alguns recursos geralmente aplicáveis comuns às ofertas de PaaS, como implantação, escalonamento, balanceamento de carga, e permite que os usuários integrem suas soluções de logging, monitoramento e alerta. No entanto, o Kubernetes não é monolítico, e essas soluções padrão são opcionais e conectáveis. O Kubernetes fornece os blocos de construção para a construção de plataformas de desenvolvimento, mas preserva a escolha e flexibilidade do usuário onde é importante.

## Escalonando containers, não equipes
Concebido com base nos mesmos princípios que permitem ao Google executar milhares de contêineres por semana, o Kubernetes pode ser redimensionado sem aumentar sua equipe de operações.

## O que o Kubernetes pode fazer por você?
Com os serviços da Web modernos, os usuários esperam que os aplicativos estejam disponíveis 24 horas por dia, 7 dias por semana, e os desenvolvedores esperam implantar novas versões desses aplicativos várias vezes ao dia. A conteinerização ajuda a empacotar o software para atender a esses objetivos, permitindo que os aplicativos sejam lançados e atualizados de maneira fácil e rápida, sem tempo de inatividade. O Kubernetes ajuda a garantir que esses aplicativos em contêiner sejam executados onde e quando você quiser e os ajuda a encontrar os recursos e ferramentas de que precisam para funcionar. Kubernetes é uma plataforma de código aberto pronta para produção, projetada com a experiência acumulada do Google em orquestração de contêineres, combinada com as melhores idéias da comunidade.

## Arquitetura Kubernetes

Para entender como o Kubernetes é capaz de fornecer esses recursos, é útil ter uma noção de como ele é projetado e organizado em alto nível. O Kubernetes pode ser visualizado como um sistema construído em camadas, com cada camada superior abstraindo a complexidade encontrada nos níveis inferiores.

Em sua base, o Kubernetes reúne máquinas físicas ou virtuais individuais em um cluster usando uma rede compartilhada para se comunicar entre cada servidor, novamente sejam máquinas físicas ou virtuais. Esse cluster do Kubernetes é a plataforma física onde todos os componentes, recursos e cargas de trabalho do Kubernetes são configurados.

As máquinas no cluster do Kubernetes recebem uma função dentro do ecossistema do Kubernetes. Um servidor (ou um pequeno grupo em implantações altamente disponíveis) funciona como o servidor mestre. Esse servidor atua como um gateway e cérebro para o cluster, expondo uma API do Kubernetes para usuários e clientes, verificando a integridade de outros servidores, decidindo a melhor forma de dividir e atribuir trabalho (conhecido como "agendamento") e orquestrando a comunicação entre outros componentes (às vezes chamada de orquestração de contêiner). O servidor mestre atua como o principal ponto de contato com o cluster e é responsável pela maioria da lógica centralizada que o Kubernetes fornece.

As outras máquinas no cluster são designadas como nós: servidores responsáveis por aceitar e executar cargas de trabalho usando recursos locais e externos. Para ajudar com isolamento, gerenciamento e flexibilidade, o Kubernetes executa aplicativos e serviços em contêineres, portanto, cada nó precisa ser equipado com um tempo de execução de contêiner (como Docker ou rkt). O nó recebe instruções de trabalho do servidor mestre e cria ou destrói contêineres de acordo, ajustando as regras de rede para rotear e encaminhar o tráfego adequadamente.

Como mencionado acima, os próprios aplicativos e serviços são executados no cluster dentro de contêineres. Os componentes subjacentes garantem que o estado desejado dos aplicativos corresponda ao estado real do cluster. Os usuários interagem com o cluster comunicando-se com o servidor principal da API do Kubernetes diretamente ou com clientes e bibliotecas. Para iniciar um aplicativo ou serviço, um plano declarativo é enviado em JSON ou YAML definindo o que criar e como ele deve ser gerenciado. Em seguida, o servidor mestre pega o plano e descobre como executá-lo na infraestrutura examinando os requisitos e o estado atual do sistema. Esse grupo de aplicativos definidos pelo usuário em execução de acordo com um plano especificado representa a camada final do Kubernetes.

![](Arquitetura%20Cluster%20Kubernetes.png)

## Noções Básicas do Kubernetes

### Início do Minikube

### O que você vai precisar
2 CPUs ou mais  
2GB de memória livre  
20GB de espaço livre em disco  
Ligação à Internet  
Gerenciador de contêiner ou máquina virtual, como: Docker, QEMU, Hyperkit, Hyper-V, KVM, Parallels, Podman, VirtualBox ou VMware Fusion/Workstation

minikube é Kubernetes local, com foco em facilitar o aprendizado e desenvolvimento para o Kubernetes.

Tudo o que você precisa é de um contêiner do Docker (ou similarmente compatível) ou de um ambiente de Máquina Virtual, e o Kubernetes está a um único comando de distância:  [Minikube Start](https://minikube.sigs.k8s.io/docs/start/)