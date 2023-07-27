# Introdução à Modelagem de Dados

Dados são valores, observações ou resultados de medição armazenados em um sistema ou base de dados. Eles podem ser estruturados, como os dados armazenados em tabelas de banco de dados relacional, ou não estruturados, como texto não formatado, imagens ou áudio.

Quando transformados ou processados os dados se tornam informações que suportam a tomada de decisões. Dados podem representar qualquer tipo de informação, como textos, números, imagens, som, vídeo, entre outros. Dados são usados para descrever eventos, tendências, relações e outras características e interesse.

Eles são coletados, armazenados e processados para fornecer informações úteis para a tomada de decisão, a pesquisa e outros fins. E dados precisam ser modelados para que possamos armazená-los e processá-los de forma eficiente.

## O que é Modelagem de Dados?

Modelagem de dados é o processo de projetar e criar modelos ou estruturas lógicas que representam como os dados são armazenados, relacionados e usados. Isso inclui a definição de tabelas, campos e relacionamentos em um banco de dados, bem como a criação de diagramas e especificações que descrevem como os dados serão usados em aplicativos e sistemas.

A modelagem de dados é uma etapa importante na construção de sistemas de informação eficientes e confiáveis.

### Modelagem Relacional X Modelagem Dimensional X Modelagem de Data Lakes

#### Modelagem Relacional

A **Modelagem Relacional** é uma abordagem para projetar bancos de dados que se baseia nas relações entre as entidades, com tabelas e campos. Isso envolve a criação de tabela sque representam entidades, como clientes ou pedidos, e definição de relações entre essas tabelas, como "um cliente pode fazer vários pedidos".

A modelagem relacional é amplamente utilizada em sistemas de gerenciamento de banco de dados relacional (SGBDs) e é uma abordagem estruturada e estável para armazenar e gerenciar dados em sistemas transacionais.

#### Modelagem Dimensional

A **Modelagem Dimensional** é uma técnica de modelagem de dados utilizada principalmente em sisrtemas de Business Intelligence (BI) e Data Warehousing (WD). Ela consiste em modelar os dados de forma a facilitar a análise de dados multidimensionais.

Os modelos dimensionais são construídos a partir de fatos (tabelas de medidas) e dimensões (tabelas de contexto), onde os fatos são medidas quantitativas, como vendas, e as dimensões são contextos dessas medidas, como data, local, produto, entre outros. Essas dimensões são divididas em hierarquias, o que permite uma análise detalhada dos dados.

#### Modelagem Data Lakes

A **Modelagem Data Lakes**, por outro lado, é uma abordagem para projetar sistemas de armazenamento de dados que são voltados para análise de grandes volumes de dados não estruturados. Um Data Lake é uma grande coleção de dados brutos, normalmente armazenada em sistemas de arquivos distribuídos, como o HDFS, que podem ser facilmente acessados e processados por ferramentas de análise de Big Data.

É menor estruturada e mais flexível do que a Modelagem Relacional e é projetada para lidar com grandes volumes de dados e permitir análises exploratórias dos dados. Com Data Lakes estamos preocupados primeiro em armazenar os dados no formato bruto, mas em algum momento os dados terão que ser organizados e estruturados e podem ser modelados e carregados em um DW, por exemplo.