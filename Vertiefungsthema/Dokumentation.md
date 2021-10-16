# Dokumentation

### 1. Installation

Installation apt-miror

Als erstes müssen wir apt-miror auf dem Server installieren, es ist bereits vorkonfiguriert so dass wir kaum etwas tun müssen um den Mirror einzurichten.
Befehl zum Installieren der Pakete: 

```diff
- sudo apt-get install apt-mirror 
```

### 2. Konfiguration

Bei der Installation wird automatisch die Datei mirror.list im Ordner /etc/apt/ mit folgendem Inhalt angelegt. In ihr steht wo welche Dateien gespeichert werden.

![Bild1](https://user-images.githubusercontent.com/89446428/137598189-5e6152fc-dab0-408f-b9e9-561886ef3015.png)
 
Wir müssen gar nichts machen ausser die config einmal zu überprüfen, ob alles geklappt hat.

Somit ist die Grundkonfiguration bereits erledigt.

Wir wollen aber noch die Download Geschwindigkeit begrenzen damit nicht die ganze Bandbreite ausgenutzt wird. Deshalb haben wir folgende Zeile in die Datei 
/etc/apt/mirror.list eingefügt 

Zu beachten ist, dass der Parameter pro Downloadslot gilt.

![Bild2](https://user-images.githubusercontent.com/89446428/137598305-41d8b2b3-4372-4b41-9071-b2c0c0b0a559.png)
![Bild3](https://user-images.githubusercontent.com/89446428/137598306-b1eba55d-59f5-48c8-a313-51c8fe868fd7.png)
 
### 3. Nachbehandlung

Wir wollen jetzt noch alle heruntergeladenen Pakete noch aufräumen. Dabei werden alte Dateien gelöscht und dafür gesorgt das der Mirror auch schnell läuft.

![Bild4](https://user-images.githubusercontent.com/89446428/137598329-467508ad-c094-45f4-af0b-6e59620aea16.png)
 
### 4. Start von apt-mirror¶

Nun müssen wir den Mirror auch noch starten. Der Start erfolgt in einem Terminal durch Eingabe von:

```diff
- sudo apt-mirror 
```

### 5. Nutzen des Mirror

Auf den Clientsystemen muss jetzt nur noch der neue Server eingetragen werden. Damit Linux weiss, wo es die Updates holen muss.

```diff
- deb http://192.168.0.154 ubuntu quantal main restricted
```

### Fehler die wir hatten

Wir hatten eigentlich nur einen Fehler nämlich das wir nicht genug Speicherplatz hatten, es benötigt ca 220Gb wir empfehlen deshalb eine Festplattengrösse von ca. 300GB. So ist dann auch noch genügen Platz da bei zukünftigen Updates noch date hinzukommen werden.

### Issue: 

- Storage on my virtual disc was firstly scaled by 10 GB afterwards i've added a second vhd with about 64 Gb storage to fight against boot errors. 
quote: Add enough Storage at the first time.

improvements: Add a dedicated HDD to store the repos for the mirror

- due to the Additon of the second vhd i was forced to re isntall the unix enviroment wit more storage.





