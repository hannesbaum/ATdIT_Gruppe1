
-----------------------------------------------------------------------------------

Datei in Eclipse �ffnen:

Der simulierter Server muss parallel in einem Programm wie Eclipse ge�ffnet werden.

Auszuw�hlen ist hierbei der Ordner <<Ordername Server>>

Zun�chst muss die Datenbank erzeugt werden, dazu muss lediglich die Datei CreateDB.java ausgef�hrt werden.

Bei einer erfolgreichen Ausf�hrung werden in der Konsole einige Dateninhalte ausgegeben.

Nun muss der Server gestartet werden. Hierf�r muss nur die Klasse "Server.java" ausgef�rt werden. Wichtig dabei ist,

dass diese nicht durch die Firewall des Computers gesperrt ist.

Obwohl die Einstellungen bereits im Dateiordner entsprechend angepasst wurden, kann es sein, dass die externen Bibliotheken nicht erkannt werden.

Hierzu m�ssen die drei folgenden jar.-Dateien dem Buildpath des Projektes hinzugef�gt werden.

- JUnit 5
- sqlite-jdbc-3.21.0.jar
- gson-2.6.2.jar

Alle Dateien befinden sich im Projektordner!

Nachdem der Server gestartet wurde kann die App in AnroidStudio gestartet werden und die Verbindung wird aufgebaut.


-----------------------------------------------------------------------------------

Installationsguide und Setup f�r AndroidStudio

Download AndroidStudio unter der folgenden URL:

https://developer.android.com/studio/


Installieren Sie AndroidStudio indem der angegebene Guide durchlaufen wird.

Zum �ffnen der App in AdroidStudio m�ssen folgende Grudlagen gegeben sein:

Der Ordner <<Ordnername f�r App-Code>> muss entpackt und lokal gespeichert werden.

In diesem Ordner m�ssen sich zwei Unterordner befinden, einmal "libs" und einmal "src"

"Src" enth�lt logischerweise den Quelltext f�r die App, in drei weiteren Unterordnern.

Wichtig f�r die App ist jedoch, dass im "libs" Ordner die Datei "gson-2.6.2.jar" liegt.

Sollte diese Datei !NICHT! im Ordner liegen, kann diese unter der folgenden URl heruntergeladen werden:

https://repo1.maven.org/maven2/com/google/code/gson/gson/2.6.2/


Beim ersten Start von Android Studio kann es vorkommen, dass die Applikation diverse Daten aus dem Internet nachl�dt.

Sobald die App bereit ist, kann das Projekt in das Programm geladen werden.

Nachdem die App geladen wurde, muss sie zun�chst einmal den "Build"-Prozess durchlaufen.

Dazu entweder in der Men�leiste Build -> Make Project ausw�hlen oder Strg + F9 dr�cken.

Nachdem der Build erfolgreich abgeschlossen wurde, kann nun der Emulator eingestellt werden.

Sollte das Build unplanm��ig scheitern, kontaktieren Sie bitte erneut die Gruppe.

Nun kann die App in einem programmeigenen Emulator getestet werden. 

�ffnen Sie dazu im "demoapp" - Ordner die Datei "MainActivity".

Im Men� unter Run -> Run MainActivity kann nun ein Endger�t selektiert werden (ggf. unter "Create new virtual device").

W�hlen Sie hier bitte unter "Phone" das Nexus 6P mit der API Version 27 (Oreo) aus.

Die App wird nun auf dem ausgew�hlten Ger�t simuliert und kann wie ein normales Handy bedient werden.

Bitte beachten Sie, dass gerade das Starten des Emulators am Anfang einige Minuten in Anspruch nehmen kann.









