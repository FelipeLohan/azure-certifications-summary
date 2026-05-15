
## O que são?
Ferramentas de linha de comando para gerenciar recursos do Azure.

## Azure CLI
- Interface de linha de comando **multiplataforma** (Windows, Linux, macOS)
- Comandos no formato: `az [grupo] [subgrupo] [ação]`
- Exemplo: `az vm create --name minhaVM --resource-group meuGrupo`
- Linguagem: **Bash / scripts shell**

## Azure PowerShell
- Módulo PowerShell chamado **Az**
- Ideal para quem já usa PowerShell no Windows
- Comandos no formato: `Verb-AzNoun`
- Exemplo: `New-AzVM -Name minhaVM -ResourceGroupName meuGrupo`
- Linguagem: **PowerShell**

## Azure Cloud Shell
- Shell **no navegador**, acessível pelo portal Azure (portal.azure.com)
- Suporta **Bash (CLI)** e **PowerShell** — escolha na hora de abrir
- Não precisa instalar nada localmente
- Armazenamento: usa um **Azure File Share** para persistir arquivos entre sessões
- Acesso: portal Azure, shell.azure.com, app mobile, VS Code

## Diferenças importantes para o exame
|                       | CLI                 | PowerShell          | Cloud Shell |
| --------------------- | ------------------- | ------------------- | ----------- |
| Onde roda             | Local / Cloud Shell | Local / Cloud Shell | Navegador   |
| Sintaxe               | `az ...`            | `Az-...`            | Ambas       |
| Multiplataforma       | ✅                   | ✅ (módulo Az)       | ✅           |
| Instalação necessária | Sim (local)         | Sim (local)         | ❌           |

## Ponto-chave
> Todas as três ferramentas executam os **mesmos resultados** — são apenas formas diferentes de interagir com a API do Azure. O que uma faz, as outras também fazem.
