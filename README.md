# Impressum & Datenschutzerklärung – CFOP/Fridrich-Algorithmen-Trainer

**Deutsch (maßgeblich)** · [Français](README.fr.md) · [Italiano](README.it.md) · [Español](README.es.md)

## Impressum

Angaben gemäß § 5 DDG (vormals § 5 TMG):

Roland Albrecht
Im Jägeracker 42
79312 Emmendingen
Deutschland

Kontakt: rca@quantentunnel.de

## Datenschutzerklärung

Stand: 18.10.2026

### 1. Verantwortlicher

Roland Albrecht
E-Mail: rca@quantentunnel.de

Verantwortlich im Sinne der Datenschutz-Grundverordnung (DSGVO) für die im Folgenden beschriebene Datenverarbeitung ist die oben genannte Person als Entwickler der App "CFOP/Fridrich-Algorithmen-Trainer" (im Folgenden "die App").

### 2. Kurzübersicht

Die App erhebt, speichert und überträgt **keine personenbezogenen Daten an den Entwickler oder an Dritte**. Es gibt:

- kein Nutzerkonto und keine Anmeldung,
- keine Internetverbindung (die App fordert keine entsprechende Berechtigung an und kommuniziert mit keinem Server),
- keine Analyse-, Tracking- oder Werbedienste (kein Google Analytics, keine Crash-Reporting- oder Ad-SDKs),
- keine Weitergabe von Daten an Dritte, da schlicht keine Daten das Gerät verlassen.

Alle innerhalb der App entstehenden Daten verbleiben ausschließlich lokal auf dem Gerät der Nutzerin bzw. des Nutzers. Das gilt auch für die optionale Bluetooth-Verbindung zu einem Smart-Cube: Sie besteht nur direkt zwischen Gerät und Würfel, ohne Standortzugriff (Abschnitt 5).

### 3. Welche Daten werden lokal auf dem Gerät gespeichert?

Damit die App ihre Trainingsfunktionen (Algorithmen-Training, Lernpfad, Spaced-Repetition-Wiederholung) erfüllen kann, speichert sie folgende Daten **ausschließlich lokal in einer Datenbank auf dem jeweiligen Gerät**:

- Trainings- und Übungsstatistiken je Algorithmus-Fall (z. B. Anzahl Versuche, Erfolgsquote),
- Zeitplan-/Fälligkeitsdaten der Spaced-Repetition-Wiederholung (Datum der nächsten fälligen Wiederholung je Fall),
- Fortschritt im geführten Lernpfad (welche Stufen/Fälle bereits freigeschaltet bzw. gefestigt sind),
- von der Nutzerin/dem Nutzer selbst gespeicherte eigene Zugfolgen-Varianten zu einzelnen Algorithmus-Fällen,
- gewählte App-Spracheinstellung (Deutsch, Englisch, Französisch, Italienisch oder Spanisch) sowie sonstige App-Einstellungen (z. B. Sticker-Look-Voreinstellung, Anzeige der Tagesserie).
- bei Nutzung eines Smart-Cubes (Abschnitt 5): Name und Bluetooth-Adresse des zuletzt verbundenen Würfels samt den zugehörigen Einstellungen (automatisch verbinden, Lage des Würfels verwenden) sowie je Übungsversuch, ob er per Touch oder mit dem Smart-Cube ausgeführt wurde.

Diese Daten werden technisch mittels einer lokalen Room-Datenbank (SQLite) sowie lokaler Einstellungsspeicherung (SharedPreferences) auf dem Gerät abgelegt. Es handelt sich dabei nicht um eine Übermittlung an den Entwickler – niemand außer der Person, die das Gerät nutzt, hat Zugriff auf diese Daten.

### 4. Backup-Funktion (lokale Sicherungsdatei)

Die App bietet im Einstellungsmenü optional die Möglichkeit, eine lokale Sicherungsdatei (Backup) der Erfolgsstatistik, des Übungsverlaufs samt Zeitplan/Fälligkeiten der Spaced-Repetition-Wiederholung, des Lernpfad-Fortschritts, der favorisierten Algorithmen-Varianten und der selbst gespeicherten Algorithmen zu erstellen sowie eine zuvor erstellte Sicherungsdatei wieder zu laden. Die Datei wird ausschließlich über den vom Betriebssystem bereitgestellten Dateiauswahl-Dialog an einem von der Nutzerin/dem Nutzer selbst gewählten Speicherort abgelegt bzw. von dort gelesen – die App wählt keinen Speicherort automatisch und überträgt die Datei zu keinem Zeitpunkt an den Entwickler oder an Dritte. Wählt die Nutzerin/der Nutzer als Speicherort einen cloud-synchronisierten Ordner (z. B. eine Drive- oder OneDrive-Integration des Geräts), unterliegt die weitere Verarbeitung dieser Datei den Datenschutzbestimmungen des jeweiligen Cloud-Anbieters, nicht denen dieser App.

### 5. Bluetooth-Verbindung zu einem Smart-Cube (optional)

Ab Android 12 kann die App optional mit einem Bluetooth-fähigen Zauberwürfel ("Smart-Cube", derzeit GAN i4 und GoCube) verbunden werden, der die Drehungen am Würfel an die App meldet. Die Funktion ist freiwillig; ohne sie bleibt die App vollständig per Touch bedienbar.

