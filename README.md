# TrabalhoGA_Redes2_V-torPires
## Objetivo
• Configurar e avaliar o desempenho de dois protocolos de roteamento dinâmico, RIP e OSPF, em uma rede virtual com três roteadores utilizando a plataforma BIRD, focando em métricas da Camada 3 do modelo OSI.
## Etapa 1
• Após criar as 3VM'S (Roteador1, Roteador2 e Roteador3) utilizar o comando "sudo nano /etc/netplan/00-installer-config.yaml" no terminal em cada uma delas. Limpe tudo e cole o conteúdo do netplan respectivo de cada roteador disponível na pasta configs. Use o comando sudo "netplan apply" para validar as modificações.
## Etapa 2
• Utilize os seguintes comandos no terminal dos 3 roteadores: "echo 'net.ipv4.ip_forward=1' | sudo tee -a /etc/sysctl.conf" e "sudo sysctl -p".
## Etapa 3
• Em todos os roteadores, instale o BIRD com o comando "sudo apt install bird2 -y".
• Para backup utilize "sudo cp /etc/bird/bird.conf /etc/bird/bird.conf.backup".
• Para configurar por arquivo único utilize: "sudo ls -la /etc/bird/".
## Etapa 4
• Use o comando "sudo nano /etc/bird/bird.conf" em cada roteador, e cole o conteúdo do bird.conf respectivo de cada roteador presente na pasta configs.
## Etapa 5
• Para testes, habilidade o console BIRD com o comando "sudo birdc". Utilize comandos como •show status •show protocols •show route e etc..
