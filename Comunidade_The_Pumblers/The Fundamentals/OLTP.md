# OLTP

### Online Transaction Processing

O OLTP ou Processamento de Transações Online é um tipo de processamento de dados que consiste na execução de várias transações que ocorrem simultaneamente (transações bancárias online, compras, entrada de pedidos ou envio de mensagens de texto, por exemplo). Essas transações são tradicionalmente chamadas de transações econômicas ou financeiras, registradas e protegidas para que uma empresa possa acessar as informações a qualquer momento para fins contábeis ou de relatórios.

A definição primária para transações, sejam elas econômicas ou financeiras, continua sendo a base para a maioria dos sistemas OLTP, portanto, o processamento de transações online normalmente envolve inserir, atualizar e/ou excluir pequenas quantidades de dados em um armazenamento de dados para coletar, gerenciar e proteger essas transações. Normalmente, uma aplicação da Web, móvel ou corporativa, rastreia todas essas interações ou transações com clientes, fornecedores ou parceiros e as atualiza no banco de dados OLTP. Esses dados de transação armazenados no banco de dados são essenciais para as empresas e são usados em relatórios ou analisados visando a tomada de decisões orientada por dados.

## Requisitos para um Sistema OLTP

A arquitetura mais comum de um sistema OLTP que usa dados transacionais é uma arquitetura de três camadas que normalmente consiste em uma camada de apresentação, uma camada de lógica de negócios e uma camada de armazenamento de dados. A camada de apresentação é o front-end, onde a transação se origina por meio de uma interação humana ou é gerada pelo sistema. A camada lógica consiste em regras que verificam a transação e garantem que todos os dados necessários para concluir a transação estejam disponíveis. A camada de armazenamento de dados armazena a transação e todos os dados relacionados a ela.