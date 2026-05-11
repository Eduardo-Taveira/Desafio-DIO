 Gerenciamento de Instâncias EC2 na AWS - Desafio DIO 

Este repositório contém a documentação do projeto prático sobre AWS EC2 da DIO (Digital Innovation One). 

Objetivo do Desafio
Aplicar os conceitos de provisionamento e gerenciamento de instâncias EC2, demonstrando a compreensão da infraestrutura de rede e segurança necessária para seu funcionamento.

Arquitetura do Projeto

Para este laboratório, realizei a modelagem estrutural da arquitetura utilizando o **draw.io**. Este diagrama demonstra o conhecimento sobre como os componentes de rede e computação da AWS se interligam na prática.

Componentes Modelados:
- AWS Cloud & Region: O ambiente global onde a infraestrutura é hospedada.
- VPC (Virtual Private Cloud): A rede virtual isolada para garantir a segurança e o controle dos recursos.
- Public Subnet: A sub-rede onde a instância foi alocada, permitindo roteamento para a internet.
- Internet Gateway: O componente que permite a comunicação bidirecional entre a VPC e a internet pública.
- Security Group: O firewall virtual configurado para permitir:
  - Porta 22 (SSH): Para acesso administrativo seguro remoto.
  - Porta 80 (HTTP): Para tráfego web, permitindo que a aplicação seja acessada externamente.
- Instância EC2: O servidor de aplicação (App Server) configurado com:
  - AMI: Ubuntu 22.04
  - Tipo: t2.micro (Padrão Free Tier)
  - Storage: Root EBS Volume (20GB)

Diagrama da Arquitetura
Abaixo está a representação visual da infraestrutura projetada:



---
*Documentação criada para fins de estudo e consolidação de conhecimentos em Cloud Computing.*
