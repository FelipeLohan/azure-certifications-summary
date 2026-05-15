
## O que é?
Emulação de um computador físico na nuvem. Modelo **IaaS** (Infrastructure as a Service).

## Responsabilidades
- **Você gerencia:** SO, patches, runtimes, aplicações, dados
- **Azure gerencia:** hardware, rede física, datacenter

## Componentes principais
- **Imagem:** SO base (Windows Server, Ubuntu, Red Hat, etc.)
- **Tamanho (SKU):** define vCPUs, memória RAM e disco
- **Região:** datacenter onde a VM será hospedada
- **Disco:** OS Disk (obrigatório) + Data Disks (opcionais)
- **VNet/NIC:** conectividade de rede
- **NSG:** regras de firewall (Network Security Group)

## Casos de uso (importantes no exame)
- **Lift-and-shift:** migrar aplicações on-premises sem reescrever código
- **Controle total do SO:** quando é necessário customizar o sistema operacional
- **Ambientes de teste/dev:** criar e destruir ambientes rapidamente
- **Alta disponibilidade:** usar Availability Zones ou Availability Sets

## Alta Disponibilidade
| Recurso | O que faz |
|---|---|
| **Availability Set** | Distribui VMs em fault domains e update domains no mesmo datacenter |
| **Availability Zone** | Distribui VMs em datacenters fisicamente separados na mesma região |

## Modelos de preço
- **Pay-as-you-go:** paga pelo tempo ligado
- **Reserved Instances:** desconto em troca de compromisso de 1 ou 3 anos
- **Spot VMs:** capacidade sobressalente com grande desconto (pode ser interrompida)
