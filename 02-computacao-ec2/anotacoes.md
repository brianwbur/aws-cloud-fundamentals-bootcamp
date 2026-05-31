# Anotações - Computação com Amazon EC2

## Amazon EC2

O Amazon EC2 (Elastic Compute Cloud) é o serviço de máquinas virtuais da AWS.

Ele permite criar servidores na nuvem sob demanda, escolhendo recursos como CPU, memória, armazenamento e sistema operacional.

### Palavras-chave

* Máquina virtual
* Servidor
* Computação
* Escalabilidade
* Alta disponibilidade

---

## Tipos de Compra de Instâncias

### On-Demand

Pagamento somente pelo tempo utilizado.

Ideal para:

* Testes
* Ambientes temporários
* Cargas imprevisíveis

### Reserved Instances

Desconto em troca de compromisso de uso por um período.

Ideal para:

* Ambientes estáveis
* Uso contínuo
* Longo prazo

### Spot Instances

Utilizam capacidade ociosa da AWS.

Vantagem:

* Grande economia

Desvantagem:

* Podem ser interrompidas pela AWS

---

## Amazon EBS

Serviço de armazenamento em bloco utilizado pelas instâncias EC2.

Funciona como um disco rígido conectado ao servidor.

### Palavras-chave

* Disco virtual
* Armazenamento em bloco
* Persistência
* Snapshot

---

## Elastic Load Balancer (ELB)

Distribui automaticamente o tráfego entre múltiplas instâncias.

Benefícios:

* Alta disponibilidade
* Balanceamento de carga
* Melhor utilização dos recursos

### Associação rápida

"Distribuir tráfego"

→ ELB

---

## Auto Scaling

Permite aumentar ou reduzir automaticamente a quantidade de instâncias conforme a demanda.

Benefícios:

* Economia de custos
* Melhor desempenho
* Elasticidade

### Associação rápida

"Adicionar ou remover instâncias automaticamente"

→ Auto Scaling

---

## Amazon CloudWatch

Serviço de monitoramento da AWS.

Permite acompanhar métricas e criar alarmes.

Exemplos:

* Uso de CPU
* Rede
* Disco
* Logs

### Associação rápida

"Monitoramento e métricas"

→ CloudWatch

---

## Escalabilidade

### Vertical

Aumentar os recursos da mesma máquina.

Exemplo:

t3.micro → t3.large

### Horizontal

Adicionar mais instâncias.

Exemplo:

1 EC2 → 5 EC2

---

## Alta Disponibilidade

Consiste em distribuir recursos entre múltiplas Zonas de Disponibilidade para reduzir impactos de falhas.

### Exemplos

EC2 + ELB + Multi-AZ

→ Active-Active

RDS Multi-AZ

→ Active-Passive

---

## Resumo para Certificação

CPU alta

→ CloudWatch

Disco da EC2

→ EBS

Distribuir tráfego

→ ELB

Escalar automaticamente

→ Auto Scaling

Economia com interrupção aceitável

→ Spot Instances

Servidor virtual na AWS

→ EC2
