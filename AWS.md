# Resumo de AWS

1. O que é computação em nuvem
Entrega sob demanda de computação, banco de dados, armazenamento, aplicativos e outros recursos de TI por meio de uma plataforma de serviços em nuvem via Internet com preços pré-pagos.
Infraestrutura do AWS – 
As três principais categorias de computação são máquinas virtuais (VMs), contêineres e computação sem servidor
3 tipos de computação em nuvem
Infraestrutura como serviço (IAAS)
Você gerencia o servidor, que pode ser físico ou virtual, bem como o sistema operacional
Plataforma como serviço (PAAS)
Outra pessoa gerencia o hardware e os sistemas subjacentes, você apenas se concentra em seus aplicativos, outra pessoa se preocupa com segurança, aplicação de patches, atualizações, manutenção e etc.
Software como serviço (SAAS)
Pense no Outlook. Você se preocupa em como usar o software, o resto é terceirizado.
3 tipos de implantações de computação em nuvem
Nuvem pública (Cloud-based) - AWS, Azure, GCP
Híbrido (Hybrid) - mistura público e privado
Nuvem privada (on-premises) - você gerencia o datacenter
6 vantagens da computação em nuvem
1 – Mudar de despesa de capital para despesa variável. Pagar conforme o uso.
2 – Enormes economias de escala
3 – Parar de adivinhar a capacidade
4 – Aumentar velocidade e agilidade
5 – Parar de gastar dinheiro executando e mantendo datacenter
6 – Tornar-se global
2. Região X Zona de Disponibilidade X Edge Location
Região - é uma localização física on globo que consiste em três ou mais zonas de disponibilidade.
AZ - formação de um ou mais datacenter em que cada um tem energia redundante, rede e conectividade entre si, e pelo menos 100km de distância um do outro
Edge Locations - são endpoints para a AWS usados para cache e conteúdo. Consiste no serviço de CloudFront, que é o CDN da AWS.
3. Amazon Virtual Private Cloud (Amazon VPC)
Um serviço de rede que você pode usar para estabelecer limites em torno de seus recursos da AWS.
Permite que você provisione uma seção isolada da Nuvem AWS. Nesta seção isolada, você pode iniciar recursos em uma rede virtual que você define. Dentro de uma nuvem privada virtual (VPC), você pode organizar seus recursos em sub-redes. Uma sub-rede é uma seção de uma VPC que pode conter recursos como instâncias do Amazon EC2.
Ao criar uma Amazon VPC, você deve escolher três fatores principais:
Nome da VPC
Região onde a VPC ficará – Uma VPC abrange todas as Zonas de Disponibilidade dentro da Região selecionada.
Intervalo de IP para a VPC na notação CIDR – Isso determina o tamanho da sua rede. Cada VPC pode ter até cinco CIDRs: um primário e quatro secundários para IPv4. Cada um desses intervalos pode ter entre /28 (na notação CIDR) e /16 em tamanho.
Gateway de Internet
Para permitir que o tráfego público da internet acesse sua VPC
Um gateway de internet é uma conexão entre uma VPC e a internet. Você pode pensar em um gateway de internet como sendo semelhante a uma porta que os clientes usam para entrar na cafeteria. Sem um gateway de internet, ninguém pode acessar os 