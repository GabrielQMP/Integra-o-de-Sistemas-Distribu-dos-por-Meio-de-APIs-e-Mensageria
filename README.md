# 🔬 Integração de Sistemas Distribuídos por Meio de APIs e Mensageria

## 📚 Sobre a pesquisa

Este projeto apresenta uma pesquisa científica sobre mecanismos de integração em sistemas distribuídos, com foco na comparação entre comunicação síncrona utilizando APIs REST e comunicação assíncrona utilizando RabbitMQ.

O estudo busca analisar como essas abordagens se comportam em diferentes condições de execução, considerando aspectos como desempenho, tempo de resposta, utilização de recursos e tolerância a falhas.

## 🎯 Objetivo

Comparar experimentalmente os mecanismos de integração síncrona, por meio de APIs REST, e assíncrona, por meio do RabbitMQ, avaliando suas características, vantagens, limitações e comportamento diante de diferentes condições de carga e indisponibilidade de serviços.

## 🛠️ Tecnologias utilizadas

- **Node.js:** ambiente de execução da aplicação.
- **TypeScript:** desenvolvimento dos serviços.
- **Fastify:** construção das APIs.
- **RabbitMQ:** gerenciamento e processamento de mensagens.
- **PostgreSQL:** armazenamento dos dados.
- **Prisma ORM:** comunicação com o banco de dados.
- **Docker:** configuração e execução do ambiente experimental.
- **k6:** execução dos testes de carga.

## 🧪 Metodologia

Foram desenvolvidos dois cenários de integração para comparação:

- **REST (Síncrono):** comunicação direta entre os serviços por meio de requisições e respostas.
- **RabbitMQ (Assíncrono):** comunicação intermediada por filas de mensagens, permitindo desacoplamento entre o recebimento e o processamento das solicitações.

Os experimentos foram organizados em diferentes cenários:

1. Teste de carga baixa.
2. Teste de carga crescente.
3. Teste de pico de carga.
4. Teste de falha do serviço de processamento.
5. Teste exploratório de limite.
6. Análise da utilização de recursos computacionais.

## 📊 Principais resultados

Os experimentos demonstraram que as duas abordagens apresentam vantagens e limitações, dependendo das necessidades do sistema.

- **REST:** apresentou menor tempo de processamento em determinados cenários e comunicação direta entre os serviços.
- **RabbitMQ:** apresentou maior capacidade de absorver indisponibilidades temporárias do serviço de processamento, mantendo as mensagens em fila.
- **Tolerância a falhas:** durante a interrupção do serviço de processamento, o cenário REST apresentou aproximadamente 33,79% de erros nas requisições, enquanto o RabbitMQ não apresentou erros para o cliente e conseguiu registrar todas as solicitações recebidas.

Os resultados indicam que a escolha da arquitetura deve considerar os requisitos de desempenho, disponibilidade e tolerância a falhas de cada aplicação.

## 📁 Organização do repositório

- `Artigo-cientifico.pdf` — documento completo da pesquisa.
- `codigos/` — implementação dos serviços e dos mecanismos de integração.
- `resultados/` — dados e resultados dos experimentos.
- `diagramas/` — representações da arquitetura utilizada.

*Os diretórios e arquivos serão disponibilizados conforme a organização dos materiais da pesquisa.*

## 🎓 Instituição

Centro Universitário Impacta  
São Paulo – SP  
Novembro de 2026

**Orientador:** Professor Me. Gilberto Alves Pereira.

## 👨‍💻 Participação

**Gabriel Quaglio Monteiro Praça**

Estudante de Sistemas de Informação, com participação no desenvolvimento de uma pesquisa científica voltada à integração de sistemas distribuídos, arquitetura de software e análise experimental de desempenho.

## 🔗 Contato

- [GitHub](https://github.com/GabrielOMP)

---

*Projeto acadêmico desenvolvido em grupo no contexto de iniciação científica.*
