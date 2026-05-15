
## O que é?
Recurso que permite criar e gerenciar um **grupo de VMs idênticas** com capacidade de escalonamento automático (autoscaling).

## Como funciona
- Você define uma **imagem base** e uma **configuração de VM**
- O Azure cria múltiplas instâncias iguais automaticamente
- Um **balanceador de carga** distribui o tráfego entre as instâncias
- Escala **para cima** (mais VMs) quando a demanda aumenta
- Escala **para baixo** (menos VMs) quando a demanda cai

## Benefícios
- **Alta disponibilidade:** VMs distribuídas em múltiplas zonas/fault domains
- **Gerenciamento centralizado:** atualiza todas as instâncias de uma vez
- **Economia:** paga apenas pelo que usa — escala reduz VMs ociosas
- **Elasticidade:** responde automaticamente à carga (CPU, memória, fila...)

## Escalonamento
| Tipo | Descrição |
|---|---|
| **Manual** | Você define o número de instâncias manualmente |
| **Automático (Autoscale)** | Azure ajusta baseado em métricas (CPU > 70% → adiciona VMs) |
| **Agendado** | Escala em horários predefinidos |

## Diferença entre VMSS e VM comum
| VM comum | VMSS |
|---|---|
| Uma instância | Múltiplas instâncias idênticas |
| Escala manual | Escala automática |
| Sem LB integrado | Load Balancer incluso |

## Casos de uso
- Sites com tráfego variável
- Processamento em lote (batch jobs)
- Aplicações que precisam de alta disponibilidade