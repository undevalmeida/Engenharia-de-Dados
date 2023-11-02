# O que é IaC?

Infraestrutura como código(IaC) refere-se ao gerenciamento e provisionamento da infraestrutura por meio de códigos, em vez de processos manuais. A sigla vem do termo em inglês, "Infrastructure as Code".

Nesta abordagem, arquivos de configuração que incluem as especificações da sua infraestrutura são criados, facilitando a edição e a distribuição das configurações. A IaC também assegura o provisionamento do mesmo ambiente, todas as vezes. Ao codificar e documentar as especificações de configuração, a IaC auxilia no gerenciamento de configuração e ajuda a evitar alterações de configuração ad-hoc não documentadas.

O controle de versão é uma parte importante IaC. Os arquivos de configuração devem pertencer à fonte como qualquer outro código-fonte de software. Ao implantar a infraestrutura como código, também é possível separá-la em módulos, que podem ser combinados de diferentes maneiras por meio de automação.

Ao automatizar o provisionamento da infraestrutura com a IaC, os desenvolvedores não previsam provisionar e gerenciar manualmente servidores, sistemas operacionais, armazenamento e outros componentes de infraestrutura sempre que criam ou implantam uma aplicação.

A codificação da infraestrutura oferece um template de provisionamento para você seguir. Ainda que esse processo possa ser feito manualmente, há ferramentas de automação, capazes de cuidar disso para você.

## IaC Declarativa e IaC Imperativa

A abordagem declarativa define o estado desejado do sistema, incluindo os recursos necessários, as propriedades que eles precisam ter e uma ferramenta de IaC para configurá-lo. 

Essa abordagem também mantém uma lista do estado atual dos objetos do seu sistema, simplificando o gerenciamento da desativação da infraestrutura.

Por outro lado, a abordagem imperativa define os comandos específicos necessários para alcançar a configuração desejada. Depois, esses comandos precisam ser executados na ordem correta. 

Muitas das ferramentas de IaC que usam uma abordagem declarativa provisionam automaticamente a infraestrutura desejada. Se você alterar o estado desejado, uma ferramenta de IaC declarativa aplicará as alterações para você. Uma ferramenta imperativa exige que você saiba como as alterações deverão ser aplicadas.

## Benefícios

O provisionamento de infraestrutura sempre foi um processo manual, caro e demorado. Agora, o gerenciamento de infraestrutura migrou do hardware físico em datacenters (ainda que eles ainda sejam um componente da sua organização) para virtualização, containers e cloud computing. 

Com a cloud computing, o número de componentes de infraestrutura aumentou, mais aplicações são colocadas em produção diariamente e as infraestruturas precisam ser flexíveis para as frequentes alterações, escalas e desativações. Hoje em dia, sem a implementação de uma prática de IaC, fica cada vez mais difícil gerenciar a escala da infraestrutura.

A IaC pode ajudar sua organização a gerenciar as necessidades de infraestrutura de TI, melhorando a consistência e reduzindo erros e a necessidade de configuração manual.

### Benefícios:
* Redução de custos
* Aumento na velocidade das implantações
* Redução de erros 
* Melhoria na consistência da infraestrutura
* Eliminação de desvios de configuração

### Ferramentas

As ferramentas de gerenciamento de configuração e automação do servidor em geral podem ser usadas para alcançar a IaC. Há também soluções específicas para IaC. 

Estas são algumas escolhas bastante conhecidas:
* Chef
* Puppet
* Red Hat Ansible Automation Platform
* Saltstack
* Terraform 
* AWS CloudFormation