# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 07/05/2026
Empresa: Abstergo Industries
Responsável: Luiz Felipe Schroder Marcon

---

## Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Luiz Felipe Schroder Marcon. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar diminuições de custos imediatos, considerando que a empresa não possuía nenhuma infraestrutura em nuvem anteriormente, operando inteiramente com servidores físicos locais.

---

## Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos e especificações. A seguir, serão descritas as etapas do projeto:

---

### Etapa 1

- **Nome da ferramenta:** Amazon EC2 (Elastic Compute Cloud) com Auto Scaling
- **Foco da ferramenta:** Substituição de servidores físicos locais por instâncias de computação em nuvem escaláveis
- **Descrição de caso de uso:**
  A Abstergo Industries mantinha servidores físicos próprios para hospedar seus sistemas de gestão de vendas, controle de estoque e atendimento ao cliente. Esses servidores geravam altos custos fixos com manutenção, energia elétrica, refrigeração e substituição de hardware. Com a migração para instâncias EC2, a empresa passa a pagar apenas pela capacidade computacional efetivamente utilizada. O Auto Scaling garante que, em períodos de alta demanda como campanhas sazonais ou horários de pico no atendimento, novas instâncias sejam provisionadas automaticamente e desativadas quando não forem mais necessárias. Estima-se uma redução de até 40% nos custos de infraestrutura de TI no primeiro ano, além da eliminação de gastos com suporte técnico presencial para hardware.

---

### Etapa 2

- **Nome da ferramenta:** Amazon RDS (Relational Database Service) — MySQL
- **Foco da ferramenta:** Gerenciamento centralizado e seguro do banco de dados de clientes, receitas e estoque de medicamentos
- **Descrição de caso de uso:**
  O banco de dados da farmácia armazena informações críticas: cadastro de clientes, histórico de compras, receitas médicas digitalizadas e controle de estoque de medicamentos controlados e não controlados. Anteriormente, esse banco de dados era mantido em um servidor local sem redundância, expondo a empresa ao risco de perda total de dados em caso de falha de hardware. Com o Amazon RDS, o banco de dados passa a contar com backups automáticos diários, replicação multi-AZ, aplicação automática de patches de segurança e escalabilidade vertical com poucos cliques. Além de aumentar a segurança e a conformidade com a LGPD e as regulamentações da ANVISA para armazenamento de receitas, o serviço elimina custos com licenciamento e administração manual do banco de dados, reduzindo a necessidade de um DBA dedicado em tempo integral.

---

### Etapa 3

- **Nome da ferramenta:** Amazon S3 (Simple Storage Service)
- **Foco da ferramenta:** Armazenamento seguro, escalável e de baixo custo para documentos, receitas digitalizadas, notas fiscais e backups gerais
- **Descrição de caso de uso:**
  A farmácia lida diariamente com grande volume de documentos: receitas médicas digitalizadas, notas fiscais eletrônicas, laudos, relatórios de auditoria e comprovantes de dispensação de medicamentos controlados. Anteriormente, esses arquivos eram armazenados em HDs externos e servidores locais com capacidade limitada e sem controle de versões. Com o Amazon S3, todos os documentos são armazenados de forma durável com custo extremamente baixo por GB armazenado. É possível configurar políticas de ciclo de vida para mover arquivos antigos automaticamente para o Amazon S3 Glacier, reduzindo ainda mais os custos de retenção de longo prazo. O controle de acesso granular via IAM garante que apenas colaboradores autorizados acessem documentos sensíveis, reforçando a conformidade regulatória.

---

## Conclusão

A implementação das ferramentas na empresa Abstergo Industries tem como resultado esperado a **redução significativa dos custos operacionais de TI**, a **eliminação de riscos associados à infraestrutura física** e o **aumento da segurança e disponibilidade dos dados**. A migração para a nuvem AWS representa um passo estratégico para uma operação mais moderna, resiliente e escalável, sem a necessidade de grandes investimentos iniciais em hardware. Recomenda-se a continuidade da utilização das ferramentas implementadas e a avaliação de serviços complementares, como o AWS Cost Explorer para monitoramento de gastos, Amazon CloudWatch para observabilidade e AWS Backup para centralização de políticas de backup.

---

Assinatura do Responsável pelo Projeto:

Luiz Felipe Schroder Marcon
