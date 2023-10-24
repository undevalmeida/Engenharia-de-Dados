# Iniciando com Projetos de Engenharia de Dados

### O Que Fazer Antes de Decidir as Tecnologias

1. Data Sourcers
   1. Quais aplicações?
   2. Qual tipo de linguagem?
   3. Qual domínio das aplicações (se é desenvolvido na empresa ou por terceiros)?
   4. Como acessar os dados que essas applicações produzem?
   5. Quais tipos de banco de dados?
   6. Quais tipos de arquivos (csv, txt, parquet, json etc)?
   7. Tipo de extração de dados 
   8. Decidir tecnologia de ingestão
2. Data Processing
   1. Joins entre tabelas?
   2. Calculos matemáticos?
   3. Como serão as regras de negócio?
   4. Preciso converter algum tipo de dado recebido?
   5. Qual latência de processamento (batch ou streaming)?
3. Data Serving
   1. Serão relatórios?
   2. Vamos entregar esses dados analíticos a outras bases? (Conceito de ETL reverso, sistemas acessam o Data Warehouse)
   3. Os dados serão usados para Machinne Learning?
4. Decisão da tecnologia que se encaixa melhor

Após entender tudo isso iremos para outras partes...