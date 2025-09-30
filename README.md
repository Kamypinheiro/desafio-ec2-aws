# desafio-ec2-aws

Gerenciando Instâncias EC2 na AWS


Estou participando do curso Santander Code Girls - 2025.
Este repositório documenta minha experiência prática com o gerenciamento de instâncias EC2 na AWS.


Objetivo

O objetivo deste laboratório é consolidar meus conhecimentos em gerenciamento de instâncias EC2 na AWS. Ao concluir este desafio, espero:

Aplicar os conceitos aprendidos em um ambiente prático;
Documentar processos técnicos de forma clara e estruturada;
Utilizar o GitHub como ferramenta para compartilhamento de documentação técnica.



Passos Realizados

Criação de uma instância EC2 na AWS;

Configuração de Grupos de Segurança e gerenciamento de permissões de acesso SSH.

Criação e utilização de imagens AMI personalizadas.

Gerenciamento de snapshots do EBS para fins de backup.

Integração do EC2 com serviços como S3, Lambda e RDS.


Arquitetura 1: Integração S3 + EC2 + Lambda


Usuário interage com a instância EC2.

Os dados gerados ou enviados são armazenados no S3.

Um evento de notificação no S3 dispara a execução de uma função Lambda.

A função Lambda processa os dados e os salva em outro bucket S3.


<img width="791" height="494" alt="image" src="https://github.com/user-attachments/assets/8075e829-5cbb-4ad4-b574-5329eeada908" />


-------------------------------------


Arquitetura 2: EC2 com EBS e RDS


Usuário envia arquivos ou logs para o ambiente na nuvem.

A instância EC2 recebe e processa esses arquivos.

O armazenamento dos arquivos é realizado nas unidades EBS.

Dados processados e estruturados são gravados em um banco de dados relacional (RDS).

<img width="808" height="565" alt="image" src="https://github.com/user-attachments/assets/2f23569e-103c-4711-9e27-785601e797a4" />

