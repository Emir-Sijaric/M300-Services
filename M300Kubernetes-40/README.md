M300 - 40 Kubernetes (K8s)
===

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

Cluster
===

Ein Cluster ist eine Gruppe von verbundenen oder zusammengeschlossenen Computersystemen, die gemeinsam als ein System oder eine Einheit arbeiten. Die einzelnen Systeme in einem Cluster werden auch als Knoten bezeichnet. Ein Cluster wird verwendet, um die Leistung und Verfügbarkeit von Anwendungen und Diensten zu erhöhen, indem Ressourcen wie Prozessoren, Speicher und Netzwerkbandbreite zwischen den Knoten aufgeteilt werden.

Kubernetes
===
Kubernetes ist eine Open-Source-Plattform zur Automatisierung, Bereitstellung und Verwaltung von Containeranwendungen. Es dient als Orchestrierungswerkzeug, das die Skalierung, Überwachung und Lastverteilung von Containern auf mehreren Hosts oder Cloud-Plattformen erleichtert.

Kubernetes Cluster
===
Ein Kubernetes-Cluster besteht aus einem Master-Node, der die Kontrolle und Verwaltung des Clusters übernimmt, und mehreren Worker-Nodes, die die eigentlichen Anwendungen ausführen. Durch die Verwendung von Kubernetes-Clustern können Unternehmen ihre Anwendungen effizienter bereitstellen, skalieren und verwalten und gleichzeitig die Verfügbarkeit und Skalierbarkeit ihrer Anwendungen verbessern.


Reflexion
===

Als wir uns mit dem Thema Docker befasst haben, habe ich gemerkt, dass es besser ist zusammen zu arbeiten.Man kann sich gegenseitig unterstützen und so das Wissen erweitern.
Durch mehrere Versuche und mehrfachigen Fehlschlägen konnten wir unsere Docker-Umgebung zum laufen bringen. Mir ist aufgefallen, dass man das Dokumentieren mit den Testfällen
nicht unterschätzen sollte. Um zu bestätigen, dass die erstellten Container und Kubernetes funktionieren wird mithilfe Text und Screenshots im Github dokumentiert. So kann 
bestätigt werden, dass die erstellten Lösungen reproduzierbar und nachvollziehbar sind.
