Die Dateien enthalten die Pfade zu den .jar Dateien.
Das ist 1 Zeile. Die Einträge sind mit Semikolon getrennt.

Wenn es ein Maven - Projekt ist, kann die Datei automatisiert aus pom.xml erstellt wird
"start Maven..."

und als Goals eingeben: 
generate-resources

Merke: 
Die Maven build Dateien können in diesen Ordner abgelegt werden: buildZZZ
Wie so eine Maven Datei aussieht, wird dort im 1readmeFGL.txt beschrieben.

Merke:
Es gilt für Dateien unterhalb des target - Verzeichnisses: 
Sie gehören nicht in git eingecheckt.
Die Pfade können auf jeder Maschine anders sein.

Ausnahmen:
Diese readme-Datei 
und die Datei classpathOfLibrariesWorkspaceZZZ.txt, diese gibt die Pfade relativ zum Workspace an.
Man findet den Pfad unter: 
Projekteigenschaften/Java Build Path. Reiter Libraries.
Hier die Library als Kategorie aufklappen. 
Leider kann man da nichts Rauskopieren.

#########################################################
Mit den Angaben in diesen classpath...ZZZ Dateien können die notwendigen .jar Dateien 
in anderen Tools geladen werden. Z.B. Classpathloader meiner Jython Lösung.

Dabei gilt: 
Normalerweise immer absolute Pfadangaben, nur beim classpathOfLibrariesWorkspaceZZZ.txt
bezieht sich die Angabe auf den Workspace, d.h. hier relative Pfadangaben
