# O que é o Amazon Relational Database Service (Amazon RDS)?

O Amazon Relational Database Service (Amazon RDS) é um serviço da Web que facilita a configuração, a operação e escalabilidade de um banco de dados relacional na Nuvem AWS. Ele fornece capacidade econômica e redimensionável para um banco de dados relacional padrão do setor e gerencia tarefas comuns de administração de banco de dados.

Por que você deseja executar um banco de dados relacional no Nuvem AWS? Porque o AWS assume muitas das tarefas de gerenciamento difíceis ou entediantes de um banco de dados relacional.

## Amazon EC2 e bancos de dados on-premises

O Amazon Elastic Compute Cloud (Amazon EC2) oferece uma capacidade de computação escalável na Nuvem AWS. O Amazon EC2 dispensa a necessidade de investir em hardware inicialmente e, portanto, você pode desenvolver e implantar aplicações com mais rapidez.

Quando você compra um servidor on-premises, recebe CPU, memória, armazenamento e IOPS, todos no mesmo pacote. Com o Amazon EC2, estes elementos se separaram, para que você possa escalá-los independentemente. Se você precisar de mais CPU, menos IOPS ou mais capacidade de armazenamento, poderá alocá-los facilmente.

Para um banco de dados relacional em um servidor on-premises, você assume total responsabilidade pelo servidor, sistema operacional e software. Para um banco de dados em uma instância do Amazon EC2, a AWS gerencia as camadas abaixo do sistema operacional. Dessa maneira, o Amazon EC2 elimina parte do peso de gerenciar um servidor de banco de dados on-premises.

O Amazon RDS fornece as seguintes vantagens específicas em relação às implantações de banco de dados que não são totalmente gerenciadas:

Você pode usar os produtos de banco de dados que já conhece com: MariaDB, Microsoft SQL Server, MySQL, Oracle e PostgreSQL.

O Amazon RDS gerencia backups, patches de software, detecção automática de falhas e recuperação.

Você pode ativar backups automatizados ou pode criar manualmente seus próprios snapshots de backup. Você pode usar esses backups para restaurar um banco de dados. O processo de restauração do Amazon RDS funciona de maneira confiável e eficiente.

Você pode obter alta disponibilidade com uma instância primária e uma instância secundária síncrona que pode ser usada para failover em caso de problemas. Também é possível usar réplicas de leitura para aumentar a escalabilidade de leitura.

Além da segurança em seu pacote de banco de dados, você pode ajudar a controlar quem pode acessar seus bancos de dados do RDS. Para fazer isso, você pode usar o AWS Identity and Access Management (IAM) para definir usuários e permissões. Você também pode ajudar a proteger seus bancos de dados colocando-os em uma nuvem privada virtual (VPC).