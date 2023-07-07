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