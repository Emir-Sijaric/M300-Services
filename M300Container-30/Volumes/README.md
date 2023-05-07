Volumes
===

Volumes in Docker ermöglichen es, Daten zwischen Containern auszutauschen und persistent zu speichern. Sie bieten Datenspeicherung, Persistenz und Flexibilität, um Daten in einem Container-Cluster zu teilen und zu skalieren.

### **MySQL**
Dieses Dockerfile erstellt ein MySQL-Image mit spezifischen Konfigurationen. Es setzt Umgebungsvariablen, erstellt ein Volume für MySQL-Daten und öffnet den Port 3306.

### **Test**
Dieses Dockerfile erstellt ein Image auf Basis des offiziellen Busybox-Images. Es erstellt ein Volume mit dem Namen test-volume und startet die Busybox-Shell als Standardkommando.

### **Erstelle ein Image**
```
docker build -t my-mysql-image .
```

### **Erstelle des MySQL Container**
```
docker run --name my-mysql-container -p 3306:3306 -d my-mysql-image
```

### **Testen ob man sich mit dem Volume verbinden kann**
```
docker exec -it my-mysql-container mysql -u myuser -pmypassword mydatabase
```

### **Info**
Wenn du erfolgreich mit der Datenbank verbunden bist, bedeutet das, dass das Volume korrekt erstellt wurde und funktioniert.