- **Verbindung nur lokal:** Die App sucht über Bluetooth Low Energy nach Smart-Cubes in der Nähe und verbindet sich direkt mit dem ausgewählten Würfel. Es ist kein Server, kein Hersteller-Konto und keine Internetverbindung beteiligt.
- **Verarbeitete Daten:** Vom Würfel empfängt die App ausschließlich Zug-Ereignisse (welche Seite in welche Richtung gedreht wurde, mit Zeitstempel), Lage-Ereignisse (Ausrichtung des Würfels im Raum), den Akkustand sowie Gerätename, Modell und Hardware-Informationen. Diese Daten werden nur für die laufende Übung verwendet; gespeichert werden daraus nur die üblichen Trainingsdaten aus Abschnitt 3 (Zugfolge, Zeit und Bewertung eines Versuchs, ergänzt um die Eingabequelle).
- **Gespeicherter Würfel:** Damit sich die App beim nächsten Start wieder mit demselben Würfel verbinden kann, speichert sie dessen Namen und Bluetooth-Adresse lokal auf dem Gerät. Über "Entfernen" im Smart-Cube-Menü lässt sich dieser Eintrag jederzeit löschen. Diese Angaben sind nicht Teil der Backup-Datei (Abschnitt 4).
- **Kein Standortzugriff:** Die App verwendet dafür nur die Berechtigung "Geräte in der Nähe" (Abschnitt 8) und erklärt gegenüber dem System ausdrücklich, aus der Bluetooth-Suche keinen Standort abzuleiten. Andere gefundene Bluetooth-Geräte werden weder angezeigt noch gespeichert.
- **Keine Übertragung:** Weder die Würfel-Daten noch die gespeicherte Bluetooth-Adresse verlassen das Gerät.

### 6. Keine Datenübertragung, kein Server, kein Konto

Die App benötigt und besitzt keine Internetzugriffsberechtigung. Es findet daher zu keinem Zeitpunkt eine Übertragung von Daten an den Entwickler, an Google oder an sonstige Dritte über die App selbst statt. Es gibt kein Nutzerkonto, keine Registrierung und keine Cloud-Synchronisation.

### 7. Keine Analyse-, Tracking- oder Werbedienste

Die App enthält keinerlei Analyse-Software (z. B. Firebase Analytics), keine Absturzberichts-Dienste (z. B. Crashlytics) und keine Werbe-SDKs. Es werden keine Nutzungsprofile erstellt, kein Standort ermittelt und keine Werbe-ID ausgelesen.

### 8. App-Berechtigungen

Die App fordert keine besonderen Gerätezugriffs-Berechtigungen (z. B. keinen Zugriff auf Kamera, Standort, Kontakte, Mikrofon oder Internet) an – mit einer Ausnahme: Für die optionale Smart-Cube-Verbindung (Abschnitt 5) verwendet sie ab Android 12 die Berechtigung "Geräte in der Nähe" (`BLUETOOTH_SCAN` mit dem Hinweis, dass kein Standort abgeleitet wird, und `BLUETOOTH_CONNECT`). Sie wird erst angefragt, wenn die Nutzerin/der Nutzer im Smart-Cube-Menü nach einem Würfel sucht oder sich verbindet, und kann jederzeit in den Android-Einstellungen widerrufen werden; die übrige App funktioniert auch ohne sie. Die Backup-Funktion (Abschnitt 4) verwendet den systemeigenen Dateiauswahl-Dialog (Storage Access Framework), der keine zusätzliche Berechtigung erfordert.

### 9. Speicherdauer und Löschung

Die in Abschnitt 3 genannten Daten verbleiben so lange lokal auf dem Gerät gespeichert, bis sie:

- über die in der App integrierten Funktionen zurückgesetzt werden (z. B. "Statistik zurücksetzen" oder "Eigene Algorithmen löschen" im Einstellungsmenü), oder
- durch Deinstallation der App vollständig vom Gerät entfernt werden.

Der gespeicherte Smart-Cube (Abschnitt 5) lässt sich zusätzlich jederzeit über "Entfernen" im Smart-Cube-Menü löschen.

Da keine Daten außerhalb des Geräts gespeichert werden, ist mit der Deinstallation der App keine weitere Kopie der Daten mehr vorhanden – mit Ausnahme einer von der Nutzerin/dem Nutzer selbst erstellten Backup-Datei (Abschnitt 4), die unabhängig von der App an ihrem gewählten Speicherort bestehen bleibt und bei Bedarf selbst gelöscht werden kann.

### 10. Rechte der betroffenen Person

Da die App keine personenbezogenen Daten an den Entwickler überträgt, liegen sämtliche in Abschnitt 3 genannten Daten ausschließlich im unmittelbaren Zugriff und unter der vollständigen Kontrolle der Nutzerin bzw. des Nutzers selbst (Auskunft, Berichtigung und Löschung erfolgen direkt über die App bzw. durch Deinstallation). Für Fragen zum Datenschutz in Bezug auf die App kann dennoch jederzeit der in Abschnitt 1 genannte Kontakt genutzt werden.

### 11. Minderjährige

Die App richtet sich nicht gezielt an Kinder und erhebt unabhängig vom Alter der Nutzerin bzw. des Nutzers keinerlei personenbezogene Daten.

### 12. Änderungen dieser Datenschutzerklärung

Diese Datenschutzerklärung kann bei Bedarf angepasst werden, etwa wenn neue App-Funktionen eine Aktualisierung erforderlich machen. Die jeweils aktuelle Fassung ist unter der im Play-Store-Eintrag verlinkten Adresse abrufbar.

### 13. Kontakt

Bei Fragen zu dieser Datenschutzerklärung oder zur App wenden Sie sich bitte an:

rca@quantentunnel.de
