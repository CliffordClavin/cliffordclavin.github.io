# Einladungsseite (GitHub Pages)

Diese Dateien gehören in das Repository `<dein-name>.github.io` (GitHub Pages, Branch `main`, Ordner `/`).

- `join/index.html` – Ziel der Einladungslinks `https://<dein-name>.github.io/join/?c=CODE`.
  Ist die App installiert, öffnet Android den Link direkt in der App (App Links).
- `.well-known/assetlinks.json` – Bestätigt Android, dass die App diese Links öffnen darf.
  Enthält den SHA-256-Fingerabdruck des **Debug**-Schlüssels. Für eine Release- oder
  Play-Store-Version den Fingerabdruck des Release- bzw. Play-App-Signing-Schlüssels ergänzen.
- `.nojekyll` – Sorgt dafür, dass GitHub Pages den Ordner `.well-known` ausliefert.

In der App muss `local.properties` den Host enthalten: `INVITE_HOST=<dein-name>.github.io`.
