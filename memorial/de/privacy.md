# Datenschutzerklärung von Virtual Memorial Space

**Gültig ab: 1. November 2026**

## 1. Einleitung

Virtual Memorial Space („die App“, „wir“, „uns“) ist eine iOS-App, mit der du private Gedenkräume anlegen, Gedenkrituale durchführen und Briefe schreiben kannst. Diese Datenschutzerklärung erklärt, welche Informationen die App verarbeitet, wo sie gespeichert werden und welche Wahlmöglichkeiten du hast.

Die App benötigt kein Konto. Deine Gedenkinhalte bleiben auf deinem Gerät. Unser Server wird ausschließlich für Gedenk-Token verwendet, optionale In-App-Token für besondere Varianten von Gaben.

Durch die Nutzung der App bestätigst du, dass du diese Datenschutzerklärung gelesen und verstanden hast.

## 2. Informationen, die wir nicht erheben

Die App erhebt oder verlangt nicht:

- Deinen Namen, deine E-Mail-Adresse, Telefonnummer oder ein Anmeldekonto
- Die Namen, Fotos, Daten, Beschreibungen, Briefe oder Nachrichten in deinen Gedenkräumen
- Zugriff auf deine gesamte Fotomediathek, Kamera, Mikrofon, Kontakte oder Standort
- Deine Zahlungskartendaten
- Eine Werbe-ID (IDFA). Die App verfolgt dich nicht über Apps oder Websites anderer Unternehmen hinweg und zeigt die Abfrage zur App-Tracking-Transparenz nicht an.
- Analyse- oder Nutzungsereignisse. Die App enthält kein Analyse-SDK und keine Werbung.

## 3. Gedenkinhalte, die nur auf deinem Gerät gespeichert werden

Folgendes wird im privaten Speicher der App auf deinem iPhone oder iPad gesichert:

- Gedenkräume: Name, Art (zum Beispiel geliebter Mensch, Partner, Freund oder Haustier), Beschreibung, Geburtsdatum, Gedenktag, Design und Erinnerungseinstellung
- Fotos, die du einem Gedenkraum hinzufügst
- Ritualeinträge: welche Kerze, Blume oder Papiergabe verwendet wurde, die Anzahl verbrauchter Token, der Zeitpunkt und eine eventuell hinzugefügte Nachricht
- Briefe, die du schreibst, einschließlich Entwürfen
- Einstellungen: Sprache, reduzierte Effekte, ob traditionelle Papiergaben angezeigt werden, ob die Einführung abgeschlossen ist, eine Markierung für ausstehende Kaufsynchronisierung und ein Zähler, der Bewertungsanfragen begrenzt
- Der zuletzt von unserem Server erhaltene Token-Kontostand, nur zur Anzeige ohne Internetverbindung

Diese Inhalte werden nicht auf unseren Server hochgeladen, nicht für Werbung verwendet und nicht für Funktionen oder das Training künstlicher Intelligenz (KI) genutzt. Ist iCloud-Backup aktiviert, kann iOS diese Daten in die Gerätesicherung aufnehmen, die Apple im Rahmen deiner Apple-ID verarbeitet. Die App hat keine eigene Cloud-Synchronisierung.

**Fotos.** Du wählst Fotos über die Fotoauswahl des Systems aus. Die App erhält nur die ausgewählten Fotos und greift nicht auf deine gesamte Fotomediathek zu. Von jedem ausgewählten Foto wird eine komprimierte Kopie im Speicher der App abgelegt.

## 4. Gedenk-Token und unser Server

Gedenk-Token sind Verbrauchsartikel, die per In-App-Kauf erworben werden. Damit dein Kontostand eine Neuinstallation der App übersteht, wird er auf unserem Server („appapi“) gespeichert. Dieser läuft bei Vercel und speichert Daten in Vercel KV (Upstash Redis).

Der Server speichert ausschließlich:

