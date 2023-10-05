# Arquitetura Kappa é Mainstream Substituindo o Lambda

Os dados em tempo real superam os dados lentos. Isso vale para quase todos os casos de uso. No entendo, os arquitetos corporativos criam novas infraestruturas com a arquitetura Lambda que inclui camadas em lote e em tempo real separadas. Esta postagem explora por que um único pipeline em tempo real, chamado de arquitetura Kappa, é o melhor ajuste. Exemplos do mundo real de empresas como Disney, Shopify, Uber e Twitter exploram os benefícios Kappa, mas também mostram como o processamento em lote se encaixa positivamente nessa discussão sem a necessidade do Lambda.

Este post é fortemente inspirado no artigo de Jay Kreps [Questioning the Lambda Architecture](https://www.oreilly.com/radar/questioning-the-lambda-architecture/) de 2014 (!) e mapeia seus pensamentos para a situação do mundo real em 2021. Hoje, quase todas as soluções de negócios, provedores de armazenamento e análise de dados e aplicativos de negócios aproveitam o streaming de eventos e paradigmas de comunicação assíncronos e verdadeiramente desacoplados baseados em eventos para processamento de dados. Por essa razão, muitos mudam de arquiteturas Lambda para Kappa.

## Uma Arquitetura Corporativa Moderna

Uma arquitetura corporativa moderna oferece características nativas da nuvem: flexibilidade, elasticidade, automação, desacoplamento real entre diferentes aplicativos e recursos em tempo real (quando necessário).

### Microsserviços, malha de dados e design orientado a domínio para desacoplamento verdadeiro

Vamos explorar rapidamente as palavras da moda para entender como a maioria das pessoas cria arquiteturas corporativas modernas hoje:

* O DDD (Domain-driven Design) impõe limites estritos entre a comunicação de serviço e um cenário de aplicativos descentralizado.
* Os microsserviços permitem a construção de aplicativos flexíveis e desacoplados com diferentes linguagens de programação e paradigmas de comunicação.
* O Data Mesh permite arquitetar serviços em torno de dados. Dados são o produto em uma malha de dados. Os recursos de autoatendimento e a federação permitem que as unidades de negócios se concentrem em seus problemas de negócios.

[Link](https://www.kai-waehner.de/blog/2021/09/23/real-time-kappa-architecture-mainstream-replacing-batch-lambda/)