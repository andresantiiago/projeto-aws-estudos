Implantar uma instância EC2 na AWS rodando o nginx via docker e que exiba uma pagina web.


- Criar uma conta na AWS
- Criar uma VPC e subnet
- Criar uma keypair
- Criar uma instância EC2:
    - Utilizar o tipo t2.micro (free tier)
    - Utilizar o ubuntu ou debian
    - Utilizar a keypair criada anteriormente para permitir o acesso a instância
    - Utilizar a VPC e subnet criada
    - Atribuir IP público a instância
    - Criar um novo grupo de segurança (security group) permitindo acesso via SSH do seu IP (a AWS consegue identificar o IP na tela de criação) e liberando a porta 80 para internet
- Acessar a instância via ssh utilizando a keypair criada
- Instalar o docker
- Executar o nginx via docker e de forma que seja possível acessar a página default via IP público na porta 80