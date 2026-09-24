# Wallpapers

Hintergrundbilder fuer von Intune verwaltete Android-Tablets (Nienhaus IT). Der Microsoft Launcher laedt das Bild anonym ueber eine
oeffentliche URL, deshalb ist dieses Repo **oeffentlich** und getrennt vom privaten Repo `intune-baseline`.

**Nur Bilder ablegen, die jeder sehen darf** (Logos, Hintergruende). Keine internen Informationen, keine Zugangsdaten.

## Verwendung

1. Bild hochladen, Dateiname nach dem Muster `<kunde>-<zweck>-<version>.jpg`, z. B. `nsk-tablet-v1.jpg`.
   Empfehlung: JPG oder PNG, Seitenverhaeltnis und Aufloesung des Tablets (z. B. 2560x1600), moeglichst unter 1 MB.
2. URL des Bildes:
   ```
   https://raw.githubusercontent.com/nienhausdavid/wallpapers/main/<dateiname>
   ```
3. In Intune in der Geraeteeinschraenkung (Microsoft Launcher) bei **Custom wallpaper image URL** eintragen, bzw. in der Vorlage
   `Restriktion - Vollverwaltete Geraete Samsung Kiosk` aus `intune-baseline` den Platzhalter ersetzen.

**Bild austauschen:** neue Datei mit hoeherer Version anlegen (`...-v2.jpg`) und die URL in Intune anpassen. Eine gleichnamige Datei zu
ersetzen kann dazu fuehren, dass Geraete das alte, zwischengespeicherte Bild behalten. Alte Versionen erst loeschen, wenn keine
Richtlinie mehr darauf zeigt.
