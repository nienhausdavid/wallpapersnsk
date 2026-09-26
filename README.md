# Wallpapers NSK

Hintergrundbilder für die von Intune verwalteten Android-Tablets von NSK (Niessing), betreut von Nienhaus IT. Der Microsoft Launcher lädt das Bild anonym über eine
öffentliche URL, deshalb ist dieses Repo **öffentlich** und getrennt vom privaten Repo `intune-baseline`.

**Nur Bilder ablegen, die jeder sehen darf** (Logos, Hintergründe). Keine internen Informationen, keine Zugangsdaten.

## Verwendung

1. Bild hochladen, Dateiname nach dem Muster `<rolle>-<variante>-<seitenverhaeltnis>-<version>.jpg`, z. B. `astm-plain-16x10-v1.jpg`.
   Empfehlung: JPG oder PNG, Seitenverhältnis und Auflösung des Tablets (z. B. 2560x1600), möglichst unter 1 MB.
2. URL des Bildes:
   ```
   https://raw.githubusercontent.com/nienhausdavid/wallpapersnsk/main/<dateiname>
   ```
3. In Intune in der Microsoft-Launcher-App-Konfiguration (`NSK - Android - ASTM - App-Konfiguration - Microsoft Launcher`) den Schlüssel `com.microsoft.launcher.Wallpaper.Url` eintragen.

**Bild austauschen:** neue Datei mit höherer Version anlegen (`tablet-v2.jpg`) und die URL in Intune anpassen. Eine gleichnamige Datei zu
ersetzen kann dazu führen, dass Geräte das alte, zwischengespeicherte Bild behalten. Alte Versionen erst löschen, wenn keine
Richtlinie mehr darauf zeigt.

## Enthaltene Bilder

18 Bilder in 2560 Pixel Breite (aus den 8000 Pixel breiten Originalen verkleinert, JPEG, 140 bis 250 KB), Version `v1`.

| Rolle | Bedeutung |
|---|---|
| `stm` | Store Manager |
| `astm` | Assistant Store Manager (stellvertretender Store Manager) |
| `store` | allgemeines Store-Bild |

| Variante | Bedeutung |
|---|---|
| `plain` | ohne Beschriftung |
| `beschriftet` | mit Beschriftung der Rolle unten rechts |

| Seitenverhältnis | Auflösung | Geräte |
|---|---|---|
| `16x10` | 2560 x 1600 | 11-Zoll-Tablets (z. B. Galaxy Tab A9+ und S9 FE) |
| `16x9` | 2560 x 1440 | Full-HD-Bildschirme |
| `3x2` | 2560 x 1707 | 3:2-Bildschirme |

Aktuell im Einsatz auf den Tablets: `astm-plain-16x10-v1.jpg`.

URL-Muster: `https://raw.githubusercontent.com/nienhausdavid/wallpapersnsk/main/<dateiname>`.

