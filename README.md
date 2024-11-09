# eines vor weg alles was ich so gefunden habe im Netz oder hier in Github oder im Forum, alles ungetestet
# Hi-Link mmWave Radar For ESPHome
Suggest used ESP-IDF framework to improve efficiency and stabilized.   
If using Arduino Framework, disconnect the UART cable might cause API error(disconnect).
## Plan to Support:
:white_check_mark: LD1115H UART/GPIO output, UART with sensitivity adjustable >[Link](./LD1115H)    
:white_check_mark: LD1125H UART output, UART with sensitivity adjustable >[Link](./LD1125H)     
:white_check_mark: LD112 GPIO output without adjustable >[Link](./LD112)  
:white_check_mark: LD017 IIC/GPIO output, IIC/GPIO for sensitivity adjustable >[Link](./LD017)     
:negative_squared_cross_mark: LD016 GPIO output, UART for sensitivity adjustable   
:white_check_mark: LD012 GPIO output with sensitivity adjustable pins >[Link](./LD012)  
:negative_squared_cross_mark: LD6001   
:negative_squared_cross_mark: LD7903A   

Code at each Radar Folder   
Note: Don't use 5V on LD017, LD012, LD2420   

### Similar Device:
LD2410 = LD2410B = LD2410C   
CEM5825F = LD1125H   
CEM5855H = LD1115H   


## No Plan to Support:   
LD2410: ESPHome Official Support Already   
LD2420: ESPHome Official Support Already   
LD7901B: 79Ghz Water Level Radar   
LD303: 24Ghz Leagacy Model    
LD116: 24Ghz Leagacy Model   
LD101: 10Ghz Leagacy Model   
LD102: 10Ghz Leagacy Model   
LD105: 5.8Ghz Leagacy Model   
LD010: 5.8Ghz Leagacy Model   
LD015: 5.8Ghz Leagacy Model   

## Reference:  
  ESPHOME:  
    <https://esphome.io/cookbook/uart_text_sensor.html>  
    https://esphome.io/custom/uart.html  
    https://esphome.io/components/uart.html  
    https://esphome.io/components/sensor/custom.html   
