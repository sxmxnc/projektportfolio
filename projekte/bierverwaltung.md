# Bierverwaltung

[Quellcode und Startanleitung](https://github.com/sxmxnc/bierverwaltung-demo)

Die Anwendung digitalisiert die gemeinsame Strichliste eines Vereins. Grundlage
war das Web-Engineering-Teamprojekt „Deckel 2.0“. Bei der Weiterentwicklung kamen
Abläufe für den Thekenbetrieb und für die Übernahme vorhandener Listen hinzu.

## Nutzung im Alltag

Am Thekengerät wählt man ein Konto und ein Getränk. Der Thekenzugang dient zum
Erfassen von Getränken und zeigt keine Kontostände. Mitglieder sehen in ihrem
eigenen Verlauf Buchungen und Korrekturen. Eine Korrektur bleibt im Verlauf
nachvollziehbar.

## Import und Datenmodell

Importe älterer Strichlisten beginnen mit einer Vorschau. Die Zuordnung zu
Konten kann geprüft und korrigiert werden. Die Anwendung erkennt bereits
verarbeitete Listen und gruppiert Buchungen, damit sich ein Import geschlossen
übernehmen und bei Bedarf zurücknehmen lässt.

Ein fiktives Beispiel: Drei Getränke zu je 2,00 € ergeben eine Buchung von
6,00 €. Wird eine Position rückgängig gemacht, steht im Verlauf die ursprüngliche
Buchung mit einer Korrektur um 2,00 €. Der verbleibende Betrag ist 4,00 €.

TypeScript, Lit, Node.js und PostgreSQL bilden den technischen Rahmen.
