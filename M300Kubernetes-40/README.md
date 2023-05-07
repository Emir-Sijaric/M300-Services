Grundbegriffe
===
Service Discovery ist der Prozess, bei dem Clients Verbindungsinformationen zu passenden Instanzen eines Services erhalten. Es hilft dabei, die Interaktion und Koordination zwischen den verschiedenen Komponenten eines verteilten Systems oder einer Mikroservices-Architektur zu erleichtern.

Service Discovery Health Checking was ist das ?

Health Checking ist eine wichtige Funktion von Service Discovery, die dazu beiträgt, die Gesundheit von Instanzen eines Services zu überwachen. Hierbei wird in regelmäßigen Abständen überprüft, ob die Instanzen des Services erreichbar sind und ob sie ordnungsgemäß funktionieren.

Service Discovery Failover was ist das ?

Failover ist eine weitere wichtige Funktion von Service Discovery, die dazu beiträgt, die Ausfallsicherheit von verteilten Systemen und Mikroservices-Architekturen zu verbessern. Wenn eine Instanz eines Services ausfällt oder nicht mehr erreichbar ist, kann Service Discovery automatisch auf eine andere Instanz des Services umschalten, um sicherzustellen, dass die Anfragen weiterhin bearbeitet werden können.

Lastenverteilung
===

Lastverteilung bezeichnet den Prozess der Verteilung von Arbeitslasten (z.B. Anfragen, Berechnungen oder Daten) auf mehrere parallel arbeitende Systeme oder Ressourcen.

Apache-Server
===

Die .yaml-Datei ist eine Konfiguration für eine Kubernetes-Deployment und Service für eine Apache-Webanwendung. Das Deployment verwendet ein httpd:latest-Image auf Port 80 mit dem Label app: apache, während der Service den eingehenden Traffic auf Port 80 an das Deployment weiterleitet und einen Node-Port auf 30080 öffnet.

Cluster
===
Diese YAML-Datei definiert eine Kubernetes-Deploymentkonfiguration mit einem "master"- und zwei "worker"-Pods, die die nginx-Image verwenden. Jeder Pod hört auf Port 80 und hat spezifische CPU- und RAM-Ressourcenlimits. Es gibt auch zwei Services, "master-service" und "worker-service", die ClusterIP-Typ sind und auf Port 80 hören. Der "master-service" ist mit dem "master"-Pod und der "worker-service" ist mit den "worker"-Pods verbunden.