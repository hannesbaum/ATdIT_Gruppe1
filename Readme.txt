
-----------------------------------------------------------------------------------

Datei in Eclipse �ffnen (in unserem Testbeispiel wurde Eclipse Oxygen genutzt, Kompatibilit�t mit �lternen Versionen ist nicht garantiert):


Hierzu muss zun�chst die Server_v0.9.zip entpackt werden.

Unter File-> Open Project from File System das Server Projekt (entpackte Zip-Datei) in die Eclipse laden.

Am besten daf�r den Unterordner ATdIT_Projekt ausw�hlen.

Im File Explorer ist der Quelltext dann unter src -> Projekt_Server zu finden.

Nun m�ssen die folgenden jar.-Dateien dem Buildpath des Projektes hinzugef�gt werden.

- sqlite-jdbc-3.21.0.jar
- gson-2.6.2.jar

Alle Dateien befinden sich im Github.

Um die Bibliotheken hinzuzuf�gen, einfach in Eclipse per Rechtsklick unter BuildPath -> Configure Build Path den Reiter Libraries ausw�hlen und �ber

"Add External JARs" die SQLite und Gson dateien hinzuf�gen.

JUnit 5 ist in Eclipse schon vorhanden.

Zun�chst muss die Datenbank erzeugt werden, dazu muss lediglich die Datei CreateDB2.java ausgef�hrt werden.

Bei einer erfolgreichen Ausf�hrung werden in der Konsole einige Dateninhalte ausgegeben.

Nun muss der Server gestartet werden. Hierf�r muss nur die Klasse "Server.java" ausgef�rt werden. Wichtig dabei ist,

dass diese nicht durch die Firewall des Computers gesperrt ist.

Obwohl die Einstellungen bereits im Dateiordner entsprechend angepasst wurden, kann es sein, dass die externen Bibliotheken nicht erkannt werden.


Nachdem der Server gestartet (Statusmeldung: "Server gestartet" in der Konsole) wurde kann die App in AndroidStudio gestartet werden und die Verbindung wird aufgebaut.


-----------------------------------------------------------------------------------

Installationsguide und Setup f�r AndroidStudio

Download AndroidStudio unter der folgenden URL:

https://developer.android.com/studio/


Installieren Sie AndroidStudio indem der angegebene Guide durchlaufen wird.

Der Download und die Installation k�nnen einige Zeit in Anspruch nehmen.

Zum �ffnen der App in AdroidStudio m�ssen folgende Grudlagen gegeben sein:

Der Ordner App_v0.9.zip muss entpackt und lokal gespeichert werden.

In diesem Ordner m�ssen sich zwei Unterordner befinden, einmal "libs" und einmal "src"

"Src" enth�lt logischerweise den Quelltext f�r die App, in drei weiteren Unterordnern.

Wichtig f�r die App ist jedoch, dass im "libs" Ordner die Datei "gson-2.6.2.jar" liegt.

Sollte die Datei nicht im angegebenen Ordner liegen, ist sie manuell �ber das Git herunterzuladen und dort zu platzieren.

Beim ersten Start von Android Studio kann es vorkommen, dass die Applikation diverse Daten aus dem Internet nachl�dt.



Sobald die App bereit ist, kann das Projekt in das Programm geladen werden.

Beim ersten Start von Android Studio am besten unter "Open existing project" das Projekt ausw�hlen.

Nachdem die App geladen wurde, muss sie zun�chst einmal den "Build"-Prozess durchlaufen.

Dazu entweder in der Men�leiste Build -> Make Project ausw�hlen oder Strg + F9 dr�cken.

Nachdem der Build erfolgreich abgeschlossen wurde, kann nun der Emulator eingestellt werden.

(Sollte das Build unplanm��ig scheitern, kontaktieren Sie bitte erneut die Gruppe.)

�ffnen Sie dazu im app -> java "...demoapp" - Ordner die Datei "MainActivity".

Im Men� unter Run -> Run MainActivity (ggf. auf Run -> Run app) kann nun ein Endger�t selektiert werden (ggf. unter "Create new virtual device").

W�hlen Sie hier bitte unter "Phone" das Nexus 6P mit der API Version 27 (Oreo) aus.

Die App wird nun auf dem ausgew�hlten Ger�t simuliert (App wird automatisch gestartet) und kann wie ein normales Handy bedient werden.

Bitte beachten Sie, dass gerade das Starten des Emulators am Anfang einige Minuten in Anspruch nehmen kann.








