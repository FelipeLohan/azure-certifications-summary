
## O que é?
Serviço **PaaS** (Platform as a Service) para hospedar aplicações web, APIs REST e back-ends móveis **sem gerenciar a infraestrutura**.

## Modelos de aplicação suportados
- **Web Apps** — aplicações web (ASP.NET, Node.js, Python, PHP, Java, Ruby)
- **API Apps** — APIs RESTful
- **Mobile Apps** — back-end para apps móveis
- **WebJobs** — tarefas em segundo plano (scripts, executáveis)

## Planos de serviço (App Service Plan)
Define o tamanho e os recursos da infraestrutura subjacente:

**Free / Shared**: Testes e desenvolvimento 
**Basic**: Apps de baixo tráfego sem SLA 
**Standard**: Apps de produção com autoscaling 
**Premium**: Alta performance, VNet integration 
**Isolated**: App Service Environment (ASE) — rede dedicada 

## Responsabilidades (PaaS)
- **Você gerencia:** código, configurações, dados
- **Azure gerencia:** SO, patches, servidores, rede, balanceamento de carga

## Recursos importantes
- **Autoscaling** integrado (no plano Standard+)
- **Slots de implantação (Deployment Slots):** ambientes separados (staging, produção) com troca sem downtime (swap)
- **Domínio personalizado + SSL** integrado
- **CI/CD** integrado com GitHub, Azure DevOps, Bitbucket
- **Diagnóstico e monitoramento** com Application Insights

## Ponto-chave para o exame
> App Service é **PaaS** — você foca no código, Azure cuida do resto. Não é necessário gerenciar o sistema operacional.