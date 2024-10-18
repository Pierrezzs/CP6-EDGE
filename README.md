# CP6-EDGE
Checkpoint 6 de EDGE computing 1-ESPK 2024 sistema para verificação de temperatura, umidade e luminosidade de uma vinheria. 

Grupo: NJ Tech
<table>
  <tr>
    <th>Nomes</th>
    <th>Rm</th>
  </tr>
  <tr>
    <td>Gustavo Pierre</td>
    <td>558928</td>
  </tr>
  <tr>
    <td>Gabriel Belo</td>
    <td>551669</td>
  </tr>
  <tr>
    <td>Enzo Dias</td>
    <td>558225</td>
  </tr>
  <tr>
    <td>Arthur Abonizio</td>
    <td>555506</td>
  </tr>
</table>

<h1>Link Para o projeto</h1>
https://wokwi.com/projects/409870629323275265

<h1>Materiais:</h1>
<ul>
  <li>ESP32</li>
  <li>Photoresistor (LDR) Sensor</li>
  <li>DHT22</li>
</ul>



<h1>Foto do sistema:</h1>
<img src="https://github.com/user-attachments/assets/f0d5400b-f5d8-4375-90d9-28c4384cb47b"/>

<img src="https://github.com/user-attachments/assets/f0d5400b-f5d8-4375-90d9-28c4384cb47b"/>

<h2>Explicação do projeto</h2>
Nós implementamos um projeto que utiliza o ESP32 para capturar dados de temperatura, umidade e luminosidade em uma adega, utilizando dois sensores: o DHT11 (para temperatura e umidade) e o LDR (para luminosidade). Nosso objetivo foi monitorar essas variáveis para garantir as condições ideais de conservação dos vinhos.
</br>
<h2>O que fizemos:</h2>
</br>
1. Montagem dos Sensores:
  - Conectamos o DHT22 ao ESP32 para medir a temperatura e a umidade.
  - Ligamos o LDR para monitorar os níveis de luminosidade dentro da adega.

  *Durante o desenvolvimento do projeto  em sala de aula utilizamos uma placa que possui alguns componentes, dentre eles estavam o LDR e um DHT11, fazendo assim com que tenha algumas diferenças para o projeto desenvolvido no wokwi.

</br>
2. Programação do ESP32:
  - Desenvolvemos o código para fazer leituras constantes desses sensores.
  - Incluimos as bibliotecas necessárias para o desenvolvimento do projeto. Então configuramos a conexão do ESP32 a uma rede Wi-Fi e integramos com o protocolo MQTT para enviar os dados coletados para um servidor.

</br>
3. Envio de Dados ao Servidor:
  - Usamos o broker público HiveMQ para enviar os dados da adega.
  - Os dados eram enviados em formato JSON, contendo as leituras de temperatura, umidade e luminosidade.

</br>
4. Aplicativo MyMQTT:
  - Configuramos o aplicativo MyMQTT com o IP e os topics para ler os dados que foram enviados pelo ESP32.
  - A partir do MyMQTT, conseguimos visualizar em tempo real as condições internas da adega.

</br>
<h2>Por que é importante?</h2>
Com este sistema, a Vinheria Agnello pode monitorar de forma remota e em tempo real as condições ambientais da adega, garantindo que a temperatura, umidade e luminosidade estejam adequadas para a conservação dos vinhos.
Em resumo, desenvolvemos um sistema de monitoramento de IoT eficiente e prático, utilizando sensores e o ESP32, que transmite os dados através da rede para facilitar a tomada de decisões rápidas e precisas sobre o ambiente da adega.
