
# Alarme de incêndio com ESP8266 NodeMCU.

![LogoFatec](http://fatecsantoandre.edu.br/images/logo.png)
![logoCPS](http://fatecsantoandre.edu.br/images/logo_centro.png)
![logoGoverno](http://fatecsantoandre.edu.br/images/logo_sp.png)
 
     Amanda Nardi     RA:0791611040
     Rafael Thiago    RA:0791811043
> <em> Um trabalho para a disciplina de Sistemas Microprocessados e Microcontrolados

   # Descrição do projeto:
Nesse projeto iremos desenvolver um alarme de incêndio utilizando um NodeMCU ESP8266, que após detectar chamas
ou gases inflamáveis irá disparar um alarma e enviará uma mensagem para o seu celular.

   # LISTA DE MATERIAIS:
1 Buzzer - como o alarme,
1 Sensor de Gases inflamáveis - MQ-2, 
1 Sensor de Chamas - 760 a 1100 nm, 
1 ESP8266 NodeMCU, Diversos Jumpers.
1 ESQUEIRO (para testes)

   # ANOTAÇÕES GERAIS:
Ambos os sensores possuem pino analógico e digital, no nosso caso iremos conecta-los através do pino digital,
que ira retornar o valor 0 caso não detecte nenhum problema ou 1 se detectar gases ou chamas. 
Também iremos usar um pino para ligar o buzzer, para emitir um alerta caso detecte fogo ou gases, 
além de enviar uma notificação através do Pushbullet para o nosso celular através de um APP,
compatível tanto com Apple como Android.

   # Sensores utilizados:
    -MQ-2
   Este Sensor de Gas MQ-2 Inflamável e Fumaça é capaz de detectar concentrações de gases combustíveis e fumaça no ar. 
   É um módulo confiável e simples de usar em seus projetos de automação residencial com Arduino, por exemplo.
Também é uma ótima opção para acionar um microcontrolador ou relés.
Quando a concentração de gases fica acima do nível ajustado pelo potenciômetro, a saída digital D0 fica em estado alto.
Se abaixo do nível, fica em estado baixo.
   Para ter uma resolução melhor e medir a variação da concentração dos gases no ar, 
é possível usar a saída analógica A0 e conectar a um conversor AD, como a presente no Arduino e Raspberry Pi, por exemplo.

    -SENSOR DE FOGO/CHAMAS:
   O Sensor de Chama Fogo  pode ser usado para detectar fontes de chama ou outras fontes de calor 
que possuam tamanho de onda entre 760 a 1100 nm.
Seu ângulo de detecção pode chegar a 60 graus e no meio de sua placa há um buraco onde se encaixa um parafuso
com o objetivo de direcionar o sensor conforme desejado.
   Quando há fogo, a saída do sensor fica em estado baixo (0) e quando não há detecção em estado alto (1).
Este limite pode ser ajustado através do potenciômetro presente no sensor que regulará a saída digital D0. 
Contudo, para ter uma resolução melhor é possível utilizar a saída analógica A0 e conectar a um conversor AD, 
como a presente no Arduino, por exemplo.

    -Montagem Final
![sistema-de-deteccao-e-alarme-de-incendio-03](https://uploads.filipeflop.com/2016/11/Alarme-de-inc%C3%AAndio-com-ESP8266-NodeMCU.png)

