# Sprint3-Edge-Computing

- Aline Fernandes Zeppelini - 97966
- Camilly Breitbach Ishida - 551474
- Gabriel Antony Cadima Ciziks - 98215
- Lucca Sabatini Tambellini - 98169

    O projeto:

O projeto "Care Connect" propõe uma solução inovadora para auxiliar as ONGs na captação de recursos financeiros, aproveitando o potencial das redes sociais e jogos para gerar doações. A plataforma permitirá aos usuários acumular pontos por meio do envolvimento online, convertendo esses pontos em doações transparentes para causas sociais e ambientais. Além disso, uma abordagem adicional envolve a venda de kits Arduino com sensores de temperatura e umidade para monitorar o cultivo de plantas em casa, oferecendo outra fonte de financiamento sustentável para as ONGs, promovendo simultaneamente a conscientização ambiental.

    Desenvolvimento da arquitetura para uma aplicação IoT:

A Internet das Coisas (IoT), também conhecida como Internet of Things em inglês (IoT), é uma tecnologia que descreve uma rede de objetos físicos incorporados com sensores, software e outras tecnologias. O objetivo principal é conectar esses objetos à internet e permitir que eles troquem dados com outros dispositivos e sistemas. Esses dispositivos podem variar amplamente, desde objetos domésticos comuns, como eletrodomésticos, até ferramentas industriais sofisticadas e até mesmo carros. Esses itens têm a capacidade de coletar informações e transmiti-las através da nuvem, permitindo um mundo cada vez mais conectado e inteligente.

    Instruções para a aplicação prática da IoT:

Para a aplicação prática da IoT, utilizamos um esquema em Arduino (o código utilizado está disponível no arquivo code.ino e uma imagem do esquema também está disponível).

- Utilize o esquema com o sensor DHT11 (que mede a temperatura e umidade).
- Escreva o código no Arduino, incluindo as duas bibliotecas DHT11 e ArduinoJson(DHT11 disponível neste repositório e ArduinoJson pesquisando e baixando na biblioteca do arduino).
- Verifique se os valores do sensor estão sendo lidos no Serial Monitor.
- Faça a instalação local do Node-RED.
- Digite no Node.js Command Prompt: npm install -g --unsafe-perm node-red.
- Digite no Node.js Command Prompt: node-red.
- (Deixe o cmd do Node sempre aberto).
- Acesse o localhost no navegador: http://localhost:1880.
- No Node-RED, baixe as bibliotecas "node-red" e "node-red-serialport".
- Monte uma linha do fluxo conectando o Serial In, o JSON, a Function e o MQTT Out.
- Monte a outra linha com o MQTT In conectado ao Debug.
- Configure a Serial com a porta serial de acordo com a porta conectada no Arduino; configurações: baud rate 9600.
- Coloque o código na Function (disponível neste repositório).
- No Tago.io, crie um dispositivo.
- Vá em Devices, adicione um dispositivo, escolha Custom MQTT e crie.
- Acesse o dispositivo criado, vá no ícone do olho para ver o token, copie o token.
- No Node-RED, configure o MQTT Out.
- Em segurança, coloque o token copiado como senha.
- No servidor, coloque: mqtt.tago.io.
- No tópico: tago/data/post.
- Faça o deploy do fluxo.
- Verifique se os valores do sensor estão sendo lidos no Debug do Node-RED.
- No Tago.io, crie um dashboard.
- Vá em Devices e clique em "play" no Live Inspector.
- Verifique se os valores do sensor estão sendo lidos.
- Vá em Buckets e verifique as variáveis.
- Verifique se os valores estão sendo registrados.
- Vá em Dashboards.
- Crie um widget.
- Escolha a opção Line.
- Configure o widget com o dispositivo criado e uma das variáveis.
- Crie outro widget com a outra variável.
- Verifique se os gráficos apresentam os valores lidos pelo sensor.

Link do vídeo no YouTube:
https://youtu.be/ykGct-O8oDY
