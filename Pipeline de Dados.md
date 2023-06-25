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