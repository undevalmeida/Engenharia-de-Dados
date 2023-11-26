# O que é Apache Airflow?

Apache Airflow™ é uma plataforma de código aberto para desenvolvimento, agendamento, e monitoramento de fluxos de trabalho orientados a lotes. A estrutura Python extensível do Airflow permite que você crie fluxos de trabalho conectando-se com praticamente qualquer tecnologia. Uma interface da Web ajuda a gerenciar o estado de seus fluxos de trabalho. O fluxo de ar é Implantável de várias maneiras, variando de um único processo em seu laptop a uma configuração distribuída para suportar até mesmo os maiores fluxos de trabalho.

### Directed Acyclic Graphs - Dags

Um grafo acíclico dirigido (DAG) é uma representação conceitual de uma série de atividades. A ordem das atividades é representada por um gráfico, que é apresentado visualmente como um conjunto de círculos, cada um representando uma atividade, alguns dos quais são conectados por linhas, que representam o fluxo de uma atividade para outra. Cada círculo é conhecido como um "vértice" e cada linha é conhecida como uma "aresta". "Direcionada" significa que cada aresta tem uma direção definida, de modo que cada aresta representa necessariamente um único fluxo direcional de um vértice para outro. "Acíclico" significa que não há loops (ou seja, "ciclos") no grafo, de modo que, para qualquer vértice dado, se você seguir uma aresta que conecta esse vértice a outro, não há caminho no gráfico para voltar a esse vértice inicial.

### Por que os gráficos acíclicos direcionados são úteis?

Os DAGs são úteis para representar muitos tipos diferentes de fluxos, incluindo fluxos de processamento de dados. Ao pensar em fluxos de processamento em larga escala em termos de DAGs, pode-se organizar mais claramente as várias etapas e a ordem associada para esses trabalhos. Em muitos ambientes de processamento de dados, uma série de cálculos são executados nos dados para prepará-los para um ou mais destinos finais. Esse tipo de fluxo de processamento de dados é geralmente chamado de [pipeline de dados](https://hazelcast.com/glossary/data-pipeline/). Por exemplo, os dados de transações de vendas podem ser processados imediatamente para prepará-los para fazer recomendações em tempo real aos consumidores. Como parte do ciclo de vida do processamento, os dados podem passar por muitas etapas, incluindo limpeza (correção de dados incorretos/inválidos), agregação (cálculo de resumos), enriquecimento (identificação de relacionamentos com outros dados relevantes) e transformação (gravação dos dados em um novo formato).

Uma característica fundamental dos DAGs e dos fluxos de processamento de dados que eles modelam é que pode haver vários caminhos no fluxo. Isso é importante porque reconhece a necessidade de processar dados de várias maneiras para acomodar diferentes saídas e necessidades. No fluxo de exemplo abaixo, um fluxo de dados do sensor é processado. Os dados são carregados primeiro a partir dos sensores, depois são separados pelo tipo de sensor. Os dados do sensor X serão resumidos por segundo e, em seguida, analisados em tempo real. Se algum estado crítico for observado, um alerta será enviado. Os dados também são salvos para armazenamento de longo prazo e, possivelmente, outras análises. Também neste fluxo estão os dados do sensor Y, que por enquanto são resumidos por minuto e, em seguida, armazenados no mesmo armazenamento de longo prazo que os dados do sensor X.

# Fluxos de trabalho como código

A principal característica dos fluxos de trabalho do Airflow é que todos os fluxos de trabalho são definidos em código Python. "Fluxos de trabalho como code" serve a vários propósitos:

Dinâmico: Os pipelines de fluxo de ar são configurados como código Python, permitindo a geração dinâmica de pipelines.

Extensível: A estrutura de fluxo de ar™ contém operadores para se conectar com várias tecnologias. Todos os componentes de fluxo de ar são extensíveis para se ajustar facilmente ao seu ambiente.

Flexível: a parametrização do fluxo de trabalho é integrada aproveitando o mecanismo de modelagem Jinja.