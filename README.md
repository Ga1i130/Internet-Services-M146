# Internet Services
Teammitglieder: 
- Marco Neuschwander
- Kate Falco
- Janis Müller
### This README.md file is used by this Group to Note down all information related to the Internet Services Project.
---
# Project Explanation 
This Project was started as part of the Module 146 at TBZ. In this Modul we've got the Job to make a Project aboute the Topic "Internet Services".
---
# Einleitung: 


# Inhaltsverzeichnis Theorie: 
1. Autoren, Versionierung des Dokumentes](Autoren.md "1. Autoren, Versionierung des Dokumentes ")


[2. Einfuehrung](Einfuehrung.md "2. Einfuehrung ")
   - Beschreibung: Welche Funktionen wird der Service erfuellen
   - Vorgesehener Zeitaufwand für die Realisierung
   - Stolpersteine

[3. Benoetigte Hard- und Software](Hardware.md  "3. Benoetigte Hard- und Software" )
   - Hardware (Materialliste, Funktionalitaet)
   - Software (Anforderungen, Firmware, OS-Image, ergaenzende SW-Packages, Ab-
	hängigkeiten, Funktionalitaet)
	
	
[4. Installationsanleitung](Installationsanleitung.md "4. Installationsanleitung")
   - Anweisungen verstaendlich und nachvollziehbar
   - Keine fertigen Loesungsschritte aufzeigen
   - Hilfestellung (Tipps, Quellen...)

[5. Qualitaetskontrolle](Qualitaetskontrolle.md "5. Qualitaetskontrolle")

[6. Error-Handling](Error-Handling.md  "6. Error-Handling ")

[7. Quellen](Quellen.md "7. Quellen")

[8. Lizenzen](Lizenz.md "8. Lizenzen" )

# Inhalsverzeichnis Vertiefungsarbeit: 

---
## Composition
- Virtual Box
- Ubuntu Sever LTS 20.04.2 AMD whit User Interface
- Apache Web Server (as mirror)
- 
---
## Issues

- Storage on my virtual disc was firstly scaled by 10 GB afterwards i've added a second vhd with about 64 Gb storage to fight against boot errors. 
quote: Add enough Storage at the first time.
improvements: Add a dedicated HDD to store the repos for the mirror
- due to the Additon of the second vhd i was forced to re isntall the unix enviroment wit more storage.

### Why not to use Azure VM's
As a second try, follwing the Virtual Box VM', we've tried to use Azure Virtual Machines. Firstly they are quite complicated in use. The Price Tag for Education schould be free but about 4 days after we've setted up this vm Janis got an message that about one quarter of the Money was used, the vm consumed money even when its shutted down. 

---

## Work-Flow
df
