
## O que é?
Serviço gerenciado de **orquestração de containers** baseado no Kubernetes. Automatiza implantação, escalonamento e operação de containers em produção.

## O que o Kubernetes faz?
- **Orquestra** múltiplos containers em um cluster de nós
- **Balanceia carga** entre instâncias de containers
- **Reinicia** containers com falha automaticamente
- **Escala** aplicações baseado na demanda
- **Gerencia** atualizações com zero downtime (rolling updates)

## Conceitos básicos do K8s (para o exame)
| Conceito | Descrição |
|---|---|
| **Node** | VM que executa containers |
| **Pod** | Menor unidade — um ou mais containers |
| **Cluster** | Conjunto de nodes gerenciados pelo control plane |
| **Deployment** | Define quantas réplicas de um pod devem existir |
| **Service** | Expõe pods para a rede (interno ou externo) |

## AKS vs ACI
| | ACI | AKS |
|---|---|---|
| Complexidade | Simples | Mais complexo |
| Orquestração | Não | Sim (Kubernetes) |
| Casos de uso | Tarefas isoladas | Apps em produção, microsserviços |
| Escalonamento | Básico | Avançado e automático |

## Responsabilidades no AKS
- **Você gerencia:** aplicações, configurações, pods, deployments
- **Azure gerencia:** control plane do Kubernetes (gratuito), upgrades do cluster, monitoramento base

## Ponto-chave para o exame
> AKS é a escolha quando você precisa de **orquestração de containers em escala** com alta disponibilidade e microsserviços.
