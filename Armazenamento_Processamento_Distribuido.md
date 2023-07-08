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
* Alternativas incluem: Parquet, Avro, JSON, CSV, ORC, HDF5 e vários outros formatos.


### Quando Usar Um Data Warehouse?

Um Data Warehouse é um tipo de banco de dados projetado especificamente para consultas e análises eficientes de grandes quantidades de dados. Ele é normalmente usado par armazenar e gerenciar dados de várias fontes, como bancos de dados transacionais ou arquivos de log.

Data Warehouse é um conceito, logo pode ser criado com SGBD SQL ou NoSQL, no formato colunar ou baseado em linha. 

#### Existe vários motivos pelos quais você pode optar por usar um Data Warehouse.
1. Grande volume de dados:
   * Se a Empresa possui um grande volume de dados que precisam ser armazenados e analisados, um Data Warehouse pode ser uma solução eficiente.
2. Necessidade de desempenho de consulta analítica:
   * Os DW são projetados especificamente para o desempenho de consultas, o que pode ser importante se você precisar recuperar e anaisar grandes quantidades de dados de maneira rápida.
3. Necessidade de integrar dados de várias fontes:
   * Se você tiver dados de várias fontes que precisa integrar e analisar em conjunto, um DW pode ser uma ferramente útil.
4. Necessidade de oferecer suporte à inteligência de negócios (BI) e relatórios:
   * Os DW costumam ser usados como base para inteligência de negócios e sistemas de relatórios, pois permitem consultas e análises de dados rápidas e eficientes.
5. Necessidade de dados históricos:
   * Os DW são frequentemente usados para armazenar dados históricos, pois permitem consultas e análises de dados ao longo do tempo.  

Em geral, um Data Warehouse é uma boa opção se você tiver grande volume de dados que precisa armazenar e analisar com eficiência ou se precisar oferecer suporte a sistemas de relatórios e inteligência de negócios.