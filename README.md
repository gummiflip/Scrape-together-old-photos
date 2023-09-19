# Scrape-together-old-photos


Die Zeitkapsel-Community 🕰️🖼️

Willkommen in der Zeitkapsel!

Unsere Community hat sich einem besonderen Projekt verschrieben: dem Erkunden, Sichern und Wiederentdecken alter Erinnerungen. Wir haben uns auf die Reise begeben, in den Tiefen vergessener Festplatten und unzähliger Ordner nach jenen verlorenen Augenblicken zu suchen, die im Laufe der Jahre beiseitegelegt wurden.

📂 Tausende von Ordnern, zig Festplatten – Unser Abenteuer besteht darin, uns durch diesen digitalen Dschungel zu navigieren, um jene vergessenen Momente wiederzuentdecken.

📸 Fotos aus vergangenen Zeiten – Werden Sie Zeuge von verschwundenen Erinnerungen, lachenden Gesichtern und Orten, die Sie vielleicht nie gesehen haben. Jedes Foto erzählt eine eigene Geschichte.

🗂️ Sortieren und Selektieren – Wir wählen nicht nur die besten Momente aus, sondern organisieren sie auch in einer Art, die Sinn macht. In der Tat, ein wahrer Schatz ist nur dann wertvoll, wenn man ihn auch finden kann!

Teilnehmen und Teilen!
Jeder ist eingeladen, seinen eigenen verstaubten Datenträger mitzubringen und sich uns auf dieser spannenden Reise anzuschließen. Wer weiß, welche Schätze Sie in Ihren alten Daten finden werden?

# Ubuntu Setup und Datenkopier-Guide

In diesem Repository finden Sie Skripte und Anweisungen, die Ihnen helfen, Ihr Ubuntu-System nach einer frischen Installation einzurichten und Daten von einem USB-Gerät zu kopieren.

## Inhaltsverzeichnis

- [Post-Installation von Ubuntu](#post-installation-von-ubuntu)
- [USB-Gerät finden](#usb-gerät-finden)
- [Datenkopie-Skript](#datenkopie-skript)

## Post-Installation von Ubuntu

Nachdem Sie Ubuntu installiert haben, sollten Sie Ihr System zuerst aktualisieren und dann einige grundlegende Programme installieren:

```bash
# System aktualisieren
sudo apt update && sudo apt upgrade -y

# Notwendige Programme installieren
sudo apt install pv tree rsync -y
```

## USB-Gerät finden

Um angeschlossene USB-Geräte aufzulisten, können Sie den folgenden Befehl verwenden:

```bash
# USB-Geräte auflisten
lsblk | grep -i usb
```

## Datenkopie-Skript

Im Repository finden Sie ein Skript namens `kopieren_von_usb.sh`. Mit diesem Skript können Sie Daten von einem USB-Gerät zu einem Zielverzeichnis auf Ihrem Computer kopieren.

Bevor Sie das Skript ausführen, sollten Sie sicherstellen, dass die Pfade im Skript korrekt sind und dass Sie dem Skript Ausführungsrechte gegeben haben:

```bash
chmod +x kopieren_von_usb.sh
```

Zum Ausführen des Skripts:

```bash
./kopieren_von_usb.sh
```

**Hinweis:** Testen Sie dieses Skript zunächst mit einem kleinen Daten-Set, um sicherzustellen, dass alles wie erwartet funktioniert.

---

## Beitrag

Falls Sie Verbesserungsvorschläge oder Anmerkungen zu den Skripten oder Anweisungen haben, zögern Sie nicht, einen Pull Request zu erstellen oder ein Issue zu öffnen.

---

Ich hoffe, dass Ihnen dieser `README.md`-Inhalt gefällt. Sie können ihn nach Belieben bearbeiten oder erweitern.
