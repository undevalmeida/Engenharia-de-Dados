# VPC (Virtual Private Cloud)

Com a Amazon Virtual Private Cloud (Amazon VPC), é possível iniciar recursos da AWS em uma rede virtual definida por você. Essa rede virtual se assemelha a uma rede tradicional que você operaria no seu datacenter, com os benefícios de usar a infraestrutura dimensionável da AWS.

O seguinte diagrama mostra uma VPC de exemplo. A VPC tem uma sub-rede em uma das zonas de disponibilidade na região, instâncias do EC2 em cada sub-rede e um gateway da Internet para permitir a comunicação entre os recursos em sua VPC e a Internet.

### Recursos

Os recursos a seguir ajudam você a configurar uma VPC para fornecer a conectividade de que as aplicações precisam:

#### Nuvens privadas virtuais (VPC)
Uma VPC é rede virtual muito semelhante a uma rede tradicional que pode você pode operar no seu próprio datacenter. Após criar uma VPC, você pode criar sub-redes.

#### Sub-redes
Uma sub-rede é uma gama de endereços IP na VPC. Uma sub-rede deve residir em uma única zona de disponibilidade. Após adicionar as sub-redes, você pode implantar os recursos da AWS na VPC.

#### Endereçamento IP
É possível atribuir endereços IPs, tanto IPv4 quanto IPv6, às suas VPCs e sub-redes. Você também pode trazer os endereços GUA IPv4 e IPv6 públicos para a AWS e alocá-los aos recursos na VPC, como instâncias do EC2, gateways NAT e balanceadores de carga da rede.

#### Roteamento
Use tabelas de rotas para determinar para onde o tráfego da sub-rede ou do gateway será direcionado.

#### Gateways e endpoints
Um gateway conecta a VPC a uma outra rede. Por exemplo, use um gateway da Internet para conectar a VPC à Internet. Use um endpoint da VPC para se conectar a Serviços da AWS de modo privado, sem usar um gateway da Internet ou um dispositivo NAT.

#### Conexões de emparelhamento
Use uma conexão de emparelhamento da VPC para rotear o tráfego entre os recursos em duas VPCs.

#### Espelhamento de tráfego
Copie o tráfego de rede das interfaces de rede e envie aos dispositivos de segurança e monitoramento para inspeção profunda dos pacotes.

#### Gateways de trânsito
Use um gateway de trânsito, que funciona como um hub central, para rotear tráfego entre VPCs, conexões VPN e conexões do AWS Direct Connect.

#### Logs de fluxo da VPC
Um log de fluxo captura informações sobre o tráfego IP de entrada e saída nas interfaces de rede da VPC.

#### Conexões da VPN
Conecte as VPCs às redes on-premises usando a AWS Virtual Private Network (AWS VPN) .