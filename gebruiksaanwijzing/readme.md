# Gebruiksaanwijzing

### opladen / vervangen batterijen
In dir project maken we gebruik van een batterijhouder voor 2 batterijen. Op die manier kan je ze makkelijk verwijderen om ze op te laden. Opladen kan met een oplader die geschikt is voor deze batterijen (zie BOM). Zorg steeds dat de batterijen voldoende opgeladen zijn zodat de motoren optimaal kunnen draaien.

### draadloze communicatie
#### verbinding maken
Voorzie de robot eerst van spanning door de batterijen aan te sluiten. De bluetooth module zou nu ook licht moeten geven. Verbind je apparaat(PC of android toestel) met de HC-05. Dit doe je door naar de bluetooth instellingen te gaan en op de HC-05 te klikken. Er zal een wachtwoord gevraagd worden, dit is meestal 1234. Als je verbonden bent kan je via elke serial communication app op je android of PC commando's versturen. Op PC raad ik simple serial terminal of putty aan, op android kan je de app serial bluetooth terminal gebruiken.

#### commando's
De onderstaande commando's kunnen allemaal ingegeven worden in de serial terminal. Via de HC-05 zal de arduino deze instellingen overnemen.

debug: bij het invoeren van dit commando krijg je alle parameters te zien die nu ingesteld zijn.  
run on: laat de robot rijden.  
run off: laat de robot stoppen.
set cycle [µs]  
set power [0..255]  
set diff [0..1]  
set kp [0..]  
set ki [0..]  
set kd [0..]  
calibrate black  
calibrate white  

### kalibratie
Om de robot correct te kalibreren moet je deze eerst op een wit vlak plaatsen (wit papier in voldoende licht) en het commando calibrate white ingeven. Wacht even tot er 'done' staat. Zet de robot daarna op een zwart vlak en doe hetzelfde met calibrate black.

### settings
De robot rijdt stabiel met volgende parameters:  
set cycle 5000
set power 60 (niet te hoog zetten voor de eerste keer)  
set diff 0,15 
set kp 8 
set ki 0 
set kd 0 

Als je de snelheid wilt verhogen zal kp waarschijnlijk moeten verhogen en ook kd een beetje groter maken kan handig zijn.
### start/stop button
Om de robot te starten en te stoppen geef je het commando run on of run off in. In sommige apps kan je hier ook een knop voor maken zodat het wat sneller gaat. 
