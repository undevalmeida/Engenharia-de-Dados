# Conceitos Básicos de Kubernetes

Com a utilização de containers a forma como desenvolvemos software mudou. Ao empacotar o código e suas dependências de forma isolada, a execução e teste se tornam mais rápidas e confiáveis, dispensando o uso de máquinas virtuais. Mas, ao serem utilizados, novos desafios surgem, necessitando de novas formas de integração, monitoramento e controle de recursos e quem ajuda nisso tudo é o Kubernetes. O papel do Kubernetes é trazer automação para os processos de conteinerização.

### O que é Kubernetes?

Kubernetes é uma plataforma de gerenciamento de contêineres open-source amplamente utilizada para automatizar a implantação, escalabilidade e gerenciamento de aplicativos em larga escala. Foi desenvolvido pela Google e agora é mantido pela Cloud Native Computing Foundation (CNCF).

Seu papel é gerenciar containers, pacotes de software auto-contidos que incluem todas as dependências e configurações necessárias para executar um aplicativo.

### Recursos de Gerenciamento do Kubernetes

O Kubernetes fornece uma série de recursos para gerenciar contêineres, incluindo:

* **Implantação automatizada:** Pode ser configurado para automatizar a implantação de aplicativos em containers, tornando o processo mais rápido e confiável.
* **Escalabilidade automatizada:** Consegue ajustar automaticamente o número de containers necessários para atender às demandas de tráfego, garantindo uma performance otimizada.
* Gerenciamento de recursos: Permite garantir que os aplicativos tenham acesso aos recursos de que precisam, como CPU, memória e espaço em disco, de forma equilibrada e justa.
* **Alta disponibilidade:** O Kubernetes pode garantir a disponibilidade dos aplicativos, mesmo em caso de falhas de servidor, mantendo uma cópia dos aplicativos em execução em vários servidores.
* **Atualizações de aplicativos sem interrupção:** É possível configurá-lo para atualizar aplicativos sem interrupção, garantindo a disponibilidade contínua dos aplicativos durante essas atualizações.

### Vantagens de Uso do Kubernetes

Esse gerenciador de contêineres é altamente escalável e confiável, trazendo várias vantagens para empresas e desenvolvedores de aplicativos. Aqui estão algumas das principais vantagems do uso do Kubernetes:

#### Facilidade de escalabilidade
Ele permite que você gerencie facilmente o escalonamento de aplicativos, tanto verticalmente (aumentando ou diminuindo o número de recursos, como CPU e memória, disponíveis para um aplicativo) quanto horizontalmente (aumentando ou diminuindo o número de instâncias de um aplicativo). Ajudando a garantir que os aplicativos tenham recursos suficientes para atender à demanda de usuários, sem precisar realocar manualmente os recursos.

#### Alta disponibilidade
O gerenciador é projetado para garantir alta disponibilidade de aplicativos, permitindo que você configure facilmente políticas de tolerância a falhas e alta disponibilidade para garantir que os aplicativos estejam sempre disponíveis para os usuários.

#### Automatização de deploys
Automatiza o processo de implantação de aplicativos, permitindo que você configure pipelines de implantação para implantações contínuas e automatizadas. Isso acelera o processo de desenvolvimento e ajuda a garantir que as implantações sejam confiáveis e previsíveis.

#### Portabilidade
Com ele você pode executar aplicativos em qualquer lugar, desde data centers locais até nuvens públicas, sem precisar se preocupar com a infraestrutura subjacente. Isso permite que você gerencie facilmente aplicativos em vários ambientes e facilita a migração de aplicativos entre ambientes.

#### Gerenciamento de recursos
Oferece formas avançadas de gerenciamento de recursos, como a atribuição de prioridades e garantias de recursos, que permitem que você garanta que os aplicativos tenham acesso aos meios de que precisam para funcionar de maneira eficiente.

## Como Funciona o Moonitoramento do Kubernetes

O monitoramento é uma parte importante do gerenciamento de aplicativos em um cluster Kubernetes. Ele permite que você mantenha o controle sobre o desempenho e a saúde dos aplicativos em execução, identificando e corrigindo problemas antes que eles afetem negativamente a experiência do usuário.

A monitoração no Kubernetes é realizada usando ferramentas de monitoramento, como o [Prometheus](https://prometheus.io/) e o [Grafana](https://www.opservices.com.br/grafana/), que coletam dados de [telemetria](https://www.opservices.com.br/telemetria/) sobre o cluster, incluindo informações sobre o uso de recursos, tempo de atividade e erros. Estes dados são exibidos em painéis de monitoramento, onde os administradores podem analisar e entender a saúde geral do cluster.

[Link](https://www.opservices.com.br/kubernetes/#:~:text=Kubernetes%20%C3%A9%20uma%20plataforma%20de,Native%20Computing%20Foundation%20(CNCF).)