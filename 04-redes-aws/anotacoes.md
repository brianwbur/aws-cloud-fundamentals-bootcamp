# Anotações - Redes na AWS

## Amazon VPC

Amazon VPC (Virtual Private Cloud) é uma rede virtual isolada dentro da AWS.

Ela permite criar e controlar recursos de rede como:

* Subnets
* Tabelas de rotas
* Gateways
* Security Groups

### Palavras-chave

* Rede virtual
* Isolamento
* Controle de rede
* Segmentação

### Associação rápida

Criar uma rede privada na AWS

→ Amazon VPC

---

## Amazon Subnet

Uma Subnet é uma divisão lógica dentro de uma VPC.

Cada Subnet pertence a apenas uma Zona de Disponibilidade.

### Tipos

### Pública

Possui acesso à internet.

### Privada

Sem acesso direto à internet.

### Associação rápida

Divisão da VPC

→ Subnet

---

## Security Group

Funciona como um firewall virtual para recursos da AWS.

Controla:

* Tráfego de entrada (Inbound)
* Tráfego de saída (Outbound)

Características:

* Stateful
* Permite regras específicas por porta e protocolo

### Associação rápida

Firewall da instância

→ Security Group

---

## Amazon Route 53

Serviço DNS gerenciado da AWS.

Responsável por:

* Registro de domínios
* Resolução de nomes
* Roteamento de tráfego

### Associação rápida

DNS da AWS

→ Route 53

---

## Amazon CloudFront

Serviço CDN (Content Delivery Network) da AWS.

Distribui conteúdo utilizando Edge Locations espalhadas pelo mundo.

Benefícios:

* Menor latência
* Melhor desempenho
* Distribuição global

### Associação rápida

Distribuição de conteúdo global

→ CloudFront

---

## Elastic Load Balancer (ELB)

Distribui o tráfego entre múltiplas instâncias.

Benefícios:

* Alta disponibilidade
* Escalabilidade
* Balanceamento de carga

### Associação rápida

Distribuir tráfego

→ Elastic Load Balancer

---

## Tipos de Load Balancer

### Application Load Balancer (ALB)

Camada 7

Trabalha com:

* HTTP
* HTTPS

Ideal para aplicações web.

---

### Network Load Balancer (NLB)

Camada 4

Trabalha com:

* TCP
* UDP

Ideal para alta performance.

---

### Gateway Load Balancer (GWLB)

Integra appliances virtuais de segurança.

Exemplos:

* Firewalls
* IDS/IPS

---

## Relação entre os Serviços

```text
Usuário
   │
Route 53
   │
CloudFront
   │
Load Balancer
   │
EC2
```

---

## Resumo para Certificação

Rede privada na AWS

→ VPC

Divisão da VPC

→ Subnet

Firewall da instância

→ Security Group

DNS da AWS

→ Route 53

CDN da AWS

→ CloudFront

Distribuir tráfego

→ Elastic Load Balancer

Alta disponibilidade

→ Multi-AZ + ELB

Filtrar tráfego web

→ AWS WAF

Ataques DDoS

→ AWS Shield
