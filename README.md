# Arquitetura Microsoft Azure
Documento com foco em explicar os principais conceitos da arquitetura do Microsoft Azure,com o intuito de enteender a  infraestrutura global.
## Regiões e Zonas de Disponibilidade

### Regiões Azure
- Conjuntos de datacenters conectados por rede com baixa latência 
- Exemplos: Brazil South, East US
- Nem todos os serviços estão disponíveis em todas as regiões

### Zonas de Disponibilidade
- Datacenters fisicamente separados dentro de uma mesma região.
- Oferecem tolerância a falhas (cada zona tem energia, resfriamento e rede independentes).

##  Resiliência e Pares de Região

### Pares de Região
- Regiões emparelhadas ou seja com distância superior a 300 milhas.
Funcionalidades -> Replicação automática para serviços como:
    - Azure Storage
    - SQL Database
  - Priorização de recuperação em desastres técnicos.

### Backbone Global
- Rede privada de alta velocidade.
- Conecta todos os datacenters Azure.
- Reduz latência para dados críticos.

##  Conformidade e Segurança
Residência de Dados:
- Os dados ficam em uma região.
- Atendimento a regulamentações(LGPD, GDPR). 
- Opções de regiões locais(ex:Brasil para dados brasileiros). 

### Regiões Especiais
| Região | Acesso |
|--------|--------|
| Azure China | Restrito |
| Azure Government (EUA) | Autorização necessária |

### Governança e Gerenciamento
- Assinaturas(Subscriptions).
- Unidade básica de cobrança e isolamento de recursos.
- Permitem refinar custos por equipe ou projeto.
Grupos de Recursos(Resource Groups):
- Contêineres lógicos que agrupam recursos relacionados.
- Facilitam o gerenciamento e a aplicação de políticas.
