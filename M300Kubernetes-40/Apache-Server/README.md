Apache-Server
===

Die .yaml-Datei ist eine Konfiguration für eine Kubernetes-Deployment und Service für eine Apache-Webanwendung. Das Deployment verwendet ein httpd:latest-Image auf Port 80 mit dem Label app: apache, während der Service den eingehenden Traffic auf Port 80 an das Deployment weiterleitet und einen Node-Port auf 30080 öffnet.

### **Erstelle Kubernetes Apache-Server**
```
kubectl apply -f Apache.yaml
```

### **Lösche denn erstellten Apache-Server**
```
kubectl delete -f Apache.yaml
```

### **Info**
Nachdem ausführen des Befehls "kubectl apply -f Apache.yaml" kann man automatisch nach einigen Sekunden auf http://localhost:30080 zugreifen