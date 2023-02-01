# UPS_HAT_v1.2
 File fo monitoring voltage and battery capacity of UPS Lite v1.2 power supply for Raspberry Pi Zero.
 
 Para execucao do projeto sao necessarios os seguintes aplicatiovos instalados no dispopsitivo:
 ```
 apt install i2c-tools libi2c-dev python3-smbus wiringpi git-core
 ```
 Para executar o script basta chama-lo com `python3 ups-hat-monitor.py` e a cada 5 segundos ele trara a voltagem e o percentual de bateria, bem como seus status se esta carregando ou descarregando.
 Acima de 100% sera exibido "Battery FULL", entre 5 e 15% e exibido o alerta "Battery LOW" e abaixo de 5% "DANGER!!! BATTERY RUNNING OUT".
