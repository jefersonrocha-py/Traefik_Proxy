# Traefik_Proxy
 Microserviço Traefik em Docker para usar como Proxy, SSL e Load Balance

###############################################################
O Traefik é um balanceador de carga e roteador reverso
projetado especificamente para ambientes de contêiner. 
Ele fornece uma camada de gerenciamento e orquestração
para seus containers, facilitando a exposição de seus 
serviços para o mundo exterior. 
Com o Traefik, você pode configurar rotas,
balanceamento de carga e SSL/TLS de forma simples e eficiente.
###############################################################

Lembre-se de criar a Network para o Traefik e coloque as Stack que precisem usar
o Traefik como Proxy.
####################-Segue o exemplo a abaixo-##########################
### docker network create --driver=bridge --subnet=10.250.0.0/29 web ### # Subnet colocacada como exemplo
########################################################################

![image](https://github.com/user-attachments/assets/feb71ba8-a1cb-4b5b-ab84-a526398f8de2)

 
