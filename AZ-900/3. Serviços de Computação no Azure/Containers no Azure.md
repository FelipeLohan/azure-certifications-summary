
## O que é um container?
Unidade leve e portátil que **empacota código + dependências** para rodar de forma consistente em qualquer ambiente.

## Diferença: VM vs Container
| | VM | Container |
|---|---|---|
| Inclui | SO completo | Apenas app + libs |
| Peso | Gigabytes | Megabytes |
| Inicialização | Minutos | Segundos |
| Isolamento | Forte (hypervisor) | Moderado (kernel compartilhado) |

## Serviços de container no Azure

### Azure Container Instances (ACI)
- Forma mais **simples e rápida** de executar containers no Azure
- Modelo **serverless** — sem gerenciar VMs ou clusters
- Ideal para: tarefas isoladas, builds, testes, scripts agendados
- Cobrança por **segundos de uso**
- Suporta containers Linux e Windows

### Azure Container Registry (ACR)
- **Repositório privado** de imagens Docker no Azure
- Armazena e gerencia imagens de containers
- Integra com ACI, AKS, App Service
- Similar ao Docker Hub, mas privado e integrado ao ecossistema Azure

## Ponto-chave para o exame
- **ACI** = rodar containers **sem infraestrutura** (serverless, simples, rápido)
- **AKS** = orquestrar **muitos containers** (veja o tópico de Kubernetes)
- **ACR** = **armazenar** imagens de containers
