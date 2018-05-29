
-----------------------------------------------------------------------------------

Datei in Eclipse öffnen (in unserem Testbeispiel wurde Eclipse Oxygen genutzt, Kompatibilität mit älternen Versionen ist nicht garantiert):


Hierzu muss zunächst die Server_v0.9.zip entpackt werden.

Unter File-> Open Project from File System das Server Projekt (entpackte Zip-Datei) in die Eclipse laden.

Am besten dafür den Unterordner ATdIT_Projekt auswählen.

Im File Explorer ist der Quelltext dann unter src -> Projekt_Server zu finden.

Nun müssen die folgenden jar.-Dateien dem Buildpath des Projektes hinzugefügt werden.

- sqlite-jdbc-3.21.0.jar
- gson-2.6.2.jar

Alle Dateien befinden sich im Github.

Um die Bibliotheken hinzuzufügen, einfach in Eclipse per Rechtsklick unter BuildPath -> Configure Build Path den Reiter Libraries auswählen und über

"Add External JARs" die SQLite und Gson dateien hinzufügen.

JUnit 5 ist in Eclipse schon vorhanden.

Zunächst muss die Datenbank erzeugt werden, dazu muss lediglich die Datei CreateDB2.java ausgeführt werden.

Bei einer erfolgreichen Ausführung werden in der Konsole einige Dateninhalte ausgegeben.

Nun muss der Server gestartet werden. Hierfür muss nur die Klasse "Server.java" ausgefürt werden. Wichtig dabei ist,

dass diese nicht durch die Firewall des Computers gesperrt ist.

Obwohl die Einstellungen bereits im Dateiordner entsprechend angepasst wurden, kann es sein, dass die externen Bibliotheken nicht erkannt werden.


Nachdem der Server gestartet (Statusmeldung: "Server gestartet" in der Konsole) wurde kann die App in AndroidStudio gestartet werden und die Verbindung wird aufgebaut.


-----------------------------------------------------------------------------------

Installationsguide und Setup für AndroidStudio

Download AndroidStudio unter der folgenden URL:

https://developer.android.com/studio/


Installieren Sie AndroidStudio indem der angegebene Guide durchlaufen wird.

Der Download und die Installation können einige Zeit in Anspruch nehmen.

Zum Öffnen der App in AdroidStudio müssen folgende Grudlagen gegeben sein:

Der Ordner App_v0.9.zip muss entpackt und lokal gespeichert werden.

In diesem Ordner müssen sich zwei Unterordner befinden, einmal "libs" und einmal "src"

"Src" enthält logischerweise den Quelltext für die App, in drei weiteren Unterordnern.

Wichtig für die App ist jedoch, dass im "libs" Ordner die Datei "gson-2.6.2.jar" liegt.

Sollte die Datei nicht im angegebenen Ordner liegen, ist sie manuell über das Git herunterzuladen und dort zu platzieren.

Beim ersten Start von Android Studio kann es vorkommen, dass die Applikation diverse Daten aus dem Internet nachlädt.



Sobald die App bereit ist, kann das Projekt in das Programm geladen werden.

Beim ersten Start von Android Studio am besten unter "Open existing project" das Projekt auswählen.

Nachdem die App geladen wurde, muss sie zunächst einmal den "Build"-Prozess durchlaufen.

Dazu entweder in der Menüleiste Build -> Make Project auswählen oder Strg + F9 drücken.

Nachdem der Build erfolgreich abgeschlossen wurde, kann nun der Emulator eingestellt werden.

(Sollte das Build unplanmäßig scheitern, kontaktieren Sie bitte erneut die Gruppe.)

Öffnen Sie dazu im app -> java "...demoapp" - Ordner die Datei "MainActivity".

Im Menü unter Run -> Run MainActivity (ggf. auf Run -> Run app) kann nun ein Endgerät selektiert werden (ggf. unter "Create new virtual device").

Wählen Sie hier bitte unter "Phone" das Nexus 6P mit der API Version 27 (Oreo) aus.

Die App wird nun auf dem ausgewählten Gerät simuliert (App wird automatisch gestartet) und kann wie ein normales Handy bedient werden.

Bitte beachten Sie, dass gerade das Starten des Emulators am Anfang einige Minuten in Anspruch nehmen kann.








