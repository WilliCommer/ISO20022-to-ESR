# ISO200222-to-ESR
Convert ISO20022 camt.054.xml to ESR files ESR Gutschriften Einzahlungsscheine

## Was kann das Programm
Sie benutzen E-Banking-Datentransfer f�r ESR-Gutschriften um Einzahlungsscheine in Ihre Software zu importieren.
Nun hat die Post das Dateiformat ge�ndert und liefert die Daten im XML-Format in einer camt.054.xml Datei.
Mit dem Programm ISO20022toESR k�nnen die Dateien in das alte Format konvertiert werden.


## Wie wird das Programm verwendet
ISO20022toESR ist eine Konsolenanwendung f�r Windows. Die zu konvertierenden Dateien werden als Aufrufparameter �bergeben.
```
ISO20022toESR C:\users\user\desktop\camt_054_ZA1_ESR_ZE.xml
```

Es kann auch ein Ordner �bergeben werden, dann werden alle XML-Dateien in diesem Ordner konvertiert.
```
ISO20022toESR C:\users\user\desktop\Gutschriften
```

Alternativ zum Konsolenaufruf k�nnen Sie eine oder mehrere Dateien oder einen Ordner mit der Maus auf das Programmsymbol ziehen.

Die ESR Dateien werden als .txt Dateien in den gleichen Ordner wie die Quelldateien geschrieben.


## Wie kann ich das Programm konfigurieren
In der Datei ISO20022toESR.ini k�nnen einige Einstellungen vorgenommen werden.

##### BESRFileExtension
Mit dieser Einstellung kann die Dateierweiterung der Zieldateien eingestellt werden. Standard ist
```
BESRFileExtension=.txt
```
Sollen die Dateien als CSV-Dateien gespeichert werden, �ndern Sie den Eintrag in
```
BESRFileExtension=.csv
```

##### BESROutputDirectory
M�chten Sie die Zieldateien in einem Ordner sammeln, dann benutzen Sie diese Einstellung.
Per Standard ist die Einstellung leer und die Zieldateien werden im gleichen Ordner wie die Quelldateien geschrieben.

Mit dieser Einstellung werden die Zieldateien in den Ordner "Gutschriften" auf dem Desktop geschrieben
```
BESROutputDirectory=C:\users\user\desktop\Gutschriften
```

##### XMLFileFilter
Wenn ein Ordner als Quelle verwendet wird, werden alle XML-Dateien in diesem Ordner konvertiert (*.xml).
Mit dieser Einstellung kann der Dateifilter ge�ndert werden.
Um z.B. nur Dateien die mit "camt" beginnen zu konvertieren �ndern Sie die Einstellung in
```
XMLFileFilter=camt*.xml
```

##### WaitForUser
Nach der Konvertierung wartet das Programm bis der User die Enter-Taste gedr�ckt hat.
Das kann mit dieser Einstellung abgeschaltet werden
```
WaitForUser=false
```

## Wer steckt hinter dem Programm
Das Programm ist von Willi Commer, Frohnrather Weg 6, D-53925 Kall

mail: support@willicommer.de

Die aktuelle Version finden Sie [auf GitHub](http://github.com/WilliCommer/ISO200222-to-ESR/)

Wenn Ihnen das Programm gef�llt oder sogar Geld spart weil Sie Ihre Software nicht �ndern m�ssen, dann �berweisen Sie eine Spende auf dieses Konto:
IBAN: DE42 3825 0110 008 5307 01
BIC: WELADED1EUS





