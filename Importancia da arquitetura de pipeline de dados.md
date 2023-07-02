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