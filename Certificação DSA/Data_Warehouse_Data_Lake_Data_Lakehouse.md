# Data Warehouse, Data Lake e Data Lakehouse

### Data Warehouse
#### Vantagens: 

* Dados estruturados e limpos, o que facilita a análise e geração de relatórios.
* Performance de consultas e relatórios é geralmente melhor devido à otimização de dados.
* Governança de dados mais robusta, garantindo a qualidade e confiabilidade dos dados.
* Maior capacidade de suportar demandas de negócios e análise avançada.

#### Desvantagens: 

* Pode ser caro e complexo de implementar e manter.
* Exige um processamento de limpeza e modelagem de dados rigoroso antes da carga de dados. Restringe a capacidade de armazenar grandes volumes de dados não estruturados.
* Pode ser limitado em lidar com dados em tempo real ou com fontes dinâmicas e não estruturadas.

### Data Lake
#### Vantagens:

* Capaz de armazenar grandes volumes de dados não estruturados e semi-estruturados.
* Flexível para lidar com diferentes formatos de dados e fontes.
* Escalável para lidar com grandes volumes de dados.
* Permite análise avançada e aplicações de Big Data, Machine Learning e IA.

#### Desvantagens:

* Governança de dados menos robusta comparado a um Data Warehouse, o que pode levar a problemas de qualidade e confiabildiade dos dados.
* Performance de consultas e relatórios pode ser menor devido à falta de otimização dos dados.
* Pode ser caro e complexo de implementar e manter.
* Depende de ferramentas adicionais para limpeza e modelagem de dados antes da análise.

### Data Lakehouse
#### Vantagens:

* Combina vantagens de Data Warehouse e Data Lakes, fornecendo a capacidade de armazenar grandes volumes de dados não estruturados e semi-estruturados, além de garantir uma boa governança e performance em consultas e relatórios.
* Flexibilidade para lidar com diferentes formatos de dados e fontes.
* Escalável para lidar com grandes volumes de dados.
* Permite análise avançada e aplicações de Big Data, Machine Learning e IA.

#### Desvantagens:

* Pode ser caro e complexo de implementar e manter, devido à necessidade de conhecimento especializado e uma equipe multidisciplinar.
* Depende de ferramentas adicionais para limpeza e modelagem de dados antes da análise.
* Ainda é um conceito recente no mercado e necessita de evolução e maturidade.

## Enterprise Data Hub

Enterprise Data Hub (EDH) é uma arquitetura de dados que combina uma variedade de tecnologias e ferramentas para permitir a coleta, armazenamento, gerenciamento e análise de dados em grande escala. É uma abordagem para criação de um repositório centralizado de dados que pode ser usado para acessar, integrar e analisar dados de várias fontes.

O objetivo é fornecer uma plataforma única para acessar todos os dados relevantes em uma empresa, independentemente de onde esses dados estejam armazenados ou como eles são formatados. A implementação de um EDH é muitas vezes complexa e desafiadora e requer uma equipe multidisciplinar e ferramentas avançadas.

## Data Mesh

É uma abordagem para construir uma arquitetura de dados descentralizada, através de um design de autoatendimento orientado a domínio (área de negócio). Data Mesh se preocupa principalmente com os dados em si, tendo DW, Data Lake, e os pipelines como uma preocupação secundária. A proposta principal é dimensionar os dados por descentralização orientada por domínio. 

Com Data Mesh a responsabilidade pelos dados usados nas análises é transferida da equipe de dados central para as equipes de domínio, apoiada por uma equipe de plataforma de dados que fornece uma plataforma independente de domínio. 