# Frau Mileys personal cheat sheet
Hallo Frau Miley, <img align="right" src="https://mobaxterm.mobatek.net/img/moba/xterm_logo.png">

jede Entwicklerin braucht ein Github Account, um coolen Code von sich zu teilen. Ich bin mir sicher Du kannst ihn gut brauchen :smiley:

Mit dem Cheatsheet hab ich schonmal den Anfang gemacht. Wenn Du mal wieder "mit dem schwarzen Loch" nicht mehr weiter weißt, dann findest Du hier ein Rat. Bei Deiner neuen Firma kannst Du dann gleich mit mobaXterm beeindrucken.  

Dir alles Gut für Deine Zukunft und ich hoffe wir hören wieder voneinander.:hugs:  

Grüße, Florian  
## *nix
`|` Ausgabestrom in nächsten Befehl umleiten  
`> datei.*` Ausgabestrom in Datei schreiben (inhalt wird ersetzt)  
`>> datei.*` Ausgabestrom in Datei anhängen / drunter schreiben (inhalt bleibt erhalten)  
`2>&1` Fehlerausgabestrom und Ausgabestrom zusammenführen. Ausgabestrom wird standardmäßig angezeigt  
`Befehl1 && Befehl2` Führt Befehl1 und Befehl2 aus, wenn Befehl1 erfolgreich war  
`Befehl1 ; Befehl2` Führt Befehl1 und Befehl2 aus, auch wenn Befehl1 nicht erfolgreich war  
`sort` Liste sortieren  
`uniq` alle duplikate aus einer Liste entfernen  
`wc -l` Zeilen zählen  
## less
> damit geht wirklich jede Datei auf. Egal wie groß.

`less datei.*`   
`less -S datei.*` Kein Zeilenumbruch   
`g` Anfang der Datei  
`G` Ganz nach unten  
`/` suchen von oben nach unten  
`?` suchen von unten nach oben  
`n` next suchtreffer  
`p` previous suchtreffer  
`q` quit  
## grep
> ich kann dateien durchsuchen ohne sie zu öffnen. Das ist so krass

`grep "wasIchSuche" datei.*` sucht in Datei nach: wasIchSuche  
ausserdem gibt es noch zgrep: Durchsuchen von Textdateien in *.gz Containern. Wichtig: Es darf kein tar drin sein.  
ausserdem gibt es noch egrep: Durchsuchen von Textdateien mit erweitertem Suchpattern  
## tail
`tail -f datei.*` so kannst Du logs "folgen" und dem Programm bei der Arbeit zuschauen  
`tail -n 10 datei.*` zeigt die letzten 10 Zeilen der Datei an. Kannst Du mit -f kombinieren  
## iconv
`iconv -f ISO88592 -t UTF8 < input.txt > output.txt`  
