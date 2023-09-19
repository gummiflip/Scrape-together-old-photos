# Scrape-together-old-photos
Selbstverständlich! Hier ist ein einfaches Beispiel für eine `README.md` Datei für Ihr GitHub-Repository, das sich auf das Setup von Ubuntu und das Kopieren von Daten von einem USB-Gerät bezieht:

---

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