- Eine zufällig erzeugte Benutzer-ID, die nicht mit deinem Namen, deiner E-Mail-Adresse oder deiner Apple-ID verknüpft ist
- Einen Hashwert des für diese Benutzer-ID ausgestellten Zugriffstokens. Das Token selbst wird nicht auf dem Server gespeichert.
- Deinen Token-Kontostand
- Kaufdatensätze: Produkt-ID, Apple-Transaktions-ID, Anzahl der Token und Zeitpunkt
- Verbrauchsdatensätze: Gaben-ID (zum Beispiel eine Kerzenart), Anzahl der Token, der Anfrageschlüssel gegen doppelte Abbuchung, Kontostand danach und Zeitpunkt
- Ein Buchungsprotokoll über Gutschriften, Abbuchungen und Erstattungen mit Beträgen und zugehörigen Transaktions- oder Verbrauchs-IDs

Jede Anfrage an den Server enthält außerdem die App-Version und eine Gerätekennung (die iOS-identifierForVendor), die zur Prüfung der Anfragesignatur dienen. Wie bei jedem Webdienst kann unser Hosting-Anbieter deine IP-Adresse in üblichen Anfrageprotokollen verarbeiten, um den Dienst bereitzustellen und zu schützen.

Der Server speichert weder deinen Namen noch deine E-Mail-Adresse und nichts über die Menschen oder Haustiere, an die du erinnerst: keine Namen, Fotos, Briefe oder Nachrichten aus Gedenkräumen.

Benutzer-ID und Token werden im iOS-Schlüsselbund auf deinem Gerät gespeichert. Sie können über den iCloud-Schlüsselbund synchronisiert werden, sodass dein Kontostand nach einer Neuinstallation oder auf einem anderen Gerät mit derselben Apple-ID verfügbar ist.

## 5. Käufe

- **Apple (App Store)** wickelt alle Zahlungen über deine Apple-ID ab. Wir erhalten niemals deine Zahlungskartendaten. Datenschutzrichtlinie von Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** prüft Transaktionen. RevenueCat erhält die oben genannte zufällige Benutzer-ID, Transaktionsinformationen (etwa Produkt-ID, Apple-Transaktions-ID und Kaufzeitpunkt) sowie grundlegende technische Informationen wie App-Version, Betriebssystemversion und App-Store-Land. Unser Server lässt sich Käufe von RevenueCat bestätigen, und RevenueCat informiert unseren Server über Käufe und Erstattungen, damit Token nur einmal gutgeschrieben und nach einer Erstattung wieder abgezogen werden. Datenschutzrichtlinie von RevenueCat: https://www.revenuecat.com/privacy

Gedenk-Token haben keinen realen Geldwert. Erstattungen werden von Apple nach den eigenen Regeln bearbeitet. Die Nutzungsbedingungen sind Apples Standard-Lizenzvereinbarung: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Mitteilungen (optional)

Wenn du für einen Gedenkraum eine Erinnerung an den Gedenktag aktivierst, fragt die App nach der Berechtigung für Mitteilungen und plant lokale Mitteilungen auf deinem Gerät. Erinnerungen laufen nicht über unseren Server. Du kannst sie in der App oder in den iOS-Einstellungen deaktivieren.

## 7. Wie wir Informationen verwenden

Wir verwenden die oben genannten Informationen nur, um:

- Deine Gedenkräume, Rituale und Briefe auf deinem Gerät anzuzeigen und zu speichern
- Deine Token-Wallet anzulegen, gekaufte Token einmal pro Transaktion gutzuschreiben, Token abzubuchen, wenn du eine besondere Gabe wählst, und Token nach einer Erstattung zurückzubuchen
- Anfragen zu prüfen und Betrug oder doppelte Gutschriften zu verhindern
- Auf deine Support-Anfragen zu antworten

Wir verkaufen oder vermieten keine personenbezogenen Daten, nutzen sie nicht für Werbung und erstellen keine Werbeprofile.

## 8. Weitergabe

Wir geben Informationen nur an Dienstleister weiter, die für den Betrieb der App nötig sind (Apple, RevenueCat sowie Vercel / Upstash für Hosting und Speicherung), oder wenn Gesetze oder ein gültiges rechtliches Verfahren dies verlangen.

