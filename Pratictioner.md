# O que é cloud computing
    -> Consumidor (empresa que contrata o serviço da Cloud Provider) se conecta remotamente com os servidores, via um serviço, que é prestado pela Cloud Provider, e que cuida da infraestrutura, armazenamento e manutenção das máquinas.
    
    -> Pagamento por segundo de utilização

# Benefícios
    -> Velocidade em solucionar os problemas e satisfazer a demanda
    
    -> Atualizações são feitas sem interromper o serviço e de forma automática, feita pela própria Cloud Provider
    
    -> Custo baixo e contratos personalizados
    
    -> Data security
        -> Backups são automáticos
        
        -> Não é necessário se preocupar com as máquinas dos servidores
    
    -> Scalability
        -> Pode ser configurada para ser feita automaticamente
        
        -> Se for configurada pra ser manual, pode ser feita em segundas

# Tipos de cloud 
## IaaS - Infrastructure-As-A-Service
    -> Cloud Provider fica responsável por gerenciar toda a estrutura, o resto é responsabilidade do consumidor

    -> Ex: AWS - EC2
    
    -> Responsabilidade do consumidor:
        1. Applications
        2. Data
        3. Runtime
        4. Middleware
        5. O/S
    
    -> Responsabilidade da Cloud Provider:
        1. Virtualization
        2. Servers
        3. Storage
        4. Networking
    
## PaaS - Plataform-As-A-Service
    -> Engloba também o IaaS
    
    -> Cloud Provider fica responsável também por gerenciar a plataforma, a aplicação é responsabilidade do consumidor

    -> Ex: Benstalk

    -> Responsabilidade do consumidor:
        1. Applications
        2. Data
    
    -> Responsabilidade da Cloud Provider:
        1. Runtime
        2. Middleware
        3. O/S
        4. Virtualization
        5. Servers
        6. Storage
        7. Networking
    
## SaaS - Software-As-A-Service
    -> Engloba também o PaaS
    
    -> Cloud Provider gerencia também a aplicação

    -> Ex: CRM, Office 365, Google Docs e etc
    
    -> Responsabilidade da Cloud Provider:
        1. Applications
        2. Data
        3. Runtime
        4. Middleware
        5. O/S
        6. Virtualization
        7. Servers
        8. Storage
        9. Networking

# Tipos de rede
## Public Cloud
    -> Oferecido pelos Cloud Providers
    -> Disponível para qualquer pessoa na internet
    -> Possui escalabilidade rápida
    -> Também possui camadas de segurança
    -> Um pouco mais barato

## Private Cloud
    -> Oferecido pelos Cloud Providers
    -> Disponível para qualquer pessoa na internet ou uma rede inter privada
    -> Possui grande controle de segurança, já que o servidor está fisicamente separado
    -> Requer um custo maior de manutenção
    -> Ex: U.S Gov.

## Hybrid Cloud
    -> Combinação do público e do provado
        -> Ex: App na nuvem pública e DB na nuvem privada
    
