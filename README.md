# CCU2-FW
Archiv älterer CCU2 Firmware Versionen. Texte und Firmware Copyright by [eq-3](http://www.eq-3.de/service/downloads.html)

# Changelog
---------

**2.29.18**
- Neue Geräte

  [HMCCU2-1368] Integration HmIP-PDT-UK (Dimmer-Steckdose – Phasenabschnitt (UK-Version))

  [HMCCU2-1367] Integration HmIP-eTRV-UK (Heizkörperthermostat (UK-Version))

  [HMCCU2-1350] Integration HmIP-SPI (Präsenzmelder – innen)

  [HMCCU2-1349] Integration HmIP-BBL (Jalousieaktor für Markenschalter)

  [HMCCU2-1348] Integration HmIP-FBL (Jalousieaktor für Unterputzmontage)

  [HMCCU2-1347] Integration HmIP-BROLL (Rollladenaktor für Markenschalter)

  [HMCCU2-1346] Integration HmIP-FROLL (Rollladenaktor für Unterputzmontage)

  [HMCCU2-1345] Integration HmIP-MOD-OC8 (Schaltaktor mit Open Collector-Ausgang)

  [HMCCU2-1301] Integration HmIP-SWDO-I (Fenster- und Türkontakt – verdeckten Einbau)

  [HMCCU2-1274] Integration HmIP-BWTH / BWTH24 (Wandthermostat mit Schaltausgang)

  [HMCCU2-1250] Integration HmIP-PCBS-BAT (Schaltplatine für Batteriebetrieb)

  [HMCCU2-1206] Integration HmIP-SAM (Beschleunigungssensor)

  [HMCCU2-1043] Integration HM-LC-DW-WM (Dual-White-LED Controller)

für weitere Änderungen siehe http://www.eq-3.de/Downloads/Software/HM-CCU2-Firmware_Updates/HM-CCU2-2.29.18/HM-CCU2-Changelog.2.29.18.pdf


**2.27.8**
- Fehlerbehebungen

  [HMCCU2-1342] Unter bestimmten Umständen wurden OSRAM-Lightify-Geräte doppelt angezeigt. Dieser Fehler wurde behoben.

  [HMCCU2-1339] Fehler beim Aufrufen direkter Verknüpfungen behoben.
  
  [HMCCU2-1338] Die Controls zur Anzeige bestimmter Parameter wurden nur noch einzeilig dargestellt. Dadurch war der Wert bei langen Parameternamen nicht mehr lesbar.

  [HMCCU2-1337] HmIP-STH/STHD – Zugriff auf die Konfigurationsparameter wieder ermöglicht.


**2.27.7**
- Neue Geräte

  [HMCCU2-1260] Integration Hm-Sen-MDIR-O-3 (Homematic Funk-Bewegungsmelder, außen)

  [HMCCU2-1191] Integration HmIP-FDT (Homematic IP Dimmaktor Unterputz – Phasenabschnitt)

  [HMCCU2-1173] Integration HmIP-PCBS (Homematic IP Schaltplatine)

- Erweiterungen / Verbesserungen

  [HMCCU2-1336] Sicherheitsrelevante Erweiterungen: 

    * Firewall bei Systemstart starten 

    * Directory Traversal Schwachstelle behoben 

    * SSH Daemon erlaubt nur noch sichere Cipher und MACs 

    * Weitere Ports in der firewall.conf eingetragen 

    * Sicherheitslücke beim Prüfen auf gültige Session-ID behoben

  [HMCCU2-1335] Konfigurationsparameter „Soft On/Off“ für dimmbare OSRAM-Lightify hinzugefügt. Hinweis: Damit dieser Parameter zur Verfügung steht, müssen diese Geräte aus dem System gelöscht und neu hinzugefügt werden (erneutes Suchen von Geräten).

  [HMCCU2-1334] Unterstützung für OSRAM-Lightify Plug hinzugefügt.

  [HMCCU2-1333] Unterstützung für OSRAM-Lightify Gardensport Mini RGB hinzugefügt.

  [HMCCU2-1330] Manuelle Eingabe einer OSRAM-Lightify Gateway-IP ermöglicht.

  [HMCCU2-1328] Direkte Werteingabe der RGB-Werte im Lightify-Farbauswahldialog ermöglicht.

  [HMCCU2-1292] OSRAM Kopplung um Steuerung von Gruppen erweitert.

  [HMCCU2-1323] Parameter Luftdruck für entsprechende Geräte (z. B. WDC7000) in Diagrammen nutzbar.

  [HMCCU2-1302] Für neue HmIP Thermostat-Versionen wurde ein Konfigurationsparameter ein- geführt, der es ermöglicht, die Schaltzeitpunkte der Wochenprogramme im Auto-Modus für eine wählbare Zeit (max. 12 Std.) nicht zu berücksichtigen.

  [HMCCU2-1282] Integration HmIP-FAL-X ab Firmwareversion 1.5 (Unterscheidung des Wärmebedarfs für Kessel- oder Pumpensteuerung). Bei der Aktualisierung der FAL auf diese Firmwareversion, muss das Gerät einmal ab- und wieder angelernt werden.

  [HMCCU2-1281] Dynamische Routing-Funktionalität für den HmIP-PS/PSM ab Firmwareversion 2.x

  [HMCCU2-1242] HmIP – Die Eingabefelder für KEY und SGTIN wurden getauscht und so den Angaben auf den Gerätestickern angepasst

  [HMCCU2-1218] Der Jalousieaktor HM-LC-Ja1PBU-FM wird beim Anlernen direkt dem Gewerk Licht zugeordnet.

  [HMCCU2-1111] In den Benutzereinstellungen kann gewählt werden, ob die Servicemeldung „Gerätekommunikation war gestört“ automatisch bestätigt wird. Diese Einstellung steht nur als Administrator zur Verfügung.

  [HMCCU2-1048] HM-Sec-SIR-WM – Beim Erstellen einer direkten Verknüpfung unterscheidet die Link-Beschreibung nun zwischen internem und externem Alarm.

  [HMCCU2-820] Unter dem Punkt „Systemsteuerung/Netzwerkeinstellungen“ gibt es die Möglichkeit, ein vom Benutzer aufgespieltes Zertifikat wieder zu löschen, ohne sich per SSH Zugang auf die Zentrale verschaffen zu müssen. Der entsprechende Button wird nur angezeigt, wenn auch tatsächlich ein Zertifikat vorhanden ist.

- Fehlerbehebungen

  [HMCCU2-1322] HmIP-MIOB – Die Einheit des Levels für den analogen Ausgang (Kanal 11) innerhalb von Programmen wurde auf % gesetzt. Dadurch ist der zulässige Wertebereich statt von 0.0 -1.0 auf 0 – 100% festgelegt. Damit die Änderung wirksam wird, muss das Gerät einmal ab- und wieder angelernt werden.

  [HMCCU2-1317] Unterbindung direkter Verknüpfungen mit der internen Taste von HmIP- PS/PSM/PDT

  [HMCCU2-1314] Filtern nach Interface/Kategorie HmIP in der Geräteliste ergänzt.

  [HMCCU2-1297] HM-MOD-EM-8Bit – Die Nummerierung der Modusauswahl des Parameters „Datenübertragungsbedingungen“ wurde von 0 – 6 nach 1 – 7 geändert.

  [HMCCU2-1293] HmIP-BDT (u. a.) fehlerhafte Auswertung der Pegelbegrenzung und der Einschaltdauer bei langem Tastendruck behoben.

  [HMCCU2-1291] Link zur Hilfe zum Löschen des Browser-Caches angepasst.

  [HMCCU2-1259] Die Bearbeitung direkter Verknüpfungen zwischen virtuellen Tasten und Rollladenaktoren ergänzt

  [HMCCU2-1227] RFD beendete sich aufgrund von Speicherproblemen, wenn die Log-Datei des HM-Servers zu groß wurde.

  [HMCCU2-1226] HmIP – Hinweis auf vorhandene Programme und Verknüpfungen beim Löschen von HmIP-Geräten ergänzt.

  [HMCCU2-897] Unter Umständen kam es vor, dass die Bedienelemente einiger Dialoge
(z. B. Zusatzsoftware) nicht mehr erreichbar waren, da sie außerhalb des Screens lagen. Diese Dialoge können nun einfach mit der Maus verschoben werden, so dass die Bedienelemente wieder zugänglich sind.

  [HMCCU2-700] Testbutton für Rauchmelder-Teams entfernt.


**2.25.15**
- Fehlerbehebungen

  [HMCCU2-1257] Problem bei Verwendung von Systemvariablen innerhalb von Programmen behoben.

  [HMCCU2-1256] Ein gewähltes Profil für einen Rolladenaktor wurde unter Umständen überschrieben.


**2.25.14**
- Fehlerbehebungen

  [HMCCU2-1255] HmIP - Nutzung von Kanälen des Types KEY_TRANSMITTER (Fernbedienungen) innerhalb des Wenn-Zweiges ermöglichen.

  [HMCCU2-1254] HmIP-ASIR - Ausblenden des Kanals 1, da hier keine Funktion

  [HMCCU2-1253] Fehler beim Rückspielen eines CCU2-Backups behoben.

**2.25.12**
- Erweiterungen / Verbesserungen

  [HMCCU2-1230] Integration OSRAM-Lightify

  [HMCCU2-1190] WTH mit Fw >= 1.6 verhält sich nun wie ein WTH-2 (anlernen an HmIP-FALXXX möglich)

  [HMCCU2-1174] Integration HmIP-PDT

  [HMCCU2-1170] Integration PSM für PE, UK, IT, CH

  [HMCCU2-1163] Integration HmIP-STH Integration HmIP-STHD

  [HMCCU2-1147] Integration HM-LC-Ja1PBU-FM (Jalousieaktor mit Lamellensteuerung)

  [HMCCU2-1140] Anzeige des Endes des Urlaubsmodus für HmIP eTRV, eTRV2, WTH u. WTH-2

  [HMCCU2-1115] Integration HM-Sec-RHS-2 (Funk-Fenster-Drehgriffkontakt)

  [HMCCU2-1104] Integration Hm-MOD-EM-8Bit (8-Bit Funk-Sendemodul)

  [HMCCU2-1042] Integration HM-LC-Dim1T-DR

  [HMCCU2-1026] Integrtion HmIP-MIOB

  [HMCCU2-1022] Integration HmIP-FAL (FAL-24-6, FAL-24-10, FAL-230-6, FAL-230-10)

  [HMCCU2-1014] Integration HmIP-BDT

  [HMCCU2-1005] Integration HmIP-FSM/FSM16

  [HMCCU2-1002] Integration HmIP-ASIR (Innensirene)

  [HMCCU2-998] Integration HmIP-SMO(-A) (Bewegungsmelder, Außen)

  [HMCCU2-995] Integration HmIP-RC8 (Fernbedienung, 8-Kanal)

  [HMCCU2-993 Integration HmIP-WRC6 (Wandtaster, 6-fach)

  [HMCCU2-988] Integration HmIP-SRH (Fenstergriffsensor)

  [HMCCU2-985] Integration HmIP-BSM (Schaltaktor für Markenschalter, mit Leistungsmessung)

  [HMCCU2-1244] Easymode für rudimentäre Lamellenverstellung der Funk-Rollladenaktoren ergänzt

- Fehlerbehebungen

  [HMCCU2-1168] Die Hysterese der Temperatur war bei direkten Verknüpfungen zwischen Wandthermostaten und Aktoren als Zweipunktreglung nur noch auf ganze Grad einstellbar. Nun sind 0.1 Grad-Schritte möglich.

  [HMCCU2-1161] Bei Rolladenaktoren ließ sich beim Level kein Wert mit Nachkommastelle eingeben.

  [HMCCU2-1078] Das Verhalten des Profils „Gewünschte Temperatur“ eines HmIP-WTH bei direktenVerknüpfungen ist je nach verwendeter Firmware u. U. leicht unterschiedlich. Die Profilbeschreibung der jeweiligen Firmwareversion wurde angepasst.

  [HMCCU2-903] Bei der Erstellung einer direkten Verknüpfung zwischen einer HmIP-Fernbedienung und eines HmIP-Wandthermostaten, fehlte bei dem Profil MANU die Möglichkeit, die gewünschte Temperatur einzustellen.

**2.21.10**
- Erweiterungen / Verbesserungen

  [HMCCU2-1113] Beim HmIP-SMI ist es nun möglich, die „Bewegung erkannt“ Zeit einzustellen.

  [HMCCU2-1060] Für HmIP-Geräte steht nun Kanal 0 innerhalb von Programmen zur Verfügung. Dadurch kann nun auch mit HmIP auf bestimmte Zustände des Gerätes reagiert werden (z. B. Sabotagekontakt, Batterie leer usw.)

  [HMCCU2-1055] Stabilitätsverbesserung für HmIP

  [HMCCU2-954] Integration HM-LC-Sw1-PCB (Funk-Schaltaktor 1-fach für Kleinspannung) Bausatz/ELV-Journal

  [HMCCU2-961] Integration HM-LC-AO-SM (0 – 10V Aktor) Bausatz/ELV-Journal

  [HMCCU2-887] Integration HM-LC-Sw2PBU-FM (Funk-Schaltaktor, 2-fach für Markenschalter) Bausatz/ELV-Journal

- Fehlerbehebungen

  [HMCCU2-1142] Cron-Job für cloudmatic check von 1 Minute auf 6 Stunden geändert

  [HMCCU2-1135] Kommunikationsstörungen beim Hm-Sen-LI-O (Lichtsensor) behoben.

  [HMCCU2-1116] Beim HM-Sec-Sir-WM war bei Programmaktionen „intern scharf“ und „extern scharf“ vertauscht.

  [HMCCU2-1105] Bugfix für easy-smarthome – Den Benutzern wurden ihre Daten nach erfolgter Registrierung teilweise nicht angezeigt.

  [HMCCU2-1093] Bei Schaltaktoren wurde das Profil der internen Gerätetaste bei erneutem Aufrufen der Konfiguration von „Treppenhauslicht“ in „Schalter Ein“ geändert.

**2.19.9**
- Erweiterungen / Verbesserungen

  [HMCCU2-951] Integration HmIP-SMI (Bewegungsmelder)
  
  [HMCCU2-973] Integration HmIP-KRCA (Fernedienung Alarm)
  
  [HMCCU2-974] Integration HmIP-SWSD (Rauchmelder)
  
  [HMCCU2-779] Integration HM-WDS100-C6-o-2 (Kombi-Wettersensor)
  
  [TWIST-835]  Anzeige der Servicemeldungen von HmIP-Geräten
  
  [HMCCU2-889] Integration HM-Sec-Sir-WM (Innensirene)
  
  [HMCCU2-890] Integration HM-Dis-EP-WM55 (Statusanzeige mit E-Paper-Display)
  
- Fehlerbehebungen

  [HMCCU2-802] Gerätetausch bei Heizungsgruppen funktioniert u. U. nicht.
  
  [HMCCU2-970] Der Energiezähler HM-ES-TX-WM konnte nicht zur Verwendung in Diagrammen genutzt werden.
  
  [HMCCU2-977] Probleme bei der Erstellung einer Verknüpfung des Wetterkombisensors mit einem Rolladenaktor.
  
  [HMCCU2-1047] Der Hilfe-Button verwies auf einen toten Link
  
  [HMCCU2-1062] Der Pfad zum Navigieren im Header der Web-UI war u. U. nicht korrekt
  
  [HMCCU2-1098] Geänderter Parameter einer Verknüpfung zwischen Tastenpaar und Jalousieaktor wurde u. U. nicht übernommen. Es handelt sich dabei um den Parameter LONG_MAX_TIME_FIRST_DIR.

  Hinweis: Ist die Verknüpfung AES-gesichert, kann der Wert aus technischen Gründen nicht unter 0.8s geändert werden.

- Known Bugs

Unter Umständen bleibt die Servicemeldung "Konfigurationsdaten stehen zur Übertragung an" bei HmIP-Geräten dauerhaft bestehen, obwohl die Daten korrekt übertragen wurden.

**2.17.16**
- Erweiterungen / Verbesserungen

  * EULA angepasst
	

**2.17.15**
- Fehlerbehebungen

  [HMCCU2-958] Der Sw1PBU-FM ließ sich nicht mehr anlernen.
  
  [HMCCU2-959] Anzeige der aufsummierten Kosten der Energiezähler unter bestimmten Bedingungen um den Faktor 1000 falsch. 
    
  [HMCCU2-962] Die Verwendung der Einschaltdauer innerhalb von Programmen konnte bei den Geräten HmIP-PS/PSM zu Fehlverhalten führen. 
                
    * Die angezeigten Wochenprofile 2 und 3 der Homematic IP-Thermostate (Wand/Heizkörper) stimmten nicht mit den
      in den Geräten gespeicherten Profilen überein. Um dieses Fehlverhalten für die beiden betroffenen Profile
      zu korrigieren, müssen die betroffenen Geräte mit der CCU2-Version 2.17.15 neu angelernt werden.
                
    * Die Startreihenfolge vom Homematic und Homematic IP Server wurde synchronisiert (Stabilitätsverbesserung beim Booten der CCU2). 
               
    * Zyklische Ausgaben (alle 5 Minuten) in var/log/messages entfernt
                
    * Ein falscher Index bei bestimmten Diagrammtypen sorgte dafür, dass diese Diagramme fehlerhaft angezeigt wurden.
      Diagramme, die unter der Version 2.17.14 angelegt wurden, und folgende Datentypen enthalten, müssen in der Version 2.17.15 gelöscht und neu 
      angelegt werden. 

      Es sind folgende Datentypen betroffen:
      Windgeschwindigkeit, Windrichtung, Regen, Regenmenge, Ventilstatus, aktuelle Temperatur, Solltemperatur,
      Füllstandslevel, Energiezähler Gas u. momentaner Gasverbrauch.
                
	
2.17.14
- Erweiterungen / Verbesserungen

  [HMCCU2-792] Integration des HMOU_CFM-TW (MP3 Funk-Gong mit Signalleuchte)
  
  [HMCCU2-837] Integration des HM-Sen-LI-O (Lichtsensor)
  
  [HMCCU2-839] Integration des HM-Sec-MDIR-3 (Bewegungsmelder)
  
  [HMCCU2-883] Integration Smart-Meter-Sensor für HM-ES-TX-WM.
  
  [HMCCU2-898] Firewall-Regeln erweitert
  
  [HMCCU2-899] Integration des HM-WDS30-OT2-SM-2 (Temperaturdifferenz-Sensor).

  Support für HmIP-Geräte

    Unterstützte Geräte:
    * HmIP-PS, HmIP-PSM, HmIP-WRC2, HmIP-SWDO, HmIP-WTH, HmIP-eTRV

    Unterstützte Funktionen:
    * Konfigurierung
    * Bedienung
    * Verknüpfungen von Geräten der HmIP-Generation
    * Verwendung von HmIP-Geräten innerhalb Programmen
    * Diagramme

    Noch nicht unterstützte Funktionen:
    * Gruppen
    * Gerätetausch
    * Service-Meldungen

- Fehlerbehebungen
  
  [HMCCU2-809] Duty-Cycle-Bug behoben
  
  [HMCCU2-868] Möglicher Verbindungsabriss zum Wired-Gateway gefixt.
  
  [HMLGWOTWWEU-18] Stabilität des LAN-Gateways verbessert
  
  [EQ3_SUPPORT-5] Stabilität CCU2 Netzwerk verbessert

2.15.7
- Erweiterungen / Verbesserungen

  EULA angepasst 

2.15.6
- Erweiterungen / Verbesserungen

  Erweiterungen für eine Rückmigration von einer CCU 2 Firmware Version 2.17.X

2.15.5
- Erweiterungen / Verbesserungen
  
  [HMCCU2-769]  Integration des HM-ES-PMSw1-SM (HM-Schalt/Messaktor Aufputz)
  
  [HMCCU2-772]  Optimierung der Überprüfung auf neue Gerätefirmwaredateien.

- Fehlerbehebungen
  
  [HMCCU2-806] Die Temperaturwerte der Balkendiagramme für den Zeitraum "Monat" wurden falsch dargestellt.
  
  [HMCCU2-813] Unter bestimmten Umständen konnten keine direkten Verknüpfungen mehr angelegt werden.
  
  [HMCOP-24]   Timing Probleme beim Anlernen von Geräten bei gesetztem Systemschlüssel behoben

2.15.2
- Erweiterungen / Verbesserungen

  [HMCCU2-601]  Der Öffnungsgrad von Jalousieaktoren unter Status und Bedienung wird nun verständlicher dargestellt.
  
  [HMCCU2-699]  Bei der Zuweisung von Rauchmeldern zu Teams, wird nun, anstatt Gerätetyp und Seriennr., der Name der Rauchmeldergruppen zur Auswahl angeboten.    
  
  [HMCCU2-713]  Integration des HM-ES-PMSw1-DR (Funk-Schaltaktor mit Leistungsmessung für Hutschienenmontage.
  
  [HMCCU2-714]  Integration des HM-LC-Sw1-Pl-CT (Funk-Schaltaktor mit Klemmanschluss und spezieller Option für 0.4s Einschaltdauer). 
  
  [HMCCU2-722]  Neue Firmwareversionen vorhandener Geräte werden nun auf der Startseite angezeigt.
  
  [HMCCU2-726]  Filterhandling beim Wählen von Systemvariablen innerhalb von Programmen verbessert (Fokus bei Aufruf, Enter mittels Return, Cancel mittels ESC).
  
  [HMCCU2-734]  Integration des HMW-LC-Bl1-DR-2 (Rollladenaktor, wired, Hutschiene).
  
  [HMCCU2-736]  Menüpunkt "Geräte-Firmware" in der Gesamtübersicht der Einstellungen hinzugefügt.
  
  [HMCCU2-750]  Integration des HM-LC-RGBW-WM (Funk-RGBW-Controller für LED-Stripes).
  
  [HMCCU2-766]  Das virtuelle Gerät einer Gruppe erhalt nun den Gruppennamen.
  
  [HMCCU2-778]  Für Verknüpfungen eines Schaltaktors mit Kanal 7 des Wandthermostates HM-TC-IT-WM-W-EU, ist nun eine Hysterese einstellbar.
  
- Fehlerbehebungen
  
  [HMCCU2-733]  Alarmmeldungen wurden u. U. falsch gesetzt.
  
  [HMCCU2-742]  JSON-RPC API Formatfehler behoben.
  
  [HMCCU2-789]  Die Berechnung der Monats- und Jahreswerte von Balkendiagrammen wurde überarbeitet.
  
2.13.7
- Erweiterungen / Verbesserungen
  
  [HMCCU2-537]  Einem eingebundenen LAN-Gateway kann nun ein Name zugeordnet werden.
  
  [HMCCU2-591]  Vergleichszeitraum für Diagramme hinzugefügt.
  
  [HMCCU2-642]  Einbindung eines LAN-Gateways vereinfacht.
  
  [HMCCU2-687]  2-fach Funksender (HM-RC-2-PBU-FM) hinzugefügt.
  
  [HMCCU2-688]  Display-Fernbedienung (HM-RC-Dis-H-x-EU) hinzugefügt.
  
  [HMCCU2-690]  Darstellung des realen Dimm-Levels bei Dimmern mit virtuellen Kanälen (im Expertenmodus).
  
  [HMCCU2-692]  HM-Sec-SD-2 (Rauchmelder) hinzugefügt.
  
  [HMCCU2-695]  HM-LC-Sw1-DR (Treppenhausautomat) hinzugefügt.

- Fehlerbehebungen
  
  [HMCCU2-727]  Der Wasserstandsmelder setzt zugewiesene Alarmvariable bei Meldung von Feuchtigkeit falsch.
  
  [HMCCU2-710]  Hinweis auf bestehende Verknüpfung beim Aufruf von Kanalparametern u. U. am falschen Kanal.
  
  [HMCCU2-731]  Kommunikationsprobleme bei hoher Belastung behoben.
  
  [HMCCU2-693]  Nach Neustart der Zentrale zeigte der CCU-Zähler der Energiemessgeräte einen zu hohen Wert an.
          Um diesen Fehler zu beseitigen, ist ein Ab- und erneutes Anlernen der betroffenen Geräte nötig.
  
2.11.9
- Fehlerbehebungen
  
  [HMCCU2-681]  HM-ES-Tx-WM: keine Eingabe eines negativen Wertes beim Parameter 'Zählerempfindlichkeit' möglich.
  
  [HMCCU2-693]  HM-ES-Tx-WM: fehlerhafter CCU-Zähler nach Geräteneustart.

2.11.6
- Erweiterungen / Verbesserungen
  
  [HMCCU2-487]  Bei der Gruppenfunktion ist das automatische Umschalten von Sommer- auf Winterzeit jetzt per default aktiviert.
  
  [HMCCU2-551]  Das neue drahtlose Status Display (HM-Dis-WM55) wurde hinzugefügt.
  
  [HMCCU2-563]  HM-PB-2-WM55-2 für die Verwendung in Gruppen vorgesehen.
  
  [HMCCU2-597]  Die Kanäle des HM-MOD-EM8 können jetzt folgende Betriebsarten annehmen: Taster, Schalter, Tür-/Fensterkontakt oder nicht aktiv  
  
  [HMCCU2-615]   Der neue drahtlose Türklingel-Sensor (HM-Sen-DB-PCB) wurde hinzugefügt.
  
  [HMCCU2-616]  Der neue drahtlose Strom-/Gassensor (HM-ES-Tx-WM) wurde hinzugefügt.
  
  [HMCCU2-623]  Beim Schaltaktor mit Leistungsmessung werden die Experteneinstellungen nach der Übertragung nicht angezeigt.
  
  [HMCCU2-626]  Der neue Bewegungsmelder mit Tastenpaar (HM-Sen-MDIR-WM55) hinzugefügt.
  
  [HMCCU2-638]  Die automatische Anpassung der Y-Achse bei Diagrammen im Auto-Modus wird jetzt entsprechend der Min-/Max-Werte skaliert.
  
- Fehlerbehebungen
  
  [HMCCU2-529]  Die Überschrift der HM-SYys-sRP-Pl Parameter-Checkboxen unter Kanaleinstellungen wurde u. U. nicht angezeigt.
  
  [HMCCU2-588]  Der CSV Datenexport der Diagrammfunktion war fehlerhaft.
  
  [HMCCU2-627]  Bei der Diagrammfunktion wurden die Werte der Y-Achse u. U. (Werte größer 1000) falsch dargestellt.
  
  [HMCCU2-628]  Bei den Diagrammtypen Temperatur- u. Leistungsmessung wurden benutzerdefinierte Y-Werte ignoriert, es wurde immer 'AUTO' verwendet.
  
  [HMCCU2-632]  Benutzerdefinierte Raum- oder Gewerkenamen erschienen als Platzhalter
  
  [HMCCU2-635]  Das Hochladen einer neuen Gerätefirmwaredatei war erfolglos, wenn schon eine ältere Version vorhanden war.
  
  [HMCCU2-641]  Unter Allgemeine Geräteeinstellungen wurde beim HM-PB-4Dis-WM-2 eine falsche Gerätebezeichnung angezeigt.  
  
  [HMCCU2-656]  Bei der WinMatic war unter Zentralenprogramme die Option 'Fenster verriegeln' nicht mehr möglich.
  
2.9.12
- Erweiterungen / Verbesserungen
  
  [HMCCU2-614]  Changelog Datei bei Geräte Firmware Update Files anzeigen
  
- Fehlerbehebungen
  
  [HMCCU2-579]  Sicherheitsanforderungen der CCU2 Firewall werden nicht umgesetzt
  
  [HMCCU2-613]  Bedienung Heizkörperthermostat in Favoriten / Gewerken fehlerhaft
  
  [HMCCU2-618]  CCU2 - Favoritenansicht für HM-CC-TC ist fehlerhaft
  
  [HMCCU2-619]  Wasserstandsmelder zur Diagrammerstellung wieder hinzufügen.
  
  [HMCCU2-625]   Rolladenaktor HM-LC-BI1PBU-FM Version 2.1 kann nicht über OTAU aktualisiert werden

2.9.10
- Erweiterungen / Verbesserungen
  
  [HMCCU2-558] Der neue HomeMatic Fensterkontakt optisch (HM-SEC-SCo) wurde hinzugefügt
  
  [HMCCU2-571] Die neue HomeMatic 8-fach Fernbedienung (HM-RC-8) wurde hinzugefügt
  
  [HMCCU2-478] Der neue HomeMatic Funk-Wandtaster 2-fach für Markenschalter (HM-PB-2-FM) hinzugefügt
  
  [HMCCU2-549] Geräte Firmware Update Dateien können über die WebUI installiert werden. Ob Ihre Geräte die Over The Air Update Funktion (OTAU) unterstützen und neue Firmware Versionen vorliegen, können Sie auf der Webseite www.homematic.com unter "Downloads" überprüfen.
  
  [HMCCU2-487] Umstellung Sommer-Winterzeit bei Heizgruppen hinzugefügt
  
  [HMCCU2-509] Beim Heizkörperthermostat (HM-CC-RT-DN), Wandthermostat (HM-TC-IT-WM-W-EU) und bei Heizgruppen kann der Auto-/Manu-/Eco-/Boost- und Urlaubsmodus unter Status & Bedienung eingestellt werden
  
  [HMCCU2-562] Verzögerte Sendewiederholung bei CONFIG_PENDING für 'Permanent-Listener'. Sollten Konfigurationsänderungen nicht sofort übertragen werden, wird nach 5 bzw. 10 Sekunden erneut versucht, die Änderungen zu übertragen.
  
  [HMCCU2-603] Energiekostenanzeige beim HomeMatic Funk-Schaltaktor 1-fach mit Leistungsmessung, Zwischenstecker (HM-ES-PMSw1-Pl). Die Kosten  pro kWh können Sie unter "Einstellungen/Allgemeine Einstellunge" eintragen.
  
  [HMCCU2-379] Neue Diagramme zur Leistungsmessung (Balkendiagramme, Energieverbrauch pro Tag/Woche/Monat/Jahr)
  
- Fehlerbehebungen
  
  [HMCCU2-466] Werte im Zeitmodule werden gelöscht (1970 Problem). Ab der 2.9.10 Version werden keine Zeitmodule mehr gelöscht. Bitte kontrollieren Sie nach dem Update alle Zeitmodule und ergänzen notfalls gelöschten Einträge. Der Erste Neustart nach dem Update auf 2.9.10 kann etwas länger dauern, da alle Programme überprüft werden, ob ungültige Referenzen existieren.
  
  [HMCCU2-466] Programme lassen sich nicht mehr editieren
  
  [HMCCU2-507] HM-LGW-O-TW-W-EU Firmware Update funktioniert nicht wenn IP Adresse in WebUI konfiguriert ist
  
  [HMCCU2-508] RFD kann keine Verbindung zu HM-LGW-O-W-TW-EU aufbauen, wenn in der WebUI eine IP Adresse konfiguriert ist
  
  [HMCCU2-573] Programminhalt wird doppelt angezeigt
  
  [HMCCU2-524] Überflüssiger AES-Schlüsseltausch bei allen angelernten Geräten, die sich während aktiven Anlernmodus gemeldet haben
  
  [HMCCU2-525] Im Geräte-Posteingang funktioniert der "Löschen" Button nicht
  
  [HMCCU2-544] Zeitmodul: Gültigkeitsdauer einstellen mit IE 9 + 10 + 11
  
  [HMCCU2-547] Probleme mit Funk-LAN-Gateway und Heizkörperthermostate behoben. Nach einem LAN-Reconnect wurde die Uhrzeit nicht gesetzt
  
  [HMCCU2-561] In der Raumliste Scrollleiste hinzugefügt
  
  [HMCCU2-569] Diverse Übersetzungen hinzugefügt
  
  
2.7.17
  * [HMCCU2-522] Kommunikationsprobleme mit dem neuen HomeMatic Funk LAN Gateway (HM-LGW-O-TW-W-EU) behoben
  
2.7.16 
  * [HMCCU2-506] Wired Service stürzt ab, wenn eine IP Adresse in der WebUI angegeben wird.
  
2.7.14 Darf nicht bei Verwendung von HomeMatic Wired Geräten verwendet werden. Nähere Informationen dazu finden Sie auf der eQ-3 Webseite.
  * [HMCCU2-453] Fehlermeldungen beim HomeMatic Funk-Dimmaktor (HM-LC-Dim1PWM-CV) übersetzt 
  * [HMCCU2-443] HomeMatic Funk-Heizkörperthermostat (HM-CC-RT-DN) - Ist-Temperatur in Gewerken u. Räumen wird nicht korrekt angezeigt 
  * [HMCCU2-439] Messdatenerfassung funktioniert nach längerer Laufzeit nicht mehr korrekt
  * [HMCCU2-350] 1. und 2. interne Taste haben beim HomeMatic Funk-Rollladenaktor (HM-LC-Bl1-SM) das Profil "Experte"  
  * [HMCCU2-420] Bei der Sortierung der Geräteliste (auch im Posteingang) gehen Elemente der Seite verloren.
  * [HMCCU2-437] Nachdem der DHCP-Dienste wieder verfügbar ist, baut die Zentrale die Verbindung zu einem Wired Gateway nicht erneut auf.
  * [HMCCU2-430] Wird unter dem Windows 8.1 mit IE 11 eine neue Verknüpfung erstellt, erscheint die Auswahlliste der Geräte mit sehr großem Abstand zueinander.
  * [HMCCU2-430] Fehler 412 in WEBUI bei Benutzung vom Safari Browser
  

- Erweiterungen / Verbesserungen
  * [HMCCU2-335] Das neue HomeMatic Funk LAN Gateway (HM-LGW-O-TW-W-EU) wurde hinzugefügt
  * [HMCCU2-335] Der neue HomeMatic Wandthermostat (HM-TC-IT-WM-W-EU) wurde hinzugefügt
  * [HMCCU2-335] Der neue HomeMatic Funkschalter (HM-LC-Sw4-DR-2) wurde hinzugefügt
  * [HMCCU2-335] Der neue HomeMatic Funkschalter (HM-LC-Sw1-Pl-3) wurde hinzugefügt
  * [HMCCU2-462] Türkisches Sprachpaket hinzugefügt
  * [HMCCU2-477] Diagrammfunktion für den kapazitiven Füllstandsmesser (HM-Sen-Wa-Od) erweitert
  * [HMCCU2-476] Diagrammfunktion für den Wandthermostat (HM-TC-IT-WM-W-EU) erweitert

- Known Bugs
  * Funk LAN Gateway:
    Wenn das neue Funk LAN Gateway (HM-LGW-O-TW-W-EU) verwendet wird, muss das Gateway vor der CCU2 eingeschaltet sein. 
    Wird das Gateway erst nach der CCU2 eingeschaltet, wird das Gateway von der CCU2 nicht erkannt.
  Workaround: nicht vorhanden.
  
  * Funk LAN Gateway: 
    Ändert sich die IP Adresse des Gateways, muss die Zentrale neu gestartet werden.
    Dies ist auch der Fall, wenn nach einem zentralen Stromausfall der DHCP-Dienst nicht schnell genug zur Verfügung steht.
    Workaround: Mit dem NetFinder eine feste IP Adresse vergeben.
  
Aktuelle Informationen zu bekannten Problemen finden Sie auch im FAQ Bereich der eQ-3 Webseite (www.eq-3.de).
  
2.7.8
  * [HMCCU2-264] Simulierter Tastendruck bei Wired Geräten wird nicht ausgeführt
  * [HMCCU2-297] Programme verschwinden oder können nicht mehr bearbeitet werden
                 Beim Start der Version 2.7.8 werden Überprüfungen / Änderungen an der internen Datenbank vorgenommen. 
         Dieser Vorgang kann einigen Minuten in Anspruch nehmen. Während dieser Zeit ist die Zentrale nicht ansprechbar.
  * [HMCCU2-308] Funk-Schaltaktor mit Leistungsmessung (HM-ES-PMSw1-Pl) integrieren
  * [HMCCU2-330] Öffnungswinkel der HomeMatic Funk-Fensterantrieb WinMatic (HM-Sec-Win) wird beim IE grafisch nicht dargestellt.
  * [HMCCU2-320] SSH Zugang kann über die WebUI (Systemsteuerung/Sicherheit) aktiviert / deaktiviert werden (einschl. Passwort setzen)
  * [HMCCU2-321] HomeMatic Funk-Regensensor (HM-Sen-RD-O) - ab Firmwareversion 1.4 gibt es 4 neue Parameter. "Over The Air Update" Datei (OTAU) hinzugefügt
  * [HMCCU2-331] HomeMatic Funk-Tür-Fenster Kontakt (HM-Sec-SC-2) hinzufügen
  * [HMCCU2-333] Fenster zum Umstellen der Gewerke bzw. der Räume der im Posteingang befindlichen Geräte läßt sich nicht wieder "Schließen".
  * [HMCCU2-339] RAMP_STOP unter Programme beim HomeMatic Funk-Dimmaktor (HM-LC-Dim1T-Pl-3) nicht übersetzt.
  * [HMCCU2-340] Beim HomeMatic Funk-Dimmaktor (HM-Dim1T-Pl-3) kann kein Wertebereich größer 1 eingegeben werden.
  * [HMCCU2-358] Nach dem Hinzufügen des HomeMatic Wired RS485 LAN Gateway's (HMW-LGW-O-DR-GS-EU) wird das Logfile mit Debug Infos vollgeschrieben
  * [HMCCU2-431] Funkprobleme beim HomeMatic Funk-Heizkörperthermostat (HM-CC-RT-DN) behoben. "Over The Air Update" Datei (OTAU) hinzugefügt
  

- Erweiterungen / Verbesserungen
  * [HMCCU2-337] Messdatenerfassung und -visualisierung
           Eine genaue Funktionsbeschreibung finden Sie im WebUI Handbuch Version 3.0 (Download eQ-3 Webseite)
  * [HMCCU2-337] Heizgruppenkonzept
         Eine genaue Funktionsbeschreibung finden Sie im WebUI Handbuch Version 3.0 (Download eQ-3 Webseite)


2.5.4
- Bugfixes
  * [HMCCU2-298] Das Profil "nicht aktiv" bei interner Gerätetaste von Dimmern verursachte einen Fehler.
  * [HMCCU2-301] Easymode zwischen HomeMatic Wired RS485 Dimmakto (HMW-LC-Dim1L-DR) und HomeMatic Wired RS485 I/O-Modul (HMW-IO-4-FM) zeigte eine leere Seite
  * [HMCCU2-302] Der Hinweis zur Länge des Sicherheitsschlüssel wurde korrigiert.
  * [HMCCU2-305] Bei Verwendung bestimmter Variablennamen innerhalb von Scripts, wurde das Script ungültig.
  * [HMCCU2-311] EasyMode zwischen HomeMatic Funk-Dimmaktor (HM-LC-Dim1TPBU-FM) und Virtuellem CCU2-Kanal zeigte eine leere Seite.
  * [HMCCU2-314] Die Hilfe-Funktion einer Verknüpfung zwischen einem Bewegungsmelder und der WinMatic war fehlerhaft.

- Erweiterungen / Verbesserungen
  * [HMCCU2-276] Der neue HomeMatic Heizkörperthermostat (HM-CC-RT-DN) wurde hinzugefügt.
  * [HMCCU2-319] Bei der Sprache der WebUI kann benutzerabhängig zwischen Deutsch u. Englisch gewählt werden.

  
2.3.18
- Bugfixes
  * [HMCCU2-297] Stabilität beim Betrieb komplexer Installationen verbessert.

  
2.3.17
- Bugfixes
  * [HMCCU2-254] Innerhalb von Programmen mit Rollladenaktoren kommt das Wort "Behanghöhe" doppelt vor.
  * [HMCCU2-257] Info LED signalisiert keine Alarmmeldungen.
  * [HMCCU2-258] Wandthermostat zeigt einen Zeitunterschied von ungefähr 5 Minuten an.
  * [HMCCU2-260] Wired Service (hs485d) schreibt Debug als Error raus.
  * [HMCCU2-263] °C wird innerhalb des Expertenmodus der Easymodes falsch dargestellt.
  * [HMCCU2-288] Zeitunterschied zwischen Wandthermostat und CCU2 steigt kontinuierlich.

