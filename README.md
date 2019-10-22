# projeto-Aula

Alarme de incêndio com ESP8266 NodeMCU.

Nesse projeto vamos desenvolver um alarme de incêndio utilizando um NodeMCU ESP8266, que após detectar chamas ou gases
inflamáveis dispara um alarma e envia uma mensagem para o seu celular.

Para realização do trabalho iremos utilizar os seguintes materiais;
   1 Buzzer - como o alarme,
   1 Sensor de Gases inflamáveis - MQ-2,
   1 Sensor de Chamas - 760 a 1100 nm,
   1 ESP8266 NodeMCU,
   1 Protoboard,
Diversos Jumpers.

Ambos os sensores possuem pino analógico e digital,
no nosso caso iremos conecta-los através do pino digital,
que iram voltar o valor 0 caso não detecte nenhum problema ou 1 se detectar gases ou chamas.
Também iremos usar um pino para ligar o buzzer, para emitir um alerta caso detecte fogo ou gases, 
além de enviar uma notificação através do Pushbullet para o nosso celular através de um APP, compatível tanto com Apple
como Android.