# Serviços da AWS
    -> Qualquer coisa que seja necessária iniciar, configurar ou finalizar a AWS considera como serviço
    -> Ex: EC2 é o nome do serviço de storage no servidor
    -> Ex: Route53 é o nome do serviço de compra de domínio
    -> [https://aws.amazon.com/products/](Lista dos serviços)

# Shared Responsability Model
    -> Quase como um ato de parenting (ser mãe e pai)
    -> [https://aws.amazon.com/compliance/shared-responsibility-model/](Shared responsability model da AWS)
    -> Ao abrir a conta na AWS você aceita o Shared Responsability Model, acordando que a própria Cloud Provider não será a única responsável pela segurança, já que o consumidor também terá suas próprias responsabilidades
        -> Pode variar conforme o serviço prestado
            -> Ex: Um serviço como o Amazon Elastic Compute Cloud (Amazon EC2) é categorizado como Infrastructure as a Service (IaaS – Infraestrutura como serviço) e, dessa forma, exige que o cliente execute todas as tarefas necessárias de configuração e gerenciamento da segurança.
    -> Divisão:
        -> AWS: Responsável pela segurança da cloud
            -> Segurança do software -> Compute, storage, database e networking
            -> Segurança do harware e infraestrutura global -> Regions, avaliability zones e edge locations
        -> Consumidor: Responsável pela segurança dentro da cloud
            -> Segurança da customer data
            -> Segurança da plataform, applications, identity e gerenciamento do acesso
            -> Segurança do sistema operacional, network e configuração de firewall
            -> Criptografia dos dados do cliente e autenticação dos dados
            -> Criptografia do server-side, tanto de dados quanto de arquivos
            -> Proteção do networking traffic

# CLI e CloudShell
## CLI
    -> Command Line Interface
    -> Um terminal
    -> Pode ser instalado localmente

## CLoudshell
    -> Também é uma CLI, mas na cloud

## Conteúdo
    -> É possível visualizar, implementar, configurar e etc os serviços da AWS via console, CLI e CloudShell
    -> Os buckets da nuvem da AWS, bem como os seus serviços, podem ser accessados de 3 formas:
        -> Via console: https://us-east-1.console.aws.amazon.com/
        -> Via CLI
        -> Via CloudShell: https://us-east-1.console.aws.amazon.com/cloudshell/home?region=us-east-1#

# Regiões
    -> Região: áreas que disponibilizam serviços, cada área pode disponibilizar alguns serviços e não outros.
    -> Códigos: US, AP, EU, SA, CA, ME e AF
        -> Se está nos EUA, começa com US
            -> Ex: us-east-2
            -> US é o código da região, east é a área e 2 significa que é a segunda região dessa área
        -> Ásia-pacífico com AP
        -> Europa com EU
        -> América do SUl começa com SA
            -> EX: sa-east-1
        -> Canadá com CA
        -> Oriente Médio com ME
        -> África AF
    
# Zonas de disponibilidade (AZ)
    -> São os conteúdos dentro das regiões
    -> Ex: Quantos datacenters existem na região us-east-2? 
        -> us-east-2a
        -> us-east-2b
        -> us-east-2c
    -> AZ (Avaliability Zones ou Zonas de Disponibilidade) são o aglomerado (ou único) datacenters disponíveis em uma região da AWS
    -> Possuem links de conexão entre todas as AZ dentro da região pra diminuir a latência
        -> São fisicamente separadas por vários até 100km entre si
        -> Alta largura de banda
    -> Os serviços contratados pelos consumidores são dispersos entre todas as AZ para evitar que a falha de uma afete o serviço consumido
    -> Funções das AZ:
        -> Aumentar a disponibilidade de serviços
        -> Ser um backup uma das outras
    
# Zona local (LZ)
    -> Filho das AZs
    -> Datacenters menores pra aproximar os serviços da AWS aos usuários finais, diminuindo a latência

# Wavelength
    -> Permite aos desenvolvedores criar apps com latência inferior a 10ms pra dispositivo móvel e usuário final
    -> AWS coloca as próprias máquinas dentro das provedoras de telefonia pra melhorar a conexão (fast speed) com a AZ

# Outposts
    -> A AWS coloca seus próprios equipamentos de conexão rápida dentro de datacenters de terceiros (empresas ou etc)

# Identity and Access Management (IAM)
    -> São filtros de segurança por onde é possível chegar via autenticação (Console, CLI ou API) e concentra a execução das ações da conta, como criar e gerenciar users, groups, roles, apps e etc e a partir disso criar e as políticas (IBP ou RBP)
        -> IBP: Identity Based Policy
        -> RBP: Resource Based Polcy
        -> Com essas políticas é possível ter acesso aos serviços (criar maquina virtual, uma bucket, um EC2 e etc)
    -> Evita que os usuários tenham acesso direto aos serviços
    -> Todas as interações dos serviços da AWS são APIs
    -> Formas de acesso:
        -> Console: O usuário precisa fornecer o usuário, senha e a MFA(Multi Factor Authentication - opcional)
        -> CLI e API: Com a access key e secret key
## Usuários
    -> É uma das coisas possíveis de se criar no IAM
    -> O usuário pode acessar a plataforma via Console, CLI ou API
    -> É preciso configurar suas permissões (0 priviéglios por padrão)
## Grupos
    -> Organiza os usuários
    -> Ex: Agrupar usuários com o mesmo privilégio
## Roles
    -> São aplicadas a serviços da AWS
    -> Ex: Uma instância EC2, ou uma VM, possa criar uma bucket
## Policy
    -> Regras para permitir ou bloquear acessos de grupos ou usuários
    -> Ex: Grupo A só pode fazer uploads na Bucket X
## MFA (Multi Factor Authentication)
    -> Uma forma de autenticação em 2 fatores

# EC2 (Elastic Compute Cloud)
    -> EC2 (Elastic Compute Cloud) é a virtualização da AWS
## Virtualização 
    -> Máquina virtual -> Instância (pedaço de uma virtualização)
    -> É a camada que vai por cima do hardware que comporta vários SOs
    -> É possível alocar repartições da memória, CPU e etc pra cada SO7
    -> AWS usa a Xen Virtualization
## Vantagens
    -> Controle completo da instância
        -> Ex: Configurações, alocação de memória e etc
    -> Security:
        -> A máquina virtual só pode ser acessada pela key cadastrada
        -> Há um firewall configurado por default que pode ser modificado
    -> Integrado com os outros serviços da AWS
    -> Low cost
    -> Uncomplicated