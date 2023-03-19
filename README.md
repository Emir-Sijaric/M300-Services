# M300-Services
## 10-Toolumgebung
Bevor wir mit dem Modul starten brauchen wir zuerst eine Toolumgebung wo wir unser Wissen testen können und auch dazu lernen können.

Wir arbeiten mit dem Terminal (Bash), sowie mit dem Visual Studio Code, aber zu diesem kommen wir später.

### Github Account erstellen

1. Zuerst muss man die eigene Mail angeben.

2. Danach muss man ein Kennwort angeben, für unseren Account.

3. Nachdem man dies angegeben hat muss man einen eigenen Benutzernamen angeben.

4. Nachdem man dies gespeichert hat, muss man sich Verifizieren per Mail und sich anschliessend einmal anmelden.

### Repository erstellen

1. Zuerst meldet man sich auf github an.

2. Danach kann oben recht zu seinen eigenen Repositorys gehen und anschliessend auf Repository erstellen klicken.

screenshot/Repository-erstellen.jpg

### SSH-Key erstellen

1. Zuerst muss man den Github Account Mail eingeben
        ssh-keygen -t rsa -b 4096 -C "beispiel@beispiel.com"

2. Dann erstellen wir danach einen SSH-Key
        Generating public/private rsa key pair.

3. Danach kommt die Namensabfrage für den Schlüssel
        Enter a file in which to save the key (~/.ssh/id_rsa): 

4. Danach muss man ein Kennwort setzen
        Enter passphrase (empty for no passphrase): [Passwort]
        Enter same passphrase again: [Passwort wiederholen]

