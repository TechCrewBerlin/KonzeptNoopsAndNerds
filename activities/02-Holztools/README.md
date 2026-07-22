# Noops & Nerds
## Aktivität: Holztools

Im Spiel Minecraft nutzen die Spielfiguren Werkzeuge aus unterschiedlichen Materialien. Wir bauen diese mit den Kinder aus Holz nach.

Es gibt:
* Schwerter (zum Kämpfen!)
* Spitzhacken (um Stein abzubauen - sehr wichtig!)
* Äxte (zum Holzfällen und auch zum kämpfen)
* Schaufeln (um Erde und Sand abzubauen)
* Harken (Um Beete zu bauen)

Ich habe diese aus Pappe, dünnem Sperrholz und auch großformatig umgesetzt. Sehr schön kann man die Modelle mit Acrylfarben colorieren. Wer möchte kann sie abschließed mit Lösungsmittelhaltigem Lack versiegeln.

TODO Detaillierte Anleitung folgt hier noch.

## Resourcen
### Original Minecraft Texturen

In diesem Verzeichnis findet Ihr Vorlagen, um selber Minecraft Holztools zu erstellen.

Im Order "textures" finden sich die exemplarisch einige Beispile von original Texturen aus dem Spiel in Normalgröße und 50-fach vergrößert. Die .xcf Dateien sind Gimp Bilddateien dazu.

Ihr könnt aber auch sehr einfach in der Minecraft-Java Programmdatei auch alle Texturen extrahieren und selber einmal schauen, was Euch als Vorlage dazu attraktiv erscheint. Die Datei minecraft.jar ist ein Zip-Archiv und kann mit entsprechenden Tools einfach ausgepackt werden.

Danach finden sich die Texturen in folgenden Unterverzeichnissen:
* Werkzeuge, wie Äxte, Schwerter: <pre>assets/minecraft/textures/item/</pre>
* Blumen und vieles andere in: <pre>assets/minecraft/textures/block/</pre>

Mit den folgenden Befehlen - je nach verwendetem Betriebssystem - könnt Ihr die Minecraft-Java Programmdatei herunterladen (kostenlos) und die Texturen selber extrahieren:

#### LINUX (Bash)

<pre>
cd ~/textures
wget https://github.com/minecraft-java-edition/resources/archive/refs/tags/1.20.1.zip
unzip 1.20.1.zip
cd resources-1.20.1
ls assets/minecraft/textures/
</pre>

#### MACOS (Bash/Zsh)

<pre>
cd ~/textures
curl -L -o 1.20.1.zip https://github.com/minecraft-java-edition/resources/archive/refs/tags/1.20.1.zip
unzip 1.20.1.zip
cd resources-1.20.1
ls assets/minecraft/textures/
</pre>

# W###INDOWS (PowerShell)

<pre>
cd $env:USERPROFILE\textures
Invoke-WebRequest -Uri "https://github.com/minecraft-java-edition/resources/archive/refs/tags/1.20.1.zip" -OutFile "1.20.1.zip"
Expand-Archive -Path "1.20.1.zip" -DestinationPath "."
cd resources-1.20.1
dir assets\minecraft\textures
</pre>

#### WINDOWS (CMD/Batch)

<pre>
cd %USERPROFILE%\textures
powershell -Command "Invoke-WebRequest -Uri 'https://github.com/minecraft-java-edition/resources/archive/refs/tags/1.20.1.zip' -OutFile '1.20.1.zip'"
powershell -Command "Expand-Archive -Path '1.20.1.zip' -DestinationPath '.'"
cd resources-1.20.1
dir assets\minecraft\textures
</pre>








### Linux (Original Microsoft Minecraft Launcher)



### Linux (Modrinth Launcher via Flatpak)


Ersetze <VERSION> durch die jeweilige Minecraft-Version (z.B. 1.20.1)


## Schritt 2: Texturen extrahieren

Die Datei minecraft.jar ist ein ZIP-Archiv. Mit den folgenden Kommandos kannst du alle Texturen entpacken:

### Windows (PowerShell)

Expand-Archive -Path "path\to\minecraft.jar" -DestinationPath "minecraft_extracted"

Oder mit 7-Zip:

7z x minecraft.jar -o minecraft_extracted


### macOS

unzip minecraft.jar -d minecraft_extracted


### Linux

unzip minecraft.jar -d minecraft_extracted

oder

jar xf minecraft.jar


## Schritt 3: Texturen finden

Die extrahierten Texturen befinden sich im Ordner:

minecraft_extracted/assets/minecraft/textures/


## Referenzmaterial im Projekt

Im Ordner textures/ dieses Projekts findest du exemplarisch einige Original-Texturen aus dem Spiel in:

- Normalgroesse (16x16 Pixel)
- 50-fach vergroessert fuer bessere Bearbeitbarkeit

Die entsprechenden .xcf-Dateien sind GIMP-Bilddateien zur weiteren Bearbeitung.


## Tipps zur Bearbeitung

- Oeffne die .xcf-Dateien in GIMP
- Verwende die vergroesserten Versionen als Vorlage
- Beachte die Minecraft-typische Pixelart-Aesthetik
- Speichere deine Arbeiten als PNG ab

---

Hinweis: Die genauen Pfade koennen je nach Minecraft-Version und Launcher leicht variieren.


## Lizenz

Copyright (C) 2026 Melanie Desaive

Dieses Projekt ist lizenziert unter der **GNU General Public License Version 3 (GPLv3)**.

Du darfst die Inhalte dieses Repositories frei nutzen, verändern und weitergeben, solange:

- der Copyright-Hinweis erhalten bleibt,
- abgeleitete Werke ebenfalls unter der GPLv3 veröffentlicht werden,
- der vollständige Lizenztext beigefügt oder verlinkt wird.

Den vollständigen Lizenztext findest du in der Datei [`LICENSE`](LICENSE) oder unter:  
https://www.gnu.org/licenses/gpl-3.0.txt

---

## Kontakt & Mitarbeit

Korrekturen, Anmerkungen und Beiträge sind ausdrücklich erwünscht – ganz im Sinne der GPLv3.  
Melde dich gerne per Issue oder direkt unter **melanie@desaive.de**.
