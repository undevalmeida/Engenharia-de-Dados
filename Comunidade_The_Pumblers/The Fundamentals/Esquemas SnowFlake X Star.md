# Esquemas Snowflake X Star Schemas

No âmbito do armazenamento de dados, os esquemas de estrela e floco de neve desempenham papéis cruciais na organização de grandes quantidades de dados de forma eficiente. Ambos os esquemas oferecem vantagens exclusivas e atendem a requisitos distintos no cenário de processamento de dados. Antes de mergulhar nos detalhes, vamos primeiro fornecer uma comparação instantânea para definir o cenário: os esquemas de estrelas são mais diretos, enquanto os esquemas de floco de neve são uma versão mais normalizada dos esquemas de estrelas.

#### Aqui estão algumas diferenças importantes entre o esquema de estrela e o esquema de floco de neve:

* As tabelas de dimensão do esquema estrela não são normalizadas, enquanto as tabelas de dimensão do esquema do floco de neve são normalizadas.
* Os esquemas de flocos de neve usarão menos espaço do que os esquemas em estrela para armazenar tabelas de dimensão, mas são mais complexos.
* Os esquemas em estrela só unirão a tabela de fatos com as tabelas de dimensão, levando a consultas SQL mais simples e rápidas.
* Os esquemas Snowflake não têm dados redundantes, por isso são mais fáceis de manter.
* Os esquemas de floco de neve são bons para data warehouses, enquanto os esquemas de estrelas são melhores para datamarts com relacionamentos simples.

Essencialmente, os esquemas em estrela oferecem aos usuários uma maneira mais eficiente de organizar dados e informações em um data warehouse. Em comparação, os esquemas de floco de neve, que são uma variação dos esquemas estelares, fornecem aos usuários mais eficiência quando se trata de processar dados. Embora os dois processos sejam bastante semelhantes, eles têm diferenças importantes que os usuários também devem estar cientes. Neste artigo, primeiro vamos nos aprofundar no esquema estelar e, em seguida, fazer a transição para o esquema do floco de neve para lançar luz sobre suas nuances individuais e benefícios comparativos.

[Link](https://www.integrate.io/blog/snowflake-schemas-vs-star-schemas-what-are-they-and-how-are-they-different/)