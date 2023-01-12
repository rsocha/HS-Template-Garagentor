# HS-Template-Garagentor

## Template 40-110.hst

Version: 6.4.10082022

Template für den Gira Homeserver zum steuern eines Garagen- oder Einfahrt Tor.

Version für hell und dunkel.


# HS-Logikbaustein Torstatus

## Baustein 15014_Torsteuerung_v2.1.hsl

Version 2.1

## Eingänge


| Nr. | Name | Init | Beschreibung |
|-----:|---------------| ---- | --- |
| 1 | E1 Tor Status Offen |  | KO für Tor ist offen (1Bit). |
| 2 | E2 Tor Status Zu |  | KO für Tor ist geschlossen (1Bit) |
| 3 | E3 Verzögerung für Warnung (sec) |  | Wert in sec eingeben für Verzögerung bis an A3 die Warnausgabe (1Bit) kommt. |
| 4 | E4 Betriebsstunden Schrittweite (sec) |  | Wert in sec eingeben für Schrittweite des Betriebsstundenzählers, Ausgabe an A5. Ausgabe in hh:mm. Reset bei öffnen oder schliessen. |
| 5 | E5 Abwesend |  | Wert in sec eingeben für Schrittweite des Betriebsstundenzählers, Ausgabe an A5. Ausgabe in hh:mm. Rest bei öffnen oder schliessen. |
| 6 | E6 Regen |  | Bei 1 und Tor Offen wird an A7 eine 1 gesendet (1Bit). |
| 7 | E7 Sperre Regen |  | Bei 1 wir A7 gesperrt (keine Ausgabe) |


## Ausgänge


| Nr. | Name | Init | Sbc |Beschreibung |
|-----:|---------------| ---- | --- | -- |
| 1 | A1 Tor Status (100%=Zu / 0%=Offen) |  | Sbc | Hier wird 0%, 50% oder 100% ausgegeben, je nach Torstatus. (50% = weder offen noch zu oder fährt) |



Neuberechnung beim Start: Ja

Baustein ist Remanent: Ja

Interne Bezeichnung: "15014"

Der Baustein wird im "Experten" in r.socha einsortiert.

