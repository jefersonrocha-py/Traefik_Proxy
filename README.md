Traefik Proxy
Microserviço Traefik em Docker para Proxy, SSL e Load Balancing.

Visão Geral
O Traefik é um balanceador de carga e roteador reverso projetado especificamente para ambientes de contêiner. Ele facilita a exposição e a gestão de seus serviços, fornecendo uma camada de gerenciamento e orquestração eficiente. Com o Traefik, você pode configurar rotas, balanceamento de carga e SSL/TLS de maneira simplificada.

Principais Funcionalidades:
Balanceamento de Carga: Distribua o tráfego de forma eficiente entre seus serviços.
SSL/TLS: Configure certificados SSL/TLS para garantir a segurança das suas aplicações.
Roteamento Dinâmico: Automatize a exposição dos seus serviços com base nas suas necessidades.
Requisitos
Antes de iniciar, é essencial que você crie uma network dedicada para o Traefik. Essa network será utilizada pelas stacks que necessitam do Traefik como proxy.

Criando a Network
Para criar a network, utilize o comando abaixo:
Exemplo abaixo :
docker network create --driver=bridge --subnet=10.250.0.0/29 web
Nota: A subnet fornecida é apenas um exemplo. Certifique-se de ajustar conforme suas necessidades.

Estrutura do Projeto
plaintext
Copiar código
├── docker-compose.yml
├── traefik/
│   ├── traefik.toml
│   ├── acme.json
│   └── dynamic/
│       └── dynamic_conf.toml
└── README.md


![image](https://github.com/user-attachments/assets/018f3d2c-8312-4dc9-abb6-2a8fce5a159a)
