owntrashmail
============

Own Trashmailservice

**Installation**
Ich gehe in dieser Installation davon aus, dass "qdated" in dem Ordner ~/bin/qdated vorhanden und konfiguriert ist.

* Git Owntrashmail clonen mittels
  * git clone LINK
* master.zip herunterladen und nach ~/bin/qdated entpacken
* Alle vier neuen Dateien mittels:
  * 'chmod +x DATEINAME.sh' beschreibbar machen (ohne Anführungszeichen)
* Dateien mittels nano oder vi öffnen und Prefix sowie Domain anpassen gffl den Pfad der qdated Umgebung
* Dateien wie folgt ausführen:
  * ./generate_trash_mail.sh
  * ./parse_trashmail.sh
* Neuen Crontab anlegen_
  * 'crontab -e'
  * '0 0 * * * ~/bin/qdated/remove_expired_trashmails.sh' in die letzte Zeile (ohne Anführungszeichen)
* Die index.php kommt entweder in den Ordner auf den die Subdomain verweist oder in euern Document Root.

