# Erstellen einer EC2 instanz und kopieren einer Datei auf die Instanz

- Fahre die Sandbox Umgebung hoch und navigiere in die AWS Zentrale
- Erstelle eine EC2 Instanz mit private key
- Verschiebe den private key aus deinem windows donwloads Ordner in WSL
- Gib dem private key angemessene Rechte
- Verbinde dich über ssh mit der erstellten instanz: ssh -i \<pfad zur .pem datei\> ec2-user@\<public-ip-der-ec2-instanz\>
- Nachdem du überprüft hast, dass die Verbindung klappt, beende die Verbindung wieder
- Erstelle eine Datei lokal in deinem WSL
- Kopiere die Datei mit ssh copy auf deine Instanz: scp -i \<pfad zur .pem datei\> \<zu kopierende Datei\> ec2-user@\<ip-adresse\>:\<dateipfad\>
