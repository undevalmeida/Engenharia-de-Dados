# Pipeline de Dados e o Processamento de Engenharia de Dados

## O que é um Pipeline de Dados?

Um pipeline de dados é um meio de mover dados de um local (a origem) para um destino (um Data Warehouse ou Data Lake por exemplo).

Ao longo do caminho, os dados são transformados e otimizados, chegando a um estado em que podem ser analisados e usados para desenvolver insights de negócios.

Um pipeline de dados é essencialmente o conjunto de etapas envolvidas na agregação, organização e movimentação de dados.

Os pipelines de dados modernos automatizam muitas etapas manuais envolvidas na transformação e otimização do carregamento de dados.

Normalmente o pipeline inclui carregar dados brutos em tabela de preparação (área intermediária ou Staging Area) para armazenamento temporário e, em seguida, alterá-los antes de inseri-los no destino.

Pipeline de dados é um conceito e pode ser implementado de muitas formas diferentes, desde ferramentas de automação em ambiente local, ferramentas em nuvem ou mesmo via programação de linguagens Python, R, Scala, C++ ou Java.

Um pipeline de dados é uma série de etapas de processamento de dados. Se os dados não estiverem carregados atualmente na plataforma de dados, eles serão ingeridos no início do pipeline. Depois, há uma série de etapas nas quais cada etapa fornece uma saída que é a entrada para a próxima etapa.

Isso continua até que o pipeline esteja completo. Em alguns casos, etapas independentes podem ser executadas em paralelo.

**Construir e manter pipelines de dados é uma das principais atribuições de Engenheiro de Dados**

### Componentes de um Pipeline de Dados

1. Origem
2. Processamento
3. Destino

## Pipeline de Dados X Pipeline ETL

### Pipeline ETL

Os sistemas de Extração, Transformação e Carga (ETL - Extract, Transform, Load) são um tipo de pipeline de dados, pois eles movem dados de uma origem, transformam os dados e, em seguida, carregam os dados em um destino.

Mas ETL geralmente é apenas um subprocesso de um pipeline. O termo ETL foi criado em uma época onde normalmente o único destino era um Data Warehouse e o processo era bem menos complexo. Hoje ETL faz parte de um processo maior de pipeline de dados.

Mas o processo é cada vez mais complexo e hoje podemos ter inúmeras fontes de dados, inúmeros tipos de processamento e inúmeros destinos. Por isso o termo pipeline de dados vem sendo cada vez mais usado.

### Pipeline de Dados

Um pipeline de dados é mais amplo, pois é todo o processo envolvido no transporte de dados de um local para outro, incluindo limpeza, transformação, enriquecimento, segurança, orquestração integração/entrega contínua (CI/CD).

Um pipeline de dados pode ser composto de vários pipelines ETL, além de tarefas complementares como enriquecimento de dados, gestão de metadados, linhagem de dados entre outras tarefas.

Um pipeline de dados pode ser criado para dados em batch (em lote), dados em streaming ou ambos.

Pense no pipeline de dados com uma grande avenida por onde os dados passam indo do ponto A para o ponto B. Um pipeline ETL seria uma parte desse trajeto.

Pipeline de dados robustos podem equipar uma empresa adequadamente para obter, coletar, gerenciar, analisar e usar dados com eficiência e então usar os dados para gerar novas oportunidades de mercado e fornecer processos de negócios mais eficientes e econômicos.

Os pipelines de dados modernos tornam a extração de informações dos dados coletados rápido e eficiente.

As principais características ao considerar um pipeline de dados incluem:

* Processamento de dados contínuo e extensível.
* A elasticidade e agilidade da nuvem.
* Recursos isolados e independentes para processamento de dados.
* Acesso democratizado a dados e gerenciamento de autoatendimento.
* Alta disponibilidade e recuperação de desastres.
