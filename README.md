# asvushelper_untis_import

Das Tool erzeugt aus der Untis-Exportdatei für ASV Bayern (STDPLAN.txt) einen STDPLAN.txt für einen bestimmten Kollegen.
Man kann dann diesen einzelnen Kollegen in die ASV importieren, um zu prüfen, ob alle Stunden genau ankommen.

Vorteil:
Es ist nur dieser Kollege in der Unterrichtsmatrix enthalten. (Option im ASV-Dialog zum Import: Stunden löschen muss gewählt werden.)

Voraussetzung für die Nutzung:
1. Die STDPLAN.txt aus Untis muss in STDPLANVorlage.txt umbenannt werden.
2. STDPLANVorlage.txt muss auf dem Windows Desktop liegen.
3. Das Programm selbst kann im Prinzip in jedem Ordner gespeichert werden.
4. Das Programm muss aus einer Eingabeaufforderung ausgeführt werden. Der Pfad der Eingabeaufforderung muss auf den Ordner zeigen, in dem das Programm gespeichert wurde.

Ausführung:
asvushelper_untis_import.exe Mx (Mx = Lehrerkürzel in Untis)

Ausgabe:
Auf dem Desktop wird dann eine STDPLAN.txt erzeugt, welche mit jeder Ausführung des Programms überschrieben wird. Der Inhalt wird gleichzeit in der Eingabeaufforderung ausgegeben 
und kann dann zur Kontrolle genutzt werden.

Haftungsausschluss:
Das Programm wurde mit Rust geschrieben und zu einer .exe compiliert. Ob der PC bestimmte Voraussetzungen erfüllen muss, um das Programm auszuführen entzieht sich meiner Kenntnis.
Das Programm überschreibt ohne Warnung die STDPLAN.txt. Sollte kein Lehrerkürzel angegeben werden, dann gibt es eine Fehlermeldung. Sollte Untis die Datenreihung der 1. Zeile ändern, 
dann funktioniert der Import nach ASV nicht mehr. 
