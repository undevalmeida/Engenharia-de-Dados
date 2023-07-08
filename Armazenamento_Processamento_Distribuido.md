# Armazenamento e Processamento Distribuído

### Onde os dados residem?

* [ ] Os dados não tem residência, eles brotam do nada!  
* [ ] Os dados aparecem como um passe de mágica quando precisamos deles.  
* [ ] Os dados residem na memória RAM do computador o tempo todo!  
* [X] Os dados residem em arquivos que são armazenados no disco físico ou outras mídias de armazenamento de dados.

As decisões de armazenamento devem ser orientadas pelas necessidades de dados e padrões de acesso e devem ser exploradas antes de apenas "escolher" algo porque é fácil. Com diversas alternativas, como armazenamento de dados usando Data Lakes, armazenamento de arquivos com Data Stores e armazenamenento em sistemas de banco de dados relacionais tradicionais, um Engenheiro de Dados que sabe como construir o melhor layout de armazenamento de arquivos não tem preço.

 ### Os Padrões de Acesso Definem o Tipo de Amazenamento

 * Quantos sistemas precisarão de acesso à camada de armazenamento de dados?
 * Com que frequência os sistemas acessarão o armazenamento de dados?
 * Qual o volume de dados que esses sistemas estarão lendo?
 * Quanta lógica será aplicada por esses sistemas aos dados?
 * Como o sistema acessa tecnicamente os dados?

### Armazenamento SQL/NoSQL ou Armazenamento de Arquivos?

#### SQL

* O armazenamento SQL é o formato tradicional de armazenamento de dados no formato tabular.
* É um dos formatos de armazenamento mais antigos e amplamente usado nos dias de hoje.
* Ideal para dados estruturados.
* Usados SGBDs (Sistemas Gerenciadores de Bancos de Dados) como Oracle, PostgreeSQL, SQL Server ou MySQL, entre outros.

#### NoSQL

* O armazenamento SQL nasceu na era do Big Data para permitir o armazenamento de dados em diferentes formatos, em especial, dados semi-estruturados como formato JSON, XML ou colunar.
* São sistemas de armazenamento orientados à performance e facilidade de uso.
* Exemplos de SGBDs NoSQL: MongoDB, Redis, Apache, Cassandra, Apache HBase e Amazon DynamoDB.

#### Variedade dos Dados
* Big Data é definido por 4 V's: Volume, Velocidade, Variedade e Veracidade.
* E o V de Variedade é normalmente uma das partes mais complexas. Pode ser necessário trabalhar com dados no formato de vídeo, áudio, imagens, texto, arquivos pdf ou mesmo ícones. Ou ainda dados em um formato que facilite a pesquisa e reduza o espaço necessário para armazenamento.
* Bancos de dados SQL ou NoSQL podem não ser ideais nesses casos (vídeo, áudio, imagem, etc...), isso sem falar na perfomance de acesso.
* Extamante aí que precisaremos de alternativas para armazenamento de diferentes formatos e diferentes sistemas.
* Alternativas incluem: Parquet, Avro, JSON, CSV, ORC, HDF% e vários outros formatos.