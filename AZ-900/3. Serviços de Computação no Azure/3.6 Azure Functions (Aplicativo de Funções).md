
## O que é?
Serviço **serverless** (sem servidor) que permite executar pequenos trechos de código (funções) em resposta a eventos, **sem gerenciar infraestrutura**.

## Modelo Serverless
- Você escreve apenas o **código da função**
- Azure gerencia **tudo mais**: servidores, SO, escalonamento, disponibilidade
- Cobrança por **execução** — paga apenas quando a função roda (e pelo tempo de execução)
- Escalonamento **automático** — de zero a milhares de instâncias

## Triggers (gatilhos) — o que dispara uma função
| Trigger | Quando dispara |
|---|---|
| **HTTP** | Requisição web (como uma API) |
| **Timer** | Em intervalos agendados (tipo cron job) |
| **Blob Storage** | Quando um arquivo é adicionado ao storage |
| **Queue Storage** | Quando uma mensagem chega na fila |
| **Event Hub / Service Bus** | Mensagens de sistemas de eventos |
| **Cosmos DB** | Mudanças no banco de dados |

## Planos de hospedagem
| Plano | Característica |
|---|---|
| **Consumption (Consumo)** | Paga por execução, escala automática, cold start possível |
| **Premium** | Sem cold start, VNet integration, instâncias pré-aquecidas |
| **Dedicated (App Service)** | Roda no seu App Service Plan existente |

## Comparação: Functions vs App Service vs Containers
| | Functions | App Service | Containers |
|---|---|---|---|
| Modelo | Serverless | PaaS | PaaS/IaaS |
| Unidade | Função (evento) | Aplicação web | Container |
| Escala | Automática por evento | Manual/auto | Manual/auto |
| Ideal para | Tarefas pontuais | Apps web | Microsserviços |

## Linguagens suportadas
C#, JavaScript/TypeScript, Python, Java, PowerShell, Go (custom handler)

## Ponto-chave para o exame
> Azure Functions é **serverless** — você paga por execução, não por servidor ligado. Ideal para tarefas acionadas por eventos, automações e APIs leves.