## 9. Löschen deiner Daten

In den Einstellungen der App:

- **Alle Daten löschen (Delete All Data)** löscht alle Gedenkinhalte auf diesem Gerät: Gedenkräume, Fotos, Ritualeinträge, Briefe und Nachrichten.
- **Token-Daten löschen (Delete Token Data)** löscht deine Wallet auf unserem Server: den Datensatz der Benutzer-ID, den Token-Hash, den Kontostand, Kauf- und Verbrauchsdatensätze sowie das Buchungsprotokoll. Dein Kontostand wird auf null gesetzt und kann nicht wiederhergestellt werden. Damit derselbe Kauf nicht erneut gutgeschrieben wird, behalten wir nur die Apple-Transaktions-ID (mit ihrer Produkt-ID) ohne Benutzer-ID. Anschließend werden Benutzer-ID und Token auch aus deinem Schlüsselbund entfernt.

Das Löschen der App entfernt ihre lokalen Inhalte vom Gerät, löscht aber **nicht** deine Wallet auf unserem Server. Nutze dafür vor dem Löschen der App „Token-Daten löschen“ oder kontaktiere uns. Gelöschte lokale Daten können in früheren iCloud-Gerätebackups verbleiben, bis Apple diese ersetzt oder löscht.

Du kannst uns außerdem bitten, bei RevenueCat die Löschung des dort gespeicherten Kaufdatensatzes zu beantragen.

## 10. Sicherheit und Speicherdauer

Verbindungen zu unserem Server, zu Apple und zu RevenueCat sind per HTTPS verschlüsselt. Anfragen werden signiert, der Server speichert nur einen Hash deines Tokens, und deine Kennung liegt im iOS-Schlüsselbund. Keine Speicher- oder Übertragungsmethode ist vollkommen sicher.

- Lokale Inhalte bleiben erhalten, bis du sie oder die App löschst.
- Wallet-Daten auf dem Server bleiben erhalten, bis du „Token-Daten löschen“ verwendest oder uns um Löschung bittest.
- Apple-Transaktions-IDs ohne Benutzer-ID werden aufbewahrt, um doppelte Gutschriften zu verhindern.
- Apple und RevenueCat bewahren Kaufdatensätze nach ihren eigenen Richtlinien und gesetzlichen Pflichten auf.

## 11. Datenschutz von Kindern

Virtual Memorial Space richtet sich nicht an Kinder. Wir erheben wissentlich keine personenbezogenen Daten von Kindern unter 13 Jahren (oder unter dem in deinem Land geltenden Mindestalter). Wenn du glaubst, dass ein Kind uns personenbezogene Daten übermittelt hat, kontaktiere uns, und wir löschen sie.

## 12. Verarbeitung im Ausland

Unsere Hosting- und Speicheranbieter sowie RevenueCat können Daten in den Vereinigten Staaten oder in anderen Ländern als deinem eigenen verarbeiten. Für diese Verarbeitung stützen wir uns auf die Schutzmaßnahmen dieser Anbieter.

## 13. Deine Rechte

Je nach Wohnort hast du möglicherweise das Recht auf Auskunft, Berichtigung, Löschung oder Einschränkung der Verarbeitung deiner personenbezogenen Daten. Die meisten Daten liegen auf deinem Gerät und unter deiner Kontrolle. Für Daten auf unserem Server verwende „Token-Daten löschen“ oder kontaktiere uns. Wir können um Angaben bitten, die uns helfen, die betreffenden Datensätze zu finden.

## 14. Änderungen dieser Erklärung

Wir können diese Datenschutzerklärung aktualisieren. Das Datum oben ändert sich dann entsprechend. Wenn die App beginnt, neue Arten von Daten zu erheben, aktualisieren wir diese Erklärung vorher.

## 15. Kontakt

Bei Fragen zu dieser Datenschutzerklärung kontaktiere uns:

- E-Mail: lpjustdoit@163.com

---

## Weitere Sprachen

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
