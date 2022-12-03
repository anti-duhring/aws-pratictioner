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