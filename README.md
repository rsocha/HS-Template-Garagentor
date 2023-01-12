# HS-Template-Garagentor

## Template 40-110.hst

Version: 6.4.10082022

Template für den Gira Homeserver zum steuern eines Garagen- oder Einfahrt Tor.

Version für hell und dunkel.


# HS-Logikbaustein Torstatus

## Baustein 15014_Torsteuerung_v2.1.hsl

Version 2.1

Eingang 1:
KO für Tor ist offen (1Bit).

Eingang 2:
KO für Tor ist geschlossen (1Bit)

Eingang 3:
Wert in sec eingeben für Verzögerung bis an A3 die Warnausgabe (1Bit) kommt.

Eingang 4:
Wert in sec eingeben für Schrittweite des Betriebsstundenzählers, Ausgabe an A5. Ausgabe in hh:mm. Rest bei öffnen oder schliessen.

Ausgang 1:
Hier wird 0% bei offen, 50% bei fährt oder halboffen und 100% bei geschlossen ausgegeben.

Ausgang 2:
Hier wird eine 1 für Tor fährt und eine 0 für Tor fährt nicht ausgegeben.

Ausgang 3:
Hier wird nach Ablauf des Timers auf A3 eine 1 für Warnung ausgegeben (sbc).

Ausgang 4:
Hier wird eine 1 bei offen, eine 2 bei fährt und eine 0 bei geschlossen ausgegeben.

Ausgang 5:
Hier wird die Zeit in hh:mm seit geöffent oder geschlossen ausgegeben..

Eingänge
Eingang	Init	Beschreibung
Eingang 1	0	Hier wird das Kommunikationsobjekt zugeordnet für Tor ist offen.
Eingang 2	0	Hier wird das Kommunikationsobjekt zugeordnet für Tor ist geschlossen.
Eingang 3	0	Hier wir die Zeit für den Timer eingestellt falls Tor nicht geschlossen wird.
Eingang 4	0	Hier wir die Schrittweite für den Betriebsstundenzählers eingestellt.
Ausgänge
Ausgang	Init	Beschreibung
Ausgang 1	0	Hier wird 0%, 50% oder 100% ausgegeben, je nach Torstatus.
Ausgang 2	0	Hier wird eine 1 für Tor fährt und eine 0 für Tor fährt nicht ausgegeben.
Ausgang 3	0	Hier wird eine 1 bei Warnung ausgegeben (sbc).
Ausgang 4	0	Hier wird eine 1 bei offen, eine 2 bei fährt und eine 0 bei geschlossen ausgegeben.
Ausgang 5	0	Hier wird die Zeit in hh:mm seit geöffent oder geschlossen ausgegeben.
Sonstiges
Neuberechnung beim Start: Ja
Baustein ist Remanent: Ja
Interne Bezeichnung: "15014"
Der Baustein wird im "Experten" in socha.at einsortiert.
