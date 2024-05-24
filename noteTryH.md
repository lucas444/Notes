# Note try hack me
## Serveur C2
### *Exemple*
- *Metasploit*
- *Armitage*
- *Powershell Empire/Starkiller*
- *Covenant*
- *Sliver*
- *Brute Ratel*

### Mettre en place un serveur C2
---
---
---

## Red Team Recon

### Passive Recon: 

1) can be carried out by watching passively

Passive recon doesn't require interacting with the target. In other words, you aren't sending any packets or requests to the target or the systems your target owns. Instead, passive recon relies on publicly available information that is collected and maintained by a third party. Open Source Intelligence (OSINT) is used to collect information about the target and can be as simple as viewing a target's publicly available social media profile. Example information that we might collect includes domain names, IP address blocks, email addresses, employee names, and job posts. In the upcoming task, we'll see how to query DNS records and expand on the topics from the Passive Reconnaissance room and introduce advanced tooling to aid in your recon.

### Active Recon: 

2) requires interacting with the target to provoke it in order to observe its response.

Active recon requires interacting with the target by sending requests and packets and observing if and how it responds. The responses collected - or lack of responses - would enable us to expand on the picture we started developing using passive recon. An example of active reconnaissance is using Nmap to scan target subnets and live hosts. Other examples can be found in the Active Reconnaissance room. Some information that we would want to discover include live hosts, running servers, listening services, and version numbers.

Active recon can be classified as:

    External Recon: Conducted outside the target's network and focuses on the externally facing assets assessable from the Internet. One example is running Nikto from outside the company network.
    Internal Recon: Conducted from within the target company's network. In other words, the pentester or red teamer might be physically located inside the company building. In this scenario, they might be using an exploited host on the target's network. An example would be using Nessus to scan the internal network using one of the target’s computers.

---

### Tools 

      Whois
      nslookup
      dig
      host
      traceroute 


### Advenced Seaching 

|*Symbol / Syntax*|*Function*|
|---------------|--------|
|"search phrase"|Find results with exact search phrase|
|OSINT filetype:pdf|Find files of type PDF related to a certain term.|
|salary site:blog.tryhackme.com|Limit search results to a specific site.|
|pentest -site:example.com|Exclude a specific site from results|
|walkthrough intitle:TryHackMe|Find pages with a specific term in the page title.|
|challenge inurl:tryhackme|Find pages with a specific term in the page URL.|


>Search advanced  avec [Google advanced_search](https://www.google.com/advanced_search)\
>Advanced syntax on [DuckDuckGo](https://duckduckgo.com/duckduckgo-help-pages/results/syntax/) Search \
>[Google Hacking Database](https://www.exploit-db.com/google-hacking-database)


[**Viewdns.info**](https://viewdns.info/) pour trouver des information spécifique(DNS/Reverse IP Lookup) \
[**Threat Intelligence Platform**](https://threatintelligenceplatform.com/) \
[Censys Search](https://search.censys.io/)\
[shodan](https://cli.shodan.io/) 

### advenced tools 

[Recon-ng](https://github.com/lanmaster53/recon-ng) framework that helps automate the OSINT work.
[Maltego](https://www.maltego.com/) application qui combine la cartographie mentale et l'OSINT.
 

## Linux Fondamental 

### Linux process

#### Affiche les process
ps : pour voir les prossessus en cours 
ps aux : pour voir les prossessus en cours  de tout les utilisateur 
top : prosses en temps real 

#### Kill process
kill "pid" : tu le prosess "pid"

    SIGTERM - Kill the process, but allow it to do some cleanup tasks beforehand
    SIGKILL - Kill the process - doesn't do any cleanup after the fact
    SIGSTOP - Stop/suspend a process
    
### **Systemd** 

Systemd :
    Systemd est un système d'initialisation pour les systèmes d'exploitation basés sur Linux. Il remplace les anciens systèmes d'initialisation tels que SysV init. Systemd est responsable de l'amorçage du système, de la gestion des services, des démons, des sockets, des périphériques, etc.
    Il suit une approche plus moderne et fournit une gestion plus avancée des démons système, permettant un démarrage plus rapide, une gestion plus efficace des ressources et d'autres fonctionnalités.

Systemctl :
    Systemctl est une commande utilisée pour interagir avec le système de gestion de services systemd. Elle permet à l'administrateur système de contrôler les services, les cibles, les sockets et d'autres unités gérées par systemd.
    Avec systemctl, vous pouvez activer ou désactiver des services, démarrer ou arrêter des services, vérifier l'état des services, etc.


systemd : start le prosses
systemctl [option][service]: sart au boot

Voici les commandes `systemctl` avec des exemples, formatées en Markdown :

1. **Démarrer un service :**
   ```bash
   systemctl start nom_du_service
   ```

2. **Arrêter un service :**
   ```bash
   systemctl stop nom_du_service
   ```

3. **Redémarrer un service :**
   ```bash
   systemctl restart nom_du_service
   ```

4. **Activer un service au démarrage du système :**
   ```bash
   systemctl enable nom_du_service
   ```

5. **Désactiver un service au démarrage du système :**
   ```bash
   systemctl disable nom_du_service
   ```

6. **Vérifier l'état d'un service :**
   ```bash
   systemctl status nom_du_service
   ```

7. **Afficher les journaux d'un service :**
   ```bash
   journalctl -u nom_du_service
   ```

8. **Lister toutes les unités actives :**
   ```bash
   systemctl list-units
   ```

9. **Afficher les détails d'une unité spécifique :**
   ```bash
   systemctl show nom_de_l_unite
   ```
   


#### comande basique 

>wc 
stat 
du 
df

---

## **Weaponization**

For more information about red team toolkits, please visit the following: a [GitHub repository](https://github.com/infosecn1nja/Red-Teaming-Toolkit#Payload%20Development) that has it all, including initial access, payload development, delivery methods, and others. 
