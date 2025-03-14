### das Benutzerhandbuch für das HLK-LD6001A-60G Radar-Modul    
von Shenzhen Hi-link Electronics Co., Ltd. überprüft. Hier sind die wichtigsten    
technischen Details und der Schaltplan, um den Sensor zum Laufen zu bringen:

### Produktmerkmale   
Erkennungsmethode: Millimeterwellenradar, nicht beeinträchtigt durch Licht, Temperatur, Staub, etc.    
Erkennungsbereich: 0,5 bis 8 Meter, mit einem Radius von 3,5 Metern bei einer Installationshöhe von 2,7 Metern.    
Kommunikationsmethode: TTL-Seriellport.    
Betriebsfrequenz: 60-64 GHz.    
Stromversorgung: 3,3V.   
Leistungsaufnahme: Durchschnittlich 0,3W, Spitzenleistung 1,7W.    
Elektrische Eigenschaften   

### Pin-Beschreibung:   
3V3: Modulstromversorgung.    
NRST: Modul-Reset.    
TX: Serieller Port senden.    
RX: Serieller Port empfangen.   
GND: Masse.   
 
 
 das HLK-LD6001A-60G Radar-Modul mit einem TTL zu USB Serial Port Adapter verwenden. Hier sind die Schritte und Einstellungen, um die Daten zu lesen:

Verbindung herstellen
Hardware-Verbindung:

TX des Radar-Moduls mit RX des USB-TTL Adapters verbinden.    
RX des Radar-Moduls mit TX des USB-TTL Adapters verbinden.   
GND des Radar-Moduls mit GND des USB-TTL Adapters verbinden.   
3V3 des Radar-Moduls mit 3V3 des USB-TTL Adapters verbinden   
(falls der Adapter 3.3V unterstützt).   

## Software-Einstellungen:

Baudrate: 115200 (Standardwert, kann konfiguriert werden mit AT+BAUD=XX\n).

Protokollmodus: AT+DEBUG=2\n für Host-Computer-Modus oder AT+DEBUG=0\n für einfachen Protokollmodus.

Schritte zur Konfiguration

Treiber installieren: Stelle sicher, dass die Treiber für den USB-TTL Adapter installiert sind. Diese sind oft auf der Herstellerseite verfügbar.

Terminal-Software: Verwende eine Terminal-Software wie MobaXTerm oder PuTTY.

COM-Port: Öffne den Gerätemanager und finde den COM-Port, der dem USB-TTL Adapter zugewiesen ist.

Terminal-Einstellungen:

Serial Port: Wähle den COM-Port aus.

Baudrate: Stelle die Baudrate auf 115200 ein.

Datenbits: 8.   
Stoppbits: 1.   
Parität: Keine.   
Flusssteuerung: Keine.    
AT-Befehle zur Steuerung    
AT+START\n: Starten des Moduls.   
AT+STOP\n: Stoppen des Moduls.   
AT+RESET\n: Modul zurücksetzen.   
AT+READ\n: Parameter lesen.   
AT+RESTORE\n: Werkseinstellungen wiederherstellen.   
Beispiel für Datenpaket   
Im einfachen Protokollmodus (AT+DEBUG=0\n) sieht ein Datenpaket wie folgt aus:   

55AA 0A 04 00 00 00 00 00 0E   
55AA: Frameheader.   
0A: Byteanzahl.   
04: Typ (z.B. Personenanzahl).   
00 00: Reserviert.   
00: Anzahl der gezählten Personen.   
0E: XOR-Prüfung.   

Falls du weitere Fragen hast oder Unterstützung bei der Einrichtung benötigst, lass es mich wissen! 😊
