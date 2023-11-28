# Por que você precisa do Kubernetes e o que ele pode fazer

Os contêineres são uma boa maneira de agrupar e executar seus aplicativos. Em uma produção ambiente, você precisa gerenciar os contêineres que executam os aplicativos e Certifique-se de que não há tempo de inatividade. Por exemplo, se um contêiner cair, outro O contêiner precisa ser iniciado. Não seria mais fácil se esse comportamento fosse tratado por um sistema?

É assim que o Kubernetes vem em socorro! O Kubernetes fornece uma estrutura para executar sistemas distribuídos de forma resiliente. Ele cuida do dimensionamento e do failover para seu aplicativo, fornece padrões de implantação e muito mais. Por exemplo: Kubernetes Pode gerenciar facilmente uma implantação do Canary para seu sistema.

O Kubernetes fornece a você:

* **Descoberta de serviço e balanceamento de carga** O Kubernetes pode expor um contêiner usando o nome DNS ou usando seu próprio endereço IP. Se o tráfego para um contêiner for alto, o Kubernetes poderá balancear e distribuir a carga O tráfego de rede para que a implantação seja estável.
* **Orquestração de armazenamento** O Kubernetes permite que você monte automaticamente um sistema de armazenamento de sua escolha, como armazenamentos locais, provedores de nuvem pública e muito mais.
* **Rollouts e rollbacks automatizados** Você pode descrever o estado desejado para seus contêineres implantados usando o Kubernetes, e pode alterar o estado real para o estado desejado a uma taxa controlada. Por exemplo, você pode automatizar o Kubernetes para criar novos contêineres para seu implantação, remover contêineres existentes e adotar todos os seus recursos para o novo contêiner.
* **Embalagem automática de lixeiras** Você fornece ao Kubernetes um cluster de nós que ele pode usar para executar tarefas em contêineres. Você informa ao Kubernetes quanta CPU e memória (RAM) cada contêiner precisa. Kubernetes pode caber contêineres em seus nós para fazer o melhor uso de seus recursos.
* **Auto-cura** O Kubernetes reinicia contêineres que falham, substitui contêineres, mata contêineres que não falham responder à sua verificação de integridade definida pelo usuário e não anunciá-los aos clientes até que eles estão prontos para servir.
* **Gerenciamento de segredos e configurações** O Kubernetes permite armazenar e gerenciar informações confidenciais, como senhas, tokens OAuth, e chaves SSH. Você pode implantar e atualizar segredos e configuração de aplicativos sem reconstruindo suas imagens de contêiner e sem expor segredos em sua configuração de pilha.
* **Execução em lote** Além dos serviços, o Kubernetes pode gerenciar suas cargas de trabalho em lote e CI, substituindo contêineres que falham, se desejado.
Dimensionamento horizontal Aumente e diminua a escala do seu aplicativo com um comando simples, com uma interface do usuário ou automaticamente com base no uso da CPU.
* **IPv4/IPv6 de pilha dupla** Alocação de endereços IPv4 e IPv6 para Pods e Serviços
* **Projetado para extensibilidade** Adicione recursos ao seu cluster Kubernetes sem alterar o código-fonte upstream.