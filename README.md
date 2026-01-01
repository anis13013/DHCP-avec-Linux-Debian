# DHCP-avec-Linux-Debian

### A] Le serveur DHCP possède un nom d'hôte adapté à son rôle ainsi qu'une configuration IP correcte

![image](https://github.com/anis13013/DHCP-avec-Linux-Debian/blob/2308d57e33002c328e6918f064c55bd8e513c1ff/DHCP%20Linux/ServDHCPconfig1.PNG)



![image](https://github.com/anis13013/DHCP-avec-Linux-Debian/blob/2308d57e33002c328e6918f064c55bd8e513c1ff/DHCP%20Linux/ServDHCPconfig2.PNG)

---

### Configuration Serveur-DHCP
![image](https://github.com/anis13013/DHCP-avec-Linux-Debian/blob/2308d57e33002c328e6918f064c55bd8e513c1ff/DHCP%20Linux/ServDHCPconfig3.PNG)

---

### B] La configuration du serveur permet bien aux client d'obtenir une adresse IP par le serveur DHCP dans la plage d'adresse donnée
(préalable installer) => `apt install isc-dhcp-client` ensuite `sudo dhclient -v`

#### [CLIENT 1]

![image](https://github.com/anis13013/DHCP-avec-Linux-Debian/blob/2308d57e33002c328e6918f064c55bd8e513c1ff/DHCP%20Linux/ip%20client%201.PNG)

---

### C] Le client qui possède la réservation n'obtient pas une autre IPv4, même s'il demande un renouvellement

(libérer)`sudo dhclient -r`, (redemander) `sudo dhclient -v`

#### [CLIENT 2]

![image](https://github.com/anis13013/DHCP-avec-Linux-Debian/blob/2308d57e33002c328e6918f064c55bd8e513c1ff/DHCP%20Linux/ip%20client%202.PNG)
