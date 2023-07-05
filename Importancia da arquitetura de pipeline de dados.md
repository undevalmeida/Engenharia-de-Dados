# A importância da Arquitetura de Pipelines de Dados

## Como iniciamos um projeto de pipeline de dados?
1. [ ] Iniciamos pelas ferramentas, pois existe uma curva de aprendizado e quanto antes começar, melhor!
2. [ ] Iniciamos pelos dados, já que eles são o novo petróleo, o novo ouro, um ativo corporativo e devem ser prioridade.
3. [x] Iniciamos pela compreensão dos requisitos de negócio e o que se espera do uso de dados no dia a dia.

Os pipelines de dados não são peças isoladas criadas pela área de TI (Ou pelo menos não deveria ser). Os pipelines de dados são parte da arquitetura de dados de uma empresa, que por sua vez é parte da plataforma de dados da empresa.
1. Plataforma de dados
2. Arquitetura de dados de uma empresa
3. Pipeline de dados

Logo, cada pipeline de dados devem ter um propósito e deve fazer parte de uma arquitetura de dados que atenda aos requisitos de negócio da empresa, com o menor custo possível, com segurança e que seja flexível às mudanças ao longo do tempo. 

Uma boa estratégia é criar uma POC (Prova de Conceito), uma espécie de laboratório, que simula cenários, valida requisitos de negócio, testa ferramentas e ajuda a prever os custos.

![Pipeline de Dados](Pipeline%20de%20Dados.png)

# Antes Mesmo de Pensar em Arquitetura, as Seguintes Perguntas Devem Ser Respondidas:

1. Quais os requisitos de negócio?
2. Quais resultados finais são necessários?
3. Os dados estão disponíveis? Quais são as fontes?
4. Quais tipos de formato(s) de dados estão disponíveis?
5. Qual o crescimento esperado do volume de dados?
6. Quanto de armazenamento será necessário?
7. Quanto de capacidade computacional será necessário?
8. Usaremos dados em batch, em streaming ou ambos?
9. Já temos tecnologia que permita criar os pipelines?
10. Quais tecnologias devem ser consideradas?
11. Quais são os Acordos de Nível de Serviço (SLA's)?
12. Qual custo de implementar e manter os pipelines?
13. Qual será o destino do pipeline?
14. Como será monitoramento?
15. Usaremos diversos pipelines encadeados?
16. Vamos criar os pipelines locais, na nuvem ou ambos?

# Design de Arquitetura Moderna de Pipeline de Dados Para Empresa da Área de Manufatura

Você trabalha para  uma empresa de manufatura de médio porte que fabrica utensílios domésticos.  A empresa adquiriu recentemente alguns novos equipamentos de fabricação. Essas novas  máquinas  são  sofisticadas  e  podem  se  conectar  à  rede  da  empresa,  enviando  um sinal/dados cada vez que um item é produzido. O sinal é enviado em formato TXT como arquivo plano para um computador na rede local da empresa. Em  vez  de  contar  manualmente  o  estoque,  a  empresa  gostaria  que  a  equipe  de engenharia  de  dados  capturasse  os  dados  gerados  pelas  novas  máquinas  e  os  alimentasse  no sistema  de  estoque que  reside  na  rede  local,  além  de  fornecer  painéis  de  rendimento  das máquinas a fim de prever a necessidade de manutenção preventiva e reduzir o tempo de parada das máquinas para manutenção.

Os dados são gerados pelas máquinas a cada 1 hora e armazenados no servidor local. A empresa tem atualmente 10 máquinas e mais 5 serão compradas com entrega prevista para o próximo semestre. Cada máquina gera 1 arquivo de aproximadamente 1 MB. A empresa funciona de segunda à sexta, 12 horas por dia. A  empresa  tem  um departamento  de  TI com 15 profissionais,  sendo  3  Engenheiros  de Dados,  1  Arquiteto  de  Dados, 1  Engenheiro  de  Machine  Learning, 2 Cientistas de  Dados  e  1 Analista de Dados, entre outros profissionais. Em breve a empresa irá contratar um Engenheiro de IA.

Odepartamento  de  TI  ainda  está  no  meio  de  uma  transição  para  a  nuvem,  eles  têm alguma infraestrutura na AWS (Amazon Web Service) e alguns servidores locais que hospedam o sistema usado para os registros de manufatura. Como Arquiteto de Dados ou Engenheiro de Dados, você foi encarregado de decidir como implementar um pipeline de dados que atenda esses requisitos. Vamos percorrer o processo de design da arquitetura de um pipeline de dados e como podemos abordar as diferentes maneiras de implementar uma solução.

### Nesta etapa realizamos  as seguintes  atividades:
* Compreendemos o problema.
* Compreendemos o que deve ser entregue.
* Pesquisamos a(s) fonte(s) de dados.
* Identificamos a infraestrutura atual e o que será necessário.
* Desenhar o esboço da solução. 

### Solução

![Solução](Solução%20de%20Pipeline%20de%20Dados.png)

### Uma pergunta será fundamental para definir a arquitetura de um pipeline de dados:

* **Vamos trabalhar com dados em Batch, Streaming ou Ambos?**

## Extração e Processamento dos Dados

Para a extração dos dados podemos usar um sistema de mensagens para extração do ambiente local e ingestão dos dados na nuvem. Podemos usar o Apache Kafka para extrair os dados e enviar para o ambiente em nuvem, onde o Apache Spark poderia fazer o processamento. Isso evitaria a necessidade de ter um armazenamento intermediário. Ou seja, ao invés de armazenar os dados primeiro no Data Lake e processar depois, já processaríamos os dados no momento da extração, aplicando as transformações necessárias e reduzindo o espaço total de armazenamento dos dados. O resultado do processamento seria gravado em um Data Lake para então ser usado em Machine Learning. E enviaríamos as atualizações necessárias para o sistema de estoque da empresa, atendendo assim os 2 requisitos de entrega do pipeline, com o menor custo possível e com todo processamento sendo feito na nuvem.