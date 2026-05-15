Um **Resource Group (RG)** é um contêiner lógico onde você agrupa os recursos da Azure (como Máquinas Virtuais, Bancos de Dados SQL, Redes Virtuais e Contas de Armazenamento).

### Características Principais:

- **Ciclo de Vida Único:** Geralmente, recursos em um mesmo RG compartilham o mesmo ciclo de vida. Se você deletar o Grupo de Recursos, todos os recursos dentro dele serão excluídos simultaneamente.

- **Agrupamento Lógico:** Serve para organizar recursos por ambiente (ex: Produção, Homologação), por projeto ou por departamento.

- **Localização do Metadados:** Embora o grupo de recursos tenha uma localização (ex: East US), os recursos dentro dele podem estar em regiões diferentes. O RG armazena apenas os **metadados** (as configurações) sobre esses recursos.

- **RBAC (Controle de Acesso):** Você pode aplicar permissões de acesso diretamente no nível do Grupo de Recursos, e todos os itens dentro dele herdarão essas permissões.