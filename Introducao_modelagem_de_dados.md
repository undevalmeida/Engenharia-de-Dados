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

## O Que É Esquema em Modelagem de Dados?

Os esquemas de dados é uma estrutura lógica que descreve como os dados estão organizados e relacionados em um banco de dados. ele define as tabelas, campos e relacionamentos entre as tabelas, além de outras restrições e propriedades dos dados.

Em um banco transacional ou em um DW, o esquema é o mandatário e deve ser definido antes da carga de dados. Um mesmo SGBD pode ter diversos bancos de dados e cada banco de dados pode ter diversos esquemas (schemas).

No Data Lake normalmente não temos esquema pré-definido, mas alguma organização será requerida para o armazenamento.

## O Que São Constraints?

Constraints, ou restrições, são regras ou limitações que são aplicadas aos dados em um banco de dados para garantir a integridade dos dados. Essas restrições podem incluir regras de validação, como verificar se um valor é numérico ou se uma data está no formato correto, ou regras de integridade referencial, que garantem que os dados em diferentes tabelas sejam consistentes entre si.

Alguns exemplos de constraints são: NOT NULL, UNIQUE, PRIMARY KEY, FOREIGN KEY, CHECK E DEFAULT.

## Modelo Conceitual, Lógico e Físico

### Modelo Conceitual

O **Modelo Conceitual** é uma das três camadas de modelagem de dados, juntamente com o modelo lógico e o modelo físico. É a camada mais abstrata da modelagem de dados e é projetada para representar os dados de uma organização de forma independente de qualquer sistema ou tecnologia específica.

O **Modelo Conceitual** é projetado para capturar a estrutura de negócio dos dados, incluindo entidades, atributos e relacionamentos, e é usado para comunicar a estrutura de dados para os stakeholders de negócios. Esse modelo é geralmente desenvolvido usando notações gráficas, como diagramas de entidade-relacionamento (ER), e é usado como base para criação dos modelos lógicos e físico.

O **Modelo Conceitual** é a primeira etapa de modelagem de dados e é importante para garantir que os dados sejam projetados de forma consistente e coerente com as necessidades de negócio da empresa. Embora às vezes seja negligenciado, esse modelo é fundamental para a compreensão sobre os dados.

### Modelo Lógico

O **Modelo Lógico** é uma das três camadas de modelagem de dados, juntamente com o modelo conceitual e o modelo físico. Ele é a representação lógica dos dados, independente da plataforma ou tecnologia de banco de dados específica que será usada na implementação física.

O **Modelo Lógico** é a representação dos dados como tabelas, campos e relacionamentos, e é usado para descrever a estrutura lógica dos dados. Esse modelo é projetado para capturar a estrutura de negócio nos dados, incluindo entidades, atributos e relacionamentos, mas é adaptado para se adequar às necessidades de implementação do banco de dados, independente da tecnologia usada.

Ele é geralmente desenvolvido usando notações gráficas, como diagramas de entidade-relacionamento (ER), e é usado como base para criação do modelo físico. 

O **Modelo Lógico** permite identificar eventuais problemas que poderão ocorrer na implementação física.

### Modelo Físico

O **Modelo Físico** é a última camada de modelagem de dados. Ele é a representação física dos dados, incluindo a estrutura de armazenamento e as configurações de banco de dados epecíficas. Ele descreve como os dados serão armazenados e como eles serão acessados em um sistema de gerenciamento de banco de dados específico.

O **Modelo Físico** deve conter todas as definições de constraints, índices e particionamento dos dados.

O **Modelo Físico** incui detalhes como o nome das tabelas e campos, tipo de dados, tamanho, índices, chaves estrangeiras e outras configurações de banco de dados específicas. Esse modelo normalmente é uma extensão do modelo lógico contendo os detalhes de implementação em um SGBD espcífico. Diversas ferramentas de modelagem permitem converter um modelo lógico para um modelo físico de acordo com o SGBD escolhido.

Ele é a etapa final da modelagem de dados e é importante para garantir a eficiência, desempenho e escalabilidade do banco de dados.