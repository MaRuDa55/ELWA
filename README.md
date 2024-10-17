Programm zur Kommunikation mit dem ELWA(DC) Heizstab von MyPV
über das (optionale) my-PV USB-Interface für alle ELWA Geräte 

Folgende Daten können ausgelesen werden:
- aktuelle Betriebsdaten (ohne Wartezeit, anders als bei der Software ELWA V1_07.exe)
- Tagesdaten je Betriebstag
- Viertelstundenwerte für Temperatur und Leistung
  (ohne Diagramme)

Das Programm habe ich entwickelt weil nach einem Jahr das schnelle Auslesen der Betriebsdaten praktisch kaum noch möglich war.
Grund:
Beim Programm des Herstellers MyPv wurden immer erst die Historiendaten komplett geladen, 
was zu langen Wartezeiten (> 15min) auf die ersten Betriebsdaten führte.

Gern nehme ich Hinweise zur Verbesserung an - oder stelle ggf. auch die Quellen zur Verfügung
(VisualStudio 2022 / VB)

Martin Ruß, April 2024

Please feel free to contact me: github@russ-web.de

Bedienung des Programms:
1. Schaltfläche "COM-Port suchen" betätigen und danach in der darunterliegenden ComboBox den COM-Port auswählen.
   (bei Erfolg gibt es ein grünes "Signal")
2. danach können die weiteren Schaltflächen genutzt werden
   - "Akt. Betriebsdaten" werden im Intervall von 2 Sekunden aktualisiert. Intervall variabel wählbar

   - "Day power data": Anzeige der Solarleistung im Viertelstundenintervall (keine Auswertung)

   - "Day temp data": Anzeige der Wassertemperatur im Viertelstundenintervall (keine Auswertung)

   - "DataLog": Auslesen der Leistungsdaten je Betriebstag
      hier bitte den Betriebstag einstellen, ab dem die Daten in die Textbox übertragen werden sollen
      Achtung: wenn man ab Betriebstag 1 beginnt kann es sehr lange dauern (mehrere Minuten) bis die gelbe Schaltfläche
      auf grün switcht und das Ende der Übertragung anzeigt.
      Daten können Über die Zwischenablage (Strg+A / Strg+C) in eine Tabellenkalkulation importiert werden
     
