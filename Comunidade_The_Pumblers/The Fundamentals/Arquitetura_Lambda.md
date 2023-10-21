# O Que é Arquitetura Lambda?

A arquitetura Lambda é uma forma de processar enormes quantidades de dados ("Big Data") que fornece acesso a métodos de processamento em batch e de stream com uma abordagem híbrida. A arquitetura Lambda é usada para resolver o problema do compute de funções arbitrárias.

### Camada em Lote

Novos dados chegam continuamente, como um feed para o sistema de dados. Eles são alimentados para a camada em batch e para a camada de velocidade simultaneamente. Todos os dados são analisados de uma vez e, às vezes, corrigidos na camada de stream.  Aqui, podemos encontrar muitas ETL e um data warehouse tradicional. Essa camada é construída usando uma programação pré-definida, normalmente uma ou duas vezes por dia. A camada em batch tem duas funções muito importantes:

* Gerenciar o conjunto de dados mestre
* Fazer o pré-compute das visualizações em lote.

# Camada de Serviço

Os resultados da camada em batch na forma de visualizações em batch e aqueles provenientes da camada de velocidade na forma de visualizações quase em tempo real são encaminhados para a camada de serviço.  Essa camada indexa as visualizações em batch de forma que possam ser consultadas em baixa latência em uma base ad-hoc.

### Benefícios das arquiteturas Lambda
Conheça os principais benefícios das arquiteturas Lambda:

* Sem gerenciamento de servidor: você não precisa instalar, manter ou administrar nenhum software.
* Escala flexível: sua aplicação pode ser dimensionada automaticamente ou de acordo com o ajuste da sua capacidade
* Alta disponibilidade automatizada: refere-se ao fato de que as aplicações serverless já têm disponibilidade integrada e tolerância a falhas. Representa uma garantia de que todas as solicitações receberão uma resposta informando se foram bem-sucedidas ou não.
* Agilidade nos negócios: reaja em tempo real às mudanças nos cenários de negócios/mercado
### Desafios das arquiteturas Lambda
* Complexidade: as arquiteturas Lambda podem ter um alto nível de complexidade. Normalmente, os administradores devem manter duas bases de código separadas para camadas em batch e de streaming, o que pode dificultar a depuração.

[Link](https://www.databricks.com/br/glossary/lambda-architecture)