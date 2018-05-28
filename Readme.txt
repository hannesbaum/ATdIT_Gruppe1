
-----------------------------------------------------------------------------------

Datei in Eclipse öffnen (in unserem Testbeispiel wurde Eclipse Oxygen genutzt, Kompatibilität mit älternen Versionen ist nicht garantiert):

Der simulierte Server muss parallel in einem Programm wie Eclipse geöffnet werden.

Auszuwählen ist hierbei der Ordner Server_v0.9.zip

In der Unterstruktur ist für die Ausführung das Projekt unter src/Projekt_Server relevant.

Zunächst muss die Datenbank erzeugt werden, dazu muss lediglich die Datei CreateDB2.java ausgeführt werden.

Bei einer erfolgreichen Ausführung werden in der Konsole einige Dateninhalte ausgegeben.

Nun muss der Server gestartet werden. Hierfür muss nur die Klasse "Server.java" ausgefürt werden. Wichtig dabei ist,

dass diese nicht durch die Firewall des Computers gesperrt ist.

Obwohl die Einstellungen bereits im Dateiordner entsprechend angepasst wurden, kann es sein, dass die externen Bibliotheken nicht erkannt werden.

Hierzu müssen die drei folgenden jar.-Dateien dem Buildpath des Projektes hinzugefügt werden.

- JUnit 5
- sqlite-jdbc-3.21.0.jar
- gson-2.6.2.jar

Alle Dateien befinden sich im Github.

Um die Bibliotheken hinzuzufügen, einfach in Eclipse per Rechtsklick unter BuildPath -> Configure Build Path den Reiter Libraries auswählen und über

"Add External JARs" die SQLite und Gson dateien hinzufügen. JUnit 5 ist in Eclipse schon vorhanden.

Nachdem der Server gestartet wurde kann die App in AndroidStudio gestartet werden und die Verbindung wird aufgebaut.


-----------------------------------------------------------------------------------

Installationsguide und Setup für AndroidStudio

Download AndroidStudio unter der folgenden URL:

https://developer.android.com/studio/


Installieren Sie AndroidStudio indem der angegebene Guide durchlaufen wird.

Zum Öffnen der App in AdroidStudio müssen folgende Grudlagen gegeben sein:

Der Ordner App_v0.9.zip muss entpackt und lokal gespeichert werden.

In diesem Ordner müssen sich zwei Unterordner befinden, einmal "libs" und einmal "src"

"Src" enthält logischerweise den Quelltext für die App, in drei weiteren Unterordnern.

Wichtig für die App ist jedoch, dass im "libs" Ordner die Datei "gson-2.6.2.jar" liegt.

Sollte diese Datei !NICHT! im Ordner liegen, kann diese unter der folgenden URl heruntergeladen werden:

https://repo1.maven.org/maven2/com/google/code/gson/gson/2.6.2/


Beim ersten Start von Android Studio kann es vorkommen, dass die Applikation diverse Daten aus dem Internet nachlädt.

Sobald die App bereit ist, kann das Projekt in das Programm geladen werden.

Nachdem die App geladen wurde, muss sie zunächst einmal den "Build"-Prozess durchlaufen.

Dazu entweder in der Menüleiste Build -> Make Project auswählen oder Strg + F9 drücken.

Nachdem der Build erfolgreich abgeschlossen wurde, kann nun der Emulator eingestellt werden.

Sollte das Build unplanmäßig scheitern, kontaktieren Sie bitte erneut die Gruppe.

Nun kann die App in einem programmeigenen Emulator getestet werden. 

Öffnen Sie dazu im "demoapp" - Ordner die Datei "MainActivity".

Im Menü unter Run -> Run MainActivity kann nun ein Endgerät selektiert werden (ggf. unter "Create new virtual device").

Wählen Sie hier bitte unter "Phone" das Nexus 6P mit der API Version 27 (Oreo) aus.

Die App wird nun auf dem ausgewählten Gerät simuliert und kann wie ein normales Handy bedient werden.

Bitte beachten Sie, dass gerade das Starten des Emulators am Anfang einige Minuten in Anspruch nehmen kann.









