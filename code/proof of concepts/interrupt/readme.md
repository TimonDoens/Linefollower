# start/stop interrupt proof of concept
minimale hard- en software die de correcte werking van een start/stop drukknop aantoont, gebruik makend van een hardware interrupt

# Concept
Als de schakelaar wordt ingedrukt waarmee men een start of stop signaal wilt genereren, zal via de "attachInterrupt" functie de loop hardwarematig onderbroken worden. Als de intterupt wordt getriggerd wordt de functie "void interrupt()" uitgevoerd. Hierin wordt ter demonstratie de toestand van een led gewijzigd. Dit kan vervangen worden door een start/stop signaal.
# Elektronisch schema
<img width="1482" height="630" alt="image" src="https://github.com/user-attachments/assets/9a392bf8-dae3-479e-836f-7f45174ea7bc" />

