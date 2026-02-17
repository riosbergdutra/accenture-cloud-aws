# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 17/02/2026  
Empresa: Abstergo Industries  
Responsável: Riosberg Dutra dos Santos

---

## Introdução

Este relatório apresenta o processo de implementação de serviços em nuvem na empresa Abstergo Industries, com o objetivo de reduzir custos operacionais imediatos, aumentar a escalabilidade e melhorar a confiabilidade dos sistemas.

A estratégia adotada foi a utilização de três serviços da Amazon Web Services (AWS), focados em armazenamento, mensageria e comunicação assíncrona entre sistemas.

Os serviços escolhidos foram:

- Amazon S3
- Amazon SQS
- Amazon SNS

---

## Descrição do Projeto

O projeto foi dividido em três etapas estratégicas, cada uma com foco direto na otimização de custos e eficiência operacional.

---

### Etapa 1 – Implementação do Amazon S3

**Foco da ferramenta:**  
Armazenamento de objetos altamente durável, escalável e de baixo custo.

**Caso de uso:**  
A empresa mantinha servidores locais para armazenamento de arquivos, backups e documentos internos, gerando custos com:

- Infraestrutura física
- Energia elétrica
- Manutenção de hardware
- Equipe técnica dedicada

Com a migração para o Amazon S3, foi possível:

- Eliminar servidores físicos de armazenamento
- Reduzir custos com manutenção
- Utilizar classes de armazenamento mais baratas (como S3 Standard-IA e Glacier para backups)
- Pagar apenas pelo volume efetivamente utilizado

**Impacto na redução de custos:**  
Redução significativa de CapEx (infraestrutura física) e otimização de custos operacionais com modelo pay-as-you-go.

---

### Etapa 2 – Implementação do Amazon SQS

**Foco da ferramenta:**  
Serviço de filas totalmente gerenciado para desacoplamento de aplicações.

**Caso de uso:**  
Os sistemas internos da empresa possuíam comunicação direta entre serviços, o que causava:

- Sobrecarga em momentos de pico
- Quedas em cascata
- Necessidade de superdimensionamento de servidores

Com a implementação do Amazon SQS:

- Os serviços passaram a se comunicar de forma assíncrona
- Foi possível absorver picos de demanda sem aumentar infraestrutura
- Reduziu-se a necessidade de instâncias superdimensionadas

**Impacto na redução de custos:**  
Menor necessidade de provisionamento excessivo de recursos computacionais, reduzindo custos com servidores e melhorando estabilidade.

---

### Etapa 3 – Implementação do Amazon SNS

**Foco da ferramenta:**  
Serviço de notificação e comunicação distribuída.

**Caso de uso:**  
Antes da implementação, sistemas utilizavam chamadas diretas para enviar notificações, gerando:

- Maior consumo de processamento
- Acoplamento entre aplicações
- Complexidade na manutenção

Com o Amazon SNS:

- Notificações passaram a ser publicadas em tópicos
- Múltiplos sistemas puderam se inscrever nesses tópicos
- Reduziu-se a complexidade arquitetural

**Impacto na redução de custos:**

- Menor consumo de recursos computacionais
- Redução de retrabalho técnico
- Melhor escalabilidade sem aumento proporcional de custos

---

## Benefícios Gerais da Implementação

- Arquitetura desacoplada
- Maior escalabilidade
- Alta disponibilidade
- Modelo de pagamento sob demanda
- Redução de custos com infraestrutura física
- Otimização de recursos computacionais

---

## Conclusão

A implementação dos serviços Amazon S3, Amazon SQS e Amazon SNS permitiu à Abstergo Industries reduzir custos imediatos relacionados à infraestrutura física e superdimensionamento de recursos.

Além da redução financeira, houve ganho significativo em:

- Escalabilidade
- Resiliência
- Organização arquitetural
- Produtividade da equipe técnica

Recomenda-se a continuidade da estratégia de modernização da infraestrutura com foco em serviços gerenciados e arquitetura baseada em microsserviços.

---

## Anexos

- Diagramas de arquitetura
- Planilha de estimativa de custos comparativos
- Documentação técnica de configuração

---

Assinatura do Responsável pelo Projeto:

Riosberg Dutra dos Santos