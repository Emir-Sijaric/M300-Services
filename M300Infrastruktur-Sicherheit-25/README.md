M300 - 25 Infrastruktur-Sicherheit
===

VM Vagrantfile - Firewall
===
In diesem Beispiel werden zwei virtuelle Maschinen definiert: "firewall" und "web". Beide virtuellen Maschinen basieren auf Ubuntu "Xenial64".

Die "firewall"-VM hat die IP-Adresse "10.0.0.10" und wird über den Hostnamen "Firewall" identifiziert. Diese VM wird über eine Shell-Provisionierung konfiguriert, um das ufw-Paket zu installieren. Danach wird die ufw-Firewall so konfiguriert, dass sie den eingehenden Datenverkehr auf Port 80, eingehenden Datenverkehr von der IP-Adresse "10.0.2.2" auf Port 22 und eingehenden Datenverkehr von der IP-Adresse "10.0.0.20" auf Port 3306 erlaubt.
```
Vagrant.configure("2") do |config|
  config.vm.define :firewall do |firewall|
      firewall.vm.box = "ubuntu/xenial64"
      firewall.vm.network :private_network, ip: "10.0.0.10"
      firewall.vm.hostname = "Firewall"
      firewall.vm.provision "shell", inline: <<-SHELL
      apt-get update
      sudo apt-get install ufw
      sudo ufw allow 80/tcp
      sudo ufw allow from 10.0.2.2 to any port 22
      sudo ufw allow from 10.0.0.20 to any port 3306
      sudo ufw --force enable
      SHELL
  end
```

Die "web"-VM hat die IP-Adresse "10.0.0.20" und wird über den Hostnamen "web" identifiziert. Diese VM wird über eine Shell-Provisionierung mit dem Apache-Webserver installiert. Zusätzlich wird ein synchronisierter Ordner zwischen dem Host-Verzeichnis "html/" und dem Gast-Verzeichnis "/var/www/html" eingerichtet. Der Gast-Port 80 wird auf den Host-Port 8090 weitergeleitet.
```
config.vm.define :web do |web|
      web.vm.box = "ubuntu/xenial64"
      web.vm.network :private_network, ip: "10.0.0.20"
      web.vm.hostname = "web"
      web.vm.network "forwarded_port", guest:80, host:8090, auto_correct: true
      web.vm.synced_folder "html/", "/var/www/html"
      web.vm.provision "shell", inline: <<-SHELL
      sudo apt-get update
      sudo apt-get -y install apache2 
      SHELL
  end
```