# CarSweep

Impressum, Datenschutzerklärung und Support-Kontakt zur App CarSweep (iOS und Android).

https://carsweep.app/

Die Domain liegt bei Cloudflare (Registrar und DNS): CNAME `@` und `www` →
`carsweep-app.github.io`, beide „DNS only“ – mit Proxy stellt GitHub kein Zertifikat aus.
Die alte Adresse https://carsweep-app.github.io/CarSweep-App/ leitet hierher weiter.

## Indexierung

`index.html` setzt `noindex, nofollow`, zusätzlich schließt `robots.txt` alle Crawler inkl.
gängiger KI-Bots aus. Beides gilt nur für die GitHub-Pages-Domain, nicht für die Dateiansicht
im Repository selbst.

## Anleitungen (`guides/`)

Englische Schritt-für-Schritt-Anleitungen mit Screenshots, verlinkt von der Startseite:
`/guides/` (Übersicht), `/guides/expert-mode/`, `/guides/eq-designer/`. Gemeinsames Aussehen in
`guides/guide.css` (nur Systemschriften, keine Anfragen an Dritte), Bilder in `guides/img/`.

**Markierungen:** Jede Zahl auf einem Screenshot ist ein `<span class="pin" style="--x:…;--y:…">`
– Position in Prozent der Bildbreite bzw. -höhe, der Mittelpunkt des Kreises. Die Liste daneben
nennt dieselbe Nummer. Wer ein Bild austauscht, muss die Prozentwerte neu setzen.

**Screenshots neu machen:** Simulator iPhone 17 Pro (Referenzgerät der App), Debug-Build mit
Pro freigeschaltet, `xcrun simctl status_bar … override --time 9:41`, App gestartet mit
`-AppleLanguages "(en)" -ScreenshotInput "UMIK-1" -ScreenshotOutput "Tesla Model 3"` (sonst
steht in der Herkunftszeile „Simulator"). EQ-Designer-Schirme über `-DraftScreen hub|setup|prep|
boost|review|uncertain|result`. Aufnahme mit `xcrun simctl io … screenshot`, dann auf den
gezeigten Ausschnitt zuschneiden und auf 630 px Breite verkleinern (JPEG, Qualität ~84).
Im Experten-Bild „System info" und in den Einstellungen sind „Speaker"/„iPhone mic" durch
„Tesla Model 3"/„UMIK-1" ersetzt – der Simulator meldet nur seine eigenen Geräte.

Wie die übrige Seite stehen die Anleitungen auf `noindex`.
