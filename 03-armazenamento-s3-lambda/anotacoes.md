# Anotações - Amazon S3 e AWS Lambda

## Amazon S3

O Amazon S3 (Simple Storage Service) é o serviço de armazenamento de objetos da AWS.

Ele é utilizado para armazenar arquivos como:

* Imagens
* Vídeos
* Documentos
* Backups
* Logs

### Palavras-chave

* Objetos
* Bucket
* Armazenamento
* Backup
* Escalabilidade

### Associação rápida

Arquivos, imagens, vídeos e documentos

→ Amazon S3

---

## Bucket

Um Bucket funciona como um contêiner onde os objetos são armazenados.

Todo arquivo enviado ao S3 fica dentro de um Bucket.

### Associação rápida

Local onde os arquivos ficam armazenados

→ Bucket

---

## Características do Amazon S3

* Alta durabilidade
* Alta disponibilidade
* Escalabilidade automática
* Baixo custo
* Armazenamento praticamente ilimitado

---

## AWS Lambda

AWS Lambda é um serviço Serverless que executa código sem necessidade de gerenciar servidores.

O desenvolvedor envia apenas o código e a AWS cuida da infraestrutura.

### Palavras-chave

* Serverless
* Eventos
* Automação
* Função
* Execução sob demanda

### Associação rápida

Executar código sem gerenciar servidores

→ AWS Lambda

---

## O que é Serverless?

Serverless significa que não precisamos criar, atualizar ou administrar servidores.

A AWS gerencia toda a infraestrutura.

O foco fica apenas no desenvolvimento da aplicação.

### Associação rápida

Sem gerenciamento de servidores

→ Serverless

---

## EC2 x Lambda

### Amazon EC2

* Você gerencia o servidor
* Instância fica ativa
* Maior controle da infraestrutura

### AWS Lambda

* Não gerencia servidores
* Executa sob demanda
* Cobra apenas pela execução

### Associação rápida

Precisa administrar servidor

→ EC2

Não quer administrar servidor

→ Lambda

---

## Arquitetura comum

Usuário → S3 → Lambda

Exemplo:

1. Usuário envia um arquivo para um Bucket S3.
2. O S3 gera um evento.
3. O evento aciona uma função Lambda.
4. A Lambda processa o arquivo automaticamente.

---

## Resumo para Certificação

Armazenamento de objetos

→ Amazon S3

Contêiner de armazenamento

→ Bucket

Executar código sem servidor

→ AWS Lambda

Sem gerenciar infraestrutura

→ Serverless

Processamento baseado em eventos

→ AWS Lambda

Upload de arquivos

→ Amazon S3
