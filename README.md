# FlowScribe Releases

Offizielle Downloads und Updates für **FlowScribe**, die Diktier-App für Windows 10 und 11 von [Manuel Landeck / Firmenflow](https://www.firmenflow.de). Du sprichst, FlowScribe schreibt, in jeder App. Spracherkennung und KI laufen lokal auf deinem PC, ohne Konto und ohne Abo.

Dieses Repository enthält nur die fertigen Dateien (Setup, Portable, `latest.json` für die Auto-Updates). Der Quellcode liegt privat.

## Download

Die Downloads stehen unter [Releases](https://github.com/manuelos19-ops/flowscribe-releases/releases). FlowScribe ist zurzeit in der Beta.

| Variante | Datei | Für wen? |
| --- | --- | --- |
| **Setup** | `FlowScribe_<Version>_x64-setup.exe` | Installiert pro Benutzer ohne Admin-Rechte, Updates kommen automatisch |
| **Portable** | `FlowScribe_<Version>_x64-portable.zip` | Entpacken und starten, gut für USB-Sticks und PCs ohne Installationsrechte |

## Prüfen

Zu jeder Version stehen im Release-Text die SHA-256-Hashes und die VirusTotal-Berichte. Selbst prüfen in PowerShell:

```powershell
Get-FileHash ~/Downloads/FlowScribe_<Version>_x64-setup.exe -Algorithm SHA256
```

Exakt gleich heißt: unverändertes Original.

## Windows SmartScreen

FlowScribe ist noch nicht code-signiert. Beim ersten Start kann Windows „Der Computer wurde durch Windows geschützt“ anzeigen. Klicke auf **Weitere Informationen** und dann auf **Trotzdem ausführen**.

## Updates

Die installierte FlowScribe fragt höchstens einmal am Tag hier nach einer neuen Version und bietet sie mit „Jetzt installieren“, „Später“ oder „Überspringen“ an. Jedes Update ist signiert, FlowScribe installiert nur Pakete mit gültiger Signatur. Abschaltbar in den Einstellungen unter Allgemein → Updates.
