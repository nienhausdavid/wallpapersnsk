# Wallpapers NSK

Hintergrundbilder fuer die von Intune verwalteten Android-Tablets von NSK (Niessing), betreut von Nienhaus IT. Der Microsoft Launcher laedt das Bild anonym ueber eine
oeffentliche URL, deshalb ist dieses Repo **oeffentlich** und getrennt vom privaten Repo `intune-baseline`.

**Nur Bilder ablegen, die jeder sehen darf** (Logos, Hintergruende). Keine internen Informationen, keine Zugangsdaten.

## Verwendung

1. Bild hochladen, Dateiname nach dem Muster `<rolle>-<variante>-<seitenverhaeltnis>-<version>.jpg`, z. B. `astm-plain-16x10-v1.jpg`.
   Empfehlung: JPG oder PNG, Seitenverhaeltnis und Aufloesung des Tablets (z. B. 2560x1600), moeglichst unter 1 MB.
2. URL des Bildes:
   ```
   https://raw.githubusercontent.com/nienhausdavid/wallpapersnsk/main/<dateiname>
   ```
3. In Intune in der Richtlinie `NSK - Android - ASTM - Hintergrundbild Microsoft Launcher` bei **Custom wallpaper image URL** eintragen.

**Bild austauschen:** neue Datei mit hoeherer Version anlegen (`tablet-v2.jpg`) und die URL in Intune anpassen. Eine gleichnamige Datei zu
ersetzen kann dazu fuehren, dass Geraete das alte, zwischengespeicherte Bild behalten. Alte Versionen erst loeschen, wenn keine
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

| Seitenverhaeltnis | Aufloesung | Geraete |
|---|---|---|
| `16x10` | 2560 x 1600 | 11-Zoll-Tablets (z. B. Galaxy Tab A9+ und S9 FE) |
| `16x9` | 2560 x 1440 | Full-HD-Bildschirme |
| `3x2` | 2560 x 1707 | 3:2-Bildschirme |

Aktuell im Einsatz auf den Tablets: `astm-plain-16x10-v1.jpg`.

URL-Muster: `https://raw.githubusercontent.com/nienhausdavid/wallpapersnsk/main/<dateiname>`.

