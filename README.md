![GitHub Logo](http://www.heise.de/make/icons/make_logo.png)

Maker Media GmbH
*** 

# Die animatronische Posteule

### Wie durch Zauberhand: Der Raspberry Pi verwandelt eine Plüscheule in eure persönliche kleine Mitteilungszentrale. Sie flattert, schnattert, blinzelt und kann ihren Kopf drehen. Und das beste: Ihr habt dank Python die Programmierung selbst in der Hand. 

![Picture](https://github.com/MakeMagazinDE/Posteule/blob/main/posteule2.png)

Hier findet ihr die benötigten Dateien für den 3D-Druck und die Skripts für die Programmierung. <br>Die 3D-Dateien sind bereits ausgerichtet und mit Cura getestet. 

### Verwendete Druckparameter:
<b>Material:</b> PLA <br>
<b>Temp.:</b> 210°C <br>
<b>Infill:</b> 25% <br>
<b>Support:</b> überall, Zickzack <br>
<b>Schichthöhe:</b> 0,2mm (0,1mm für K5, K6 und K7) <br>
<b>Druckgeschwindigkeit:</b> 50mm/s (20mm/s für K5, B1 und B2) <br>
<b>Bewegungsgeschwindigkeit:</b> 100mm/s (50mm/s für K5, B1 und B2) <br>
<b>Druckplattenhaftung:</b> Skirt (Brim für K5, B1 und B2) <br>
<br>
### Hinweise: 
### Zur E-Mail-Abfrage:
- Verwendet für die Eule eine gesonderte E-Mail-Adresse, weil die Funktion checkIncoming() nach dem Abfragen alle E-Mails löscht.
### Zu den 3D-Dateien aus Teil 1:
- Das Augenlid <b>K5</b> muss zweimal gedruckt werden, die Ringe <b>F1</b> dreimal. <br>
### Zu den 3D-Dateien aus Teil 2:
- Folgende Dateien müssen zweimal gedruckt werden: <b>A8, A9, BN1, BN3, FX</b> und <b>G4</b>
### Zu optimierten 3D-Dateien:
- Es gibt ein paar angepasste 3D-Druckdaten zu <a href="https://github.com/MakeMagazinDE/Posteule/tree/main/3D-Druck/Teil%201/Optimierte%20Modelle"><b>Teil 1</b></a> und <a href="https://github.com/MakeMagazinDE/Posteule/tree/main/3D-Druck/Teil%202/Optimierte%20Modelle"><b>Teil 2</b></a>.
### Die Grafiken 7 und 10 aus der zweiten Bauanleitung (Make 2/22) wurden mit Ziffern ergänzt:
- Ihr findet sie in dem Ordner <a href="https://github.com/MakeMagazinDE/Posteule/tree/main/Extras"><b>Extras</b></a>.

![Picture](https://github.com/MakeMagazinDE/Posteule/blob/main/banner_ziffern.png)

<br>

### Hinweis zu dem Servo, der den Augenmechanismus steuert:
Die Bauform der MG90s-Servos scheint sich je nach Hersteller zu unterscheiden. Dadurch kann es passieren, dass der Arm <b>A2</b> mit <b>K1</b> kollidiert, wenn die Welle zu kurz ist oder zu weit hinten sitzt. Zwischen <b>A2</b> und <b>K1</b> sollte eine ca. 0,6mm große Lücke vorhanden sein, damit sich der Arm am Servo problemlos bewegen kann. Haltet am besten den Arm <b>A2</b> einmal an den Servo, und schaut von oben, ob ihr eine Lücke seht. <br>In dem Ordner <a href="https://github.com/MakeMagazinDE/Posteule/tree/main/3D-Druck/Teil%202/Extra"><b>3D-Druck/Teil 2/Extra</b></a> findet ihr die Datei <b>servo_spacer.stl</b>. Dabei handelt es sich um einen kleinen Ring, der in den Arm <b>A2</b> eingesetzt werden kann, bevor ihr ihn am Servo montiert. Er ist 1mm hoch, damit ihr ihn in eurem Slicer auf die richtige Größe (Z-Achse) skalieren könnt. Für alle, die bereits die Teile für den zweiten Artikel gedruckt haben: Der Abstandhalter kann auch aus Pappe gefertigt werden. In der Kurzinfo zum zweiten Artikel findet ihr den Link zu einem Video, das näher darauf eingeht.
<br>
<br>
### Befehle, die nach der Installation von Raspberry Pi OS eingegeben werden müssen <br>(siehe Teil 2 der Bauanleitung):
sudo apt update <br>
sudo apt full-upgrade <br>
sudo apt install python3-pip <br>
sudo apt install ffmpeg libavcodec-extra <br>
sudo apt install i2c-tools <br>
sudo apt install libportaudio2 <br>
sudo pip3 install imapclient <br>
sudo pip3 install smbus <br>
sudo pip3 install adafruit-circuitpython-lis3dh <br>
sudo pip3 install adafruit-circuitpython-servokit <br>
sudo pip3 install pysinewave <br>
sudo pip3 install pydub <br>



<br><br>
Den vollständigen Artikel für den <b>ersten Teil</b> der Bauanleitung gibt es in der [Make-Ausgabe 1/2022](https://www.heise.de/select/make/2022/1/2135511401796522217) zu lesen. 
<br>
Den vollständigen Artikel für den <b>zweiten Teil</b> der Bauanleitung gibt es in der [Make-Ausgabe 2/2022](https://www.heise.de/select/make/2022/2/2203916022634105772) zu lesen. 
