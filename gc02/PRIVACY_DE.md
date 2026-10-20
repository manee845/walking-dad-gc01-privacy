# Datenschutzerklärung – The Walking Dad – GC02 Beta

Private Garmin Beta · 20. Oktober 2026

[English](PRIVACY.md)

Diese Erklärung gilt für die private GC02-Beta zur Prüfung von Aufzeichnung und zusätzlichen Garmin-Connect-Kennzahlen.

## 1. Verantwortlicher und Kontakt

Manuel von Allmen, Schweiz, ist für die hier beschriebene App und die Bearbeitung eigener Supportanfragen verantwortlich. Kontakt: [support.thewalkingdad@gmail.com](mailto:support.thewalkingdad@gmail.com).

Daten, die du dieser App oder ihrem Entwicklersupport bereitstellst, stellst du Manuel von Allmen und nicht Garmin bereit. Garmin übernimmt für diese appbezogene Verarbeitung keine Verantwortung oder Haftung; Garmins eigene Dienste und Verarbeitung sind davon getrennt.

## 2. Geltungsbereich und Zweck

Diese Erklärung betrifft The Walking Dad – GC02 Beta, die private Garmin-Connect-IQ-Erprobung für Fenix 6 Pro auf dem Fachstand GC02-B1/Schema 3. Die App zeichnet Spaziergänge auf und unterscheidet die manuell gewählten Modi 0 = Kinderwagen, 1 = Babytrage und 2 = Ohne Baby. Sie erfasst keine Namen, Babygewichte oder eigenen Kinderprofile. Der Modus „Kind läuft selbst“ ist nicht implementiert.

## 3. Verarbeitung auf der Garmin-Uhr

Die App verarbeitet Zeitstempel, aktive Dauer und Distanz sowie Begleitungsmodus, Segmentreihenfolge und Segmentgrenzen. Sie zeigt verfügbare native Garmin-Aktivitätswerte an, darunter Puls, Durchschnitts-/Maximalpuls, Geschwindigkeit beziehungsweise Pace, Aufstieg und Kalorien. Die App führt keine eigene Schrittzählung durch. Nicht jeder Wert ist auf jedem Gerät oder bei jeder Aktivität verfügbar.

## 4. Standort-, Aktivitäts- und Sensordaten

Ausserhalb der Recovery-Ansicht aktiviert die App beim Öffnen kontinuierliche Standortereignisse, also bereits vor dem manuellen Aktivitätsstart. Die native Walking-Aufzeichnung beginnt nach manuellem Start; ein GPS-Fix ist empfohlen, aber keine Startvoraussetzung. Bei fehlendem oder schlechtem Empfang können Strecken- und Distanzdaten unvollständig sein. Standortereignisse können in Pause und Abschlussübersicht weiterlaufen und werden beim erfolgreichen Abschluss beziehungsweise Appende deaktiviert. Garmin übernimmt die native Strecken-/Sensoraufzeichnung; diese kann zusätzliche Geräte-, Profil- und Fitnessmetadaten enthalten, die unsere App nicht selbst abfragt.

## 5. Eigene FIT-Developer-Felder

Die App ergänzt die native FIT-Aktivität um technische Felder zur Segmenthistorie, Modusfolge, UTC-Zeitbasis, aktiven Dauer, Distanz und Datenqualität sowie Modussummen. Hinzu kommen sechs für die Zusammenfassung konfigurierte Kennzahlen: aktive Dauer und Distanz für Kinderwagen, Babytrage und Ohne Baby. Insgesamt sind zwölf SESSION-Felder und vier RECORD-Felder definiert, davon zehn technische Beiträge ohne vorgesehene Nutzeranzeige. Die technischen Daten bleiben dennoch Bestandteil der FIT-Datei. Eine erfolgreiche Anzeige der sechs Kennzahlen in Garmin Connect ist für diese Beta noch nicht bestätigt.

## 6. Lokale Speicherung und Recovery

Im App-Speicher liegen zwei abwechselnd geschriebene, zurückgelesene und integritätsgeprüfte Checkpoints. Sie enthalten unter anderem eine lokale Aktivitätskennung, Revision, Zeitstempel, Zustands-/Speicherstatus, Segmenthistorie, Zähler und Modussummen. Sie enthalten keine vollständige GPS-Rohroute und keine Pulshistorie. Zusätzlich werden der zuletzt gewählte Modus und technische Aktivitätszähler gespeichert. Die SHA-256-Integritätsprüfung ist keine Verschlüsselung. Recovery zeigt einen lokalen Teilstand; sie setzt die ursprüngliche native Aufzeichnung nicht fort und exportiert daraus keine FIT-Datei.

## 7. Garmin Connect und Weitergabe

