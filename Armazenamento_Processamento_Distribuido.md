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

### Quando Usar Um Data Lake?

Um DW requer que os dados sejam limpos e organizados antes do armazenamento.

O Data Lake permite o armazenamento dos dados no seu formato bruto para posterior processamento e organização.

DW -> Limpa e Organiza, depois carrega. (ETL -> Extract, Transform, Load)

DL -> Carrega, depois limpa e organiza. (ELT -> Extract, Load, Transform)

Um Data Lake é um repositório centralizado que permite armazenar e processar grandes quantidades de dados estruturados e não estruturados em escala. Ele foi projetado para lidar com uma ampla variedade de tipos de dados e pode armazenar dados em sua forma bruta e não estruturada, permitindo que você armazene e processe dados de maneira mais flexível e escalável do que um banco de dados tradicional. Assim como DW, o Data Lake é um conceito.

Mas por definicção um banco de dados SQL não seria o ideal, uma vez que a ideia é carregar primeiro e limpar e organizar os dados depois. Podemos usar bancos de dados NoSQL ou tecnologias de armazenamento distribuído para construir Data Lakes, localmente ou na nuvem!

#### Existem vários motivos pelos quais você pode optar por usar um Data Lake.

1. Necessidade de armazenar e processar dados em sua forma bruta:
   * Os Data Lakes permitem que você armazene e processe dados em sua forma bruta e não estruturada, o que pode ser útil se você precisar preservar os dados originais ou se quiser manter a flexibilidade na forma como processa e analisa os dados.
2. Necessidade de armazenar e processar grandes volumes de dados:
   * Se você possui um grande volume de dados que precisam ser amazenados e processados, um Data Lake pode ser uma solução eficiente.
3. Necessidade de armazenar e processar dados estruturados e não estruturados:
   * Os Data Lakes são adequados para armazenar e processar dados estruturados e não estruturados, tornando-os uma boa escolha se você tiver uma variedade diversificada de dados.
4. Necessidade de escalabilidade:
   * Os Data Lakes são projetados para serem escaláveis, permitindo que você armazene e processe facilmente grandes quantidades de dados à medida que suas necessidades aumentam.
5. Necessidade de um repositório de dados centralizado:
   * Se você tiver dados de várias fontes que precisa armazenar e processar em local centralizado, um Data Lake pode ser uma ferramenta útil.

Em geral, um Data Lake é uma boa opção se você tiver grandes volumes de dados estruturados e não estruturados que precisa armazenar e processar em escala ou se precisar de um repositório centralizado para armazenar e processar dados de várias fontes.

### Quando Usar Um Data Lakehouse?

Um Data Lakehouse pode ser definido como uma plataforma de dados moderna construída a partir de uma combinação de um Data Lake e um Data Warehouse. Mais especificamente, um Data Lakehouse une o armazenamento flexível de dados não estruturados de um Data Lake e os recursos e ferramentas de gerenciamento de Data Warehouses e os implementa estrategicamente como um sistema maior.

Essa integração de duas ferramentas exclusivas traz o melhor dos dois mundos para os usuários. 

Data Lakehouses implementam estruturas de dados e recursos de gerenciamento de dados semelhantes aos de um Data Warehouse diretamente sobre o amazenamento em nuvem de baixo custo em formatos abertos e, normalmente, distribuídos.

O Data Lakehouse traz o princípio:
* From BI to AI

A questão é que nem todas as empresas estão usando AI (Artificial Intelligence)! Ou ainda, tudo que a empresa precisa é de um relatório de BI ou apenas de um sistema de amazenamento de dados no formato bruto!

#### Vantagens ao usar um Data Lakehouse:
1. Escalabilidade
2. Flexibilidade
3. Desempenho de Consulta
4. Repositório Centralizado
   
#### Desvantagens ao usar um Data Lakehouse:
1. Complexidade
2. Uso Intensivo de Recursos
3. Desafios Adicionais de Governança de Dados
4. Desafios Adicionais de Integração de Dados