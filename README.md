# Omnitrix
Projeto de Sistemas Embarcados em Tempo Real

Com o intuito de experimentar a comunicação RTOS em dispositivos, fora-se desenvolvido a programação de dois dispositivos mestre-servo de forma a realizar a comunicação entre os mesmos, se utilizando do software STM32 CubeMX e do Keil uVision. Os dispositivos consistem de duas lógicas distintas:

## Dispositivo Mestre - Placa Utilizada: STM32F446RE

Possui a funcionalidade de contabilizar as horas, exibindo-os através de um relógio digital e de uma representação ilustrativa animada de um dia.  Além disso, é possível realizar o ajuste do horário manualmente através de transmissão de sinais para a placa STM32F446RE utilizada no projeto. O dispositivo também conta com comunicação wireless através de módulos bluetooth que se utilizam do protocolo serial para transmissão e recebimento de dados. Tal protocolo é utilizado para realizar um protocolo handshaking, além de transmitir o horário para o dispositivo servo. Todas as funcionalidades possuem telas respectivas as quais são exibidas em uma tela OLED SSD1306

## Dispositivo Servo - Microprocessador Utilizado: 

Se utiliza do módulo bluetooth para realizar o protocolo de handshaking com o dispositivo mestre, além de utilizá-lo como receptor da informação de horário transmitido pelo dispositivo mestre. A informação é então transmitida para uma tela OLED prórpia conectada ao dispositivo servo.


