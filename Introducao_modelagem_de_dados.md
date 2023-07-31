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

### Granularidade

Granularidade é o nível de detalhe ou precisão com que os dados são representados em um modelo de dados.

A granularidade dos dados pode ser alta, quando os dados são divididos em muitas entidades e atributos pequenos, ou baixa, quando os dados são agregados em poucas entidades e atributos maiores. A granularidade é uma característica importante a ser considerada na modelagem de dados, pois afeta a capacidade de armazenar, recuperar e analisar dados. Uma granularidade alta permite uma maior flexibilidade e precisão na análise dos dados, mas pode exigir mais armazenamento e processamento. Por outro lado, uma granularidade pode resultar em dados agregados e menos precisos, mas pode ser mais fácil de armazenar e processar. Portanto, é importante equilibrar a granularidade dos dados com as necessidades de negócio e técnica para garantir uma boa modelagem de dados.

### O Que São Formas Normais?

As Formas Normais são um conjunto de regras e princípios que foram desenvolvidos para garantir a integridade dos dados e a eficiência do banco de dados. Elas são usadas na modelagem relacional para garantir que as tabelas e relacionamentos estejam corretamente projetados e para evitar problemas como a redundância de dados e a inconsistência. Existem várias formas normais, cada uma com seus próprios critérios e requisitos.

#### Principais Formas Normais

As principais formas normais são:

1. Forma Normal (1NF): Todos os valores em uma tabela devem ser atômicos, ou seja, indivisíveis.
2. Forma Normal (2NF): Todos os atributos não chave devem ser dependentes funcionalmente da chave primária.
3. Forma Normal (3NF): Não deve haver dependência transitiva de não chave para chave.
4. Forma Normal (4NF): Não deve haver relacionamentos multivalorados.
5. Forma Normal (5NF): Não deve haver relacionamentos com atributos dependentes.

Cada forma normal é uma etapa para se chegar a uma tabela estruturada e sem redundância e cada uma dessas formas normais é uma pré-condição para a seguinte, e aplicando-as em ordem, garantem-se uma melhor estruturação do banco de dados.

A normalização (aplicação das formas normais) é feita ao final do processo de modelagem para ajustar o modelo e prepará-lo para o banco de dados. 

Vale resaltar que a normalização é aplicada em modelos de dados de bancos de dados transacionais. Em bancos de dados multidimensionais, como o DW, aplicamos a normalização, pois os dados devem ser agregados para facilitar as análises.

### A importância do Particionamento em Modelagem de Dados

O particionamento é a técnica de dividir grandes tabelas ou índices em partes menores chamadas partições. Isso é importante na modelagem de dados porque permite gerenciar grandes volumes de dados de forma mais eficiente e escalável.

Algumas das vantagens do particionamento são:

* Melhora o desempenho das consultas: Ao particionar grandes tabelas, as consultas podem ser direcionadas para uma partição específica, o que pode aumentar significativamente a velocidade de recuperação dos dados.
* Facilita a manutenção e backup dos dados: As partições podem ser gerenciadas de forma independente, o que permite fazer backup, recuperação ou migração de uma partição sem afetar o restante dos dados.
* Melhora a escalabilidade: Particionar as tabelas permite distribuir os dados em vários dispositivos ou servidores, o que aumenta a capacidade de armazenamento e a capacidade de processamento.

Além disso, o particionamento também pode ser usado para organizar os dados por data, geolocalização, ou outras características, tornando mais fácil e rápido para os usuários encontrar e analisar os dados relevantes para as análises.

### O Engenheiro de Dados Deve Ser Responsável Pela Modelagem de Dados?

O Engenheiro de Dados é responsável por construir e manter sistemas de gerenciamento de dados. Isso inclui a modelagem de dados. 

Ele é responsável por projetar a estrutura de dados, incluindo entidades,  atributos e relacionamentos, e garantir que os dados sejam armazenados de forma consistente e coerente com as necessidades de negócios.

Além da modelagem de dados, o Engenheiro de Dados também é responsável por outras tarefas relacionadas a dados, como:
* Garantir a qualidade dos dados, limpando, transformando e validando os dados antes de serem armazenados.
* Otimizar o desempenho dos bancos de dados, incluindo o particionamento de tabelas e o projeto de índices.
* Garantir a segurança dos dados, incluindo a criptografia de dados sensíveis e a implementação de medidas de segurança.
* Monitorar e gerenciar os sistemas de gerenciamento e pipelines de  dados  para garantir a disponibilidade e desempenho.

Em resumo, o Engenheiro de Dados é responsável por garantir que os dados sejam armazenados de forma eficiente e estruturada, e que estejam disponíveis para análise e uso em toda a organização.