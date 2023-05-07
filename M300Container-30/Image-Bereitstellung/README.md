Image Bereitstellung
===

Dieses Dockerfile erstellt ein Image für einen Apache Webserver auf Basis des offiziellen Ubuntu 20.04 Images. Der Apache wird installiert, eine Beispiel-Webseite erstellt und der Port 80 wird für eingehende Verbindungen freigegeben. Die Zeitzone wird auf Europa/Berlin gesetzt.


Das erstellte Image des Apache-Webservers kann sowohl in einem privaten Unternehmen als auch auf Docker-Hub hochgeladen werden, um es später auf anderen Systemen oder in der Cloud zu verwenden. Durch das Hochladen in ein privates Unternehmen können Sie das Image innerhalb Ihres Netzwerks oder auf Ihren eigenen Servern speichern und verteilen, während das Hochladen auf Docker-Hub das Image der breiten Öffentlichkeit zugänglich macht.

### **Erstelle ein Image**
```
docker build -t mein-apache-server .
```