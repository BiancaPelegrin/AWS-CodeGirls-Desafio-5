# AWS-CodeGirls-Desafio-5


----


# 🚀 Guia de Introdução: AWS CloudFormation e Terraform

Este repositório faz parte do **Bootcamp Santander Code Girls 2025**, promovido pela **DIO (Digital Innovation One)**.  
Aqui, implementei minha **primeira infraestrutura como código (IaC)** utilizando **AWS CloudFormation**, explorando também as diferenças entre o CloudFormation e o **Terraform**, duas das ferramentas mais utilizadas no mercado para automação e gerenciamento de infraestrutura em nuvem.

---

## ☁️ O que é Infraestrutura como Código (IaC)?

**Infraestrutura como Código (IaC)** é uma prática que permite **criar, gerenciar e provisionar ambientes de nuvem** por meio de código, em vez de realizar configurações manuais.  
Essa abordagem traz **automação, consistência e escalabilidade**, reduzindo erros humanos e tornando as implantações mais ágeis e previsíveis.

---

## 📘 O que é AWS CloudFormation?

O **AWS CloudFormation** é um serviço nativo da **Amazon Web Services (AWS)** que permite **modelar e configurar recursos de nuvem** de forma automatizada e segura.  
Com ele, você define os recursos desejados (como **instâncias EC2, buckets S3, bancos de dados RDS**, entre outros) em **templates YAML ou JSON**, e o CloudFormation se encarrega de criar e gerenciar tudo automaticamente dentro de uma **Stack**.

### ✅ Benefícios do AWS CloudFormation
- **Automação e consistência:** Provisiona recursos de forma previsível e sem erros manuais.  
- **Gerenciamento centralizado:** Monitora e atualiza todos os recursos de uma stack como uma única unidade.  
- **Controle de versão:** Templates podem ser versionados no GitHub, facilitando rastreamento e colaboração.  
- **Gerenciamento de dependências:** O serviço entende as relações entre recursos e os cria na ordem correta.  

### 🛠️ Formatos de Template
Os templates podem ser escritos em:
- **YAML** → Formato mais legível e prático para humanos.  
- **JSON** → Formato estruturado e amplamente compatível com integrações.

---

## 🌍 O que é Terraform?

O **Terraform**, desenvolvido pela **HashiCorp**, é uma ferramenta **open-source e multicloud**, usada para criar e gerenciar infraestrutura em diversos provedores como **AWS, Azure, Google Cloud, Oracle, entre outros**.  
Ele utiliza sua própria linguagem chamada **HCL (HashiCorp Configuration Language)**, que é simples, declarativa e muito flexível.

### 💡 Benefícios do Terraform
- **Multicloud:** Permite gerenciar diferentes provedores de nuvem com o mesmo conjunto de ferramentas.  
- **Código reutilizável:** Estrutura modular que facilita a replicação de ambientes.  
- **Comunidade ativa:** Possui grande suporte e muitos módulos prontos.  
- **Controle de estado:** Mantém um arquivo chamado `terraform.tfstate`, que registra o estado atual da infraestrutura.  

---

## 🔄 Comparativo: AWS CloudFormation vs Terraform

| Característica | **AWS CloudFormation** | **Terraform** |
|----------------|------------------------|---------------|
| **Provedor** | Exclusivo da AWS | Multicloud (AWS, Azure, GCP etc.) |
| **Linguagem** | YAML ou JSON | HCL (HashiCorp Configuration Language) |
| **Gerenciamento de Estado** | Feito automaticamente pela AWS | Feito via arquivo `.tfstate` local ou remoto |
| **Integração com AWS** | Nativa e profunda | Boa, mas via APIs externas |
| **Custo** | Gratuito (paga-se apenas pelos recursos criados) | Gratuito (open-source) |
| **Curva de Aprendizado** | Simples para quem usa só AWS | Mais flexível, porém com mais configuração |
| **Suporte Multicloud** | Não | Sim |
| **Comunidade e Módulos Prontos** | Limitado à AWS | Extensa e diversificada |

---

## 🧩 Quando Usar Cada Um?

- Use **CloudFormation** se você trabalha **exclusivamente com AWS** e busca **integração nativa** e simplicidade.  
- Use **Terraform** se você precisa de **flexibilidade multicloud** ou pretende gerenciar **ambientes híbridos** (várias plataformas).  

Ambas as ferramentas seguem o mesmo princípio de **Infraestrutura como Código**, mas diferem em **abrangência e portabilidade**.

---

## 🏆 O que foi abordado no Bootcamp DIO

Durante o desafio, foram explorados:
- Criação de **templates YAML/JSON** no CloudFormation;  
- **Provisionamento automático** de instâncias EC2, roles IAM e buckets S3;  
- **Parâmetros e outputs** para reuso de templates;  
- **Automação e padronização** de ambientes AWS;  
- Boas práticas de **modularização, controle de custos e versionamento**.  

---

## 📚 Referências

- [AWS CloudFormation - Guia de Início Rápido](https://docs.aws.amazon.com/pt_br/AWSCloudFormation/latest/UserGuide/gettingstarted.walkthrough.html)  
- [Documentação Oficial do Terraform](https://developer.hashicorp.com/terraform/docs)  
- [Laboratório DIO – Automação de Infraestrutura com CloudFormation](https://web.dio.me)

---