Bei Verwendung der Garmin-Synchronisierung können gespeicherte FIT-Aktivitäten einschliesslich GPS-Strecke, nativer Sensor-/Metadaten und unserer Developer-Felder an Garmin Connect gelangen. Garmin-Konto-, Synchronisations-, Freigabe- und weitere Garmin-Funktionen unterliegen Garmins eigenständiger Verarbeitung und Einstellungen. Ein lokaler Speichervorgang bestätigt keine Synchronisierung. Hinweise dazu: [Garmin Connect Datenschutz](https://www.garmin.com/privacy/connect/). Unsere lokale Checkpoint-Löschung löscht keine Garmin-Connect-Aktivität.

Zusammen mit einer GPS-Strecke können Zeitpunkt und Modus der Begleitungssegmente familiäre Routinen erkennen lassen.

## 8. Eigene Server, Konten und Diagnose

Die geprüfte App enthält keine eigene HTTP-Übertragung, keinen eigenen Cloudserver, keine Werbe-/Tracking- oder externen Analysedienste und verlangt kein separates The-Walking-Dad-Konto. Sie versendet Aktivitäten nicht selbst an den Entwickler. Die Berechtigungen sind Fit (native Aufzeichnung), FitContributor (zusätzliche FIT-Felder) und Positioning (Standortereignisse). Appseitige Diagnose verwendet feste, datenarme Status-/Fehlermeldungen ohne Segment- oder Standortdumps. Historische Logs und von Garmin erzeugte Systemprotokolle werden dadurch nicht rückwirkend gelöscht.

## 9. Speicherdauer und Löschmöglichkeiten

Es gibt keine feste zeitliche Ablaufregel für lokale Checkpoints. Nach eindeutig bestätigtem nativem Speichern und einem verifizierten Abschlussnachweis versucht die App, beide Checkpoints mit Rücklesekontrolle zu löschen. Bei Unsicherheit, Unterbrechungen oder Löschfehlern können Daten ganz oder teilweise verbleiben. Ein ausdrücklich bestätigtes Verwerfen veranlasst die Löschung der zugehörigen lokalen Checkpoints und prüft deren Abwesenheit durch Rücklesen. Eine vorhandene native Aufzeichnung muss zuvor erfolgreich verworfen werden. Verwerfen in Recovery betrifft nur die lokalen Checkpoints. Bei Fehlern können Daten ganz oder teilweise verbleiben; vollständige Löschung wird erst nach Verifikation gemeldet. „Später/Schliessen“ in Recovery erhält vorhandene Daten. Modusvorwahl und Zähler bleiben bei Checkpoint-Löschung bestehen. Gespeicherte FIT-Aktivitäten und synchronisierte Daten verwaltest du über Garmin. Für Deinstallation, Backups, Systemlogs oder physische Flashreste wird keine vollständige Löschung zugesichert.

## 10. Support per E-Mail

Bei Kontaktaufnahme bearbeitet Manuel von Allmen Absenderangaben, Nachricht und freiwillige Anhänge zur Beantwortung der Anfrage über Gmail (Google). Nur Manuel hat Zugang zum Supportpostfach. Bitte sende keine unnötigen Standort-, Gesundheits-, Kinder- oder FIT-Daten. Nachrichten bleiben so lange wie erforderlich gespeichert; das Postfach wird mindestens alle sechs Monate geprüft und nicht mehr benötigte Nachrichten werden gelöscht, sofern kein berechtigter Aufbewahrungsgrund besteht. Google nennt für Schweizer Verbraucherkonten grundsätzlich Google Ireland Limited (Irland); eine Verarbeitung insbesondere in den USA und weiteren Ländern ist möglich. Siehe [Google-Datenschutz](https://policies.google.com/privacy?hl=de) und [Übermittlungsrahmen](https://policies.google.com/privacy/frameworks?hl=de). Google beschreibt für internationale Übermittlungen unter anderem Angemessenheitsmechanismen, das Swiss–US Data Privacy Framework und Standardvertragsklauseln; deren Anwendung richtet sich nach der jeweiligen Übermittlung.

## 11. Hosting dieser Erklärung

Diese Erklärung wird als Dateien im öffentlichen GitHub-Repository manee845/walking-dad-gc01-privacy bereitgestellt. Beim Abruf seiner Webseite verarbeitet GitHub Verbindungs- und Nutzungsdaten, darunter IP-Adressen. Anbieter sind GitHub B.V. (Niederlande) beziehungsweise GitHub, Inc. (USA); eine Verarbeitung in den USA und weiteren Ländern ist möglich. Wir ergänzen die Erklärungsdateien nicht um Analyse-Skripte, externe Schriftarten oder Medien. GitHubs Webseitenfunktionen, Cookies, Aufbewahrung und eigenständige Verarbeitung beschreibt die [GitHub-Datenschutzerklärung](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). GitHub beschreibt für internationale Übermittlungen Standardvertragsklauseln und seine Teilnahme am Swiss–US Data Privacy Framework; der anwendbare Mechanismus richtet sich nach der jeweiligen Übermittlung.

## 12. Rechte und Kontaktweg

Für Auskunft über durch uns bearbeitete Personendaten sowie gesetzlich vorgesehene Berichtigung, Löschung, Herausgabe/Übertragung oder Einwendungen kannst du dich an [support.thewalkingdad@gmail.com](mailto:support.thewalkingdad@gmail.com) wenden. Soweit eine Verarbeitung auf Einwilligung beruht, kannst du sie für die Zukunft widerrufen. Wir prüfen Anfragen nach anwendbarem Recht und können zur Vermeidung unbefugter Auskunft eine geeignete Identifikation verlangen. Der Entwickler hat durch die App keinen Zugriff auf dein gesamtes Garmin-Konto. Anfragen zu Garmins eigenständiger Verarbeitung richtest du an Garmin. Du kannst dich auch an die zuständige Datenschutzaufsicht wenden, in der Schweiz den [EDÖB](https://www.edoeb.admin.ch/de).

## 13. Änderungen und Stand

Diese Erklärung wird bei wesentlichen Änderungen der beschriebenen Verarbeitung angepasst. Stand: 20. Oktober 2026. Die jeweils aktuelle deutsche und englische Fassung findest du in diesem Verzeichnis.
