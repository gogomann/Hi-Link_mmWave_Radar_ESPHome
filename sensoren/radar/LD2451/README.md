# HKL-LD2451 Motorrad 24 GHz Multi Target

Die meisten Infos kommen vom Hersteller: [https://www.hlktech.net/index.php?id=1282](https://www.hlktech.net/index.php?id=1282).



----

<a href="./HLK-LD2451_User_Manual_V1.0.pdf" class="image fit"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/PDF_file_icon.svg/534px-PDF_file_icon.svg.png" width="24" height="24"> HLK-LD2451_User_Manual_V1.0.pdf</a>
 
 

<img src="./scann 1920.webp" width=90% height=90%>

## ESPHome
ist automatisch erstellt worden von clude: [clude_hlk-ld2452.yaml](sensoren/radar/LD2451/clude_hlk-ld2452.yaml). Ist also ungestetet :warning: .

## PIN definition

PCB grösse : 70mm x 35mm <br>
Pin hole spacing: 2.54mm

| pin nr. | notation | name(of a thing) | functionnality |
| ------------ | ------------- |:-------------:| :-------------|
| 1 | VIN | Power input | Power supply input 5V |
| 2 | GND | power ground | power ground |
| 3 | OT1 | GPIO1 | Indicator pin, 3 consecutive high and low outputs on first startup Outputs high level when a person is detected approaching |
| 4 | TX | Serial port TX | serial tx pin |
| 5 | RX | Serial port RX | serial rx pin |
| 6 | OT2 | GPIO2 |temporarily unavailable |
