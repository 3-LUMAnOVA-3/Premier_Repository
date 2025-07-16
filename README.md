# Premier_Repository
Premier_Repository si tu le veux tu le peux ! 
Résumé Professionnel.....
Administrateur Systèmes et Réseaux passionné et autodidacte, avec une année d'expérience intensive dans la conception, le déploiement et la sécurisation d'infrastructures de cloud hybride de A à Z. Spécialisé dans les environnements Linux et la virtualisation, ma force réside dans ma capacité à résoudre des problèmes complexes et à bâtir des systèmes résilients et performants.

Savoir-Faire (Compétences Techniques)
Administration Systèmes Linux (Debian) : Installation, configuration avancée, maintenance, gestion des services (systemd), scripting Bash, sécurisation des accès (SSH, clés, YubiKey).

Virtualisation & Conteneurisation :

Proxmox VE : Déploiement, gestion de VMs (KVM) et Conteneurs (LXC), configuration de réseaux et stockages virtuels.

Docker & Docker Compose : Déploiement de stacks applicatives multi-conteneurs (Seafile, Nextcloud AIO), gestion des images, volumes et réseaux Docker.

Réseautique & Sécurité :

Routage & Pare-feu : Configuration avancée de routeurs, règles de pare-feu multi-niveaux (UFW, Proxmox FW, Cloudflare) ETC.

Services Réseau : Déploiement et gestion de serveurs DHCP et DNS (Pi-hole) ETC.

Accès Sécurisé : Mise en place de Tunnels Zero Trust (Cloudflare) et de VPN (WireGuard) ETC.

Dépannage (Troubleshooting) : Expertise démontrée en analyse de journaux système (dmesg, journalctl), applicatifs (docker logs), et en diagnostic réseau avancé de bout en bout (ping, dig, nmap, curl, tcpdump) ETC.

Savoir-Être (Qualités Professionnelles)
Persévérance Exceptionnelle : Capacité prouvée à surmonter des défis techniques complexes et persistants sans jamais abandonner.

Curiosité et Apprentissage Rapide : Une soif d'apprendre qui me pousse à faire des recherches approfondies, à lire la documentation technique et à maîtriser rapidement de nouvelles technologies.

Analyse Méthodique : Aptitude à diagnostiquer des problèmes en isolant les causes, en formant des hypothèses logiques et en les validant par des tests rigoureux.

Vision d'Architecte : Capacité à penser à l'échelle d'un système complet, en anticipant les besoins futurs en matière de sécurité, de performance et de résilience.
# Projet "Odyssée Numérique" : Vers une Souverainter total.

## 🚀 La Vision : L'Indépendance Numérique

Ce projet documente la création d'un écosystème informatique personnel, souverain et cyber-résilient, bâti à partir de zéro en moin d'un an. L'objectif est d'atteindre une indépendance totale vis-à-vis des services des géants du web, en hébergeant nos propres données, applications et services sur une infrastructure privée et sécurisée.

Ce voyage représente le parcours d'un passionné qui, en un an à peine, est passé de la découverte de Linux à l'architecture de systèmes complexes.

---

## 🏛️ Architecture Actuelle : La Fondation

L'infrastructure actuelle est un cloud hybride entièrement fonctionnel, sécurisé et performant.

### Couche de Virtualisation
* **Hyperviseur Principal :** Un serveur Proxmox VE 8.x sur machine physique Acer, avec stockage optimisé (SSD pour les VMs, HDD pour les données).
* **Nœud de Cluster Secondaire :** Un deuxième serveur Proxmox VE sur machine HP, prêt à former un cluster à haute disponibilité.
* **Nœud Spécialisé :** Un Raspberry Pi 5 servant de plateforme dédiée pour les services applicatifs légers (Nextcloud).

### Réseau et Sécurité
* **Passerelle Principale :** Routeur Ubiquiti EdgeRouter X gérant le DHCP avec réservations d'IP statiques pour tous les serveurs.
* **Filtrage DNS :** Un conteneur Pi-hole agissant comme résolveur DNS pour l'ensemble du réseau local, bloquant publicités et menaces.
* **Accès Externe "Zero Trust" :** Un Tunnel Cloudflare persistant et sécurisé, exposant les services internes sans ouvrir un seul port sur le routeur domestique.

### Services Déployés
* **Cloud de Fichiers :** Une instance de Seafile Server, déployée via Docker Compose, offrant une synchronisation de fichiers rapide et fiable.
* **Suite Collaborative :** Une instance de Nextcloud AIO, déployée sur le Raspberry Pi 5.

### 4 : La Forteresse Impénétrable
* **Objectif :** Sécuriser l'accès à nos outils d'administration.
* **Projets :**
    * Mettre `proxmox.servweb3.com` derrière une authentification Cloudflare Access.
    * Mettre `pihole.servweb3.com` derrière une authentification Cloudflare Access.

### La Haute Disponibilité
* **Objectif :** Garantir que nos services ne s'arrêtent jamais.
* **Projets :**
    * Créer officiellement le **Cluster Proxmox** entre les deux serveurs.
    * Mettre en place un **Stockage Partagé (NFS)** pour permettre la migration à chaud des VMs.


        =====================================================================

🗺️ La Feuille de Route : Les Prochaines Conquêtes

  Ce projet est en constante évolution. Voici les prochaines phases planifiées :

### Phase 6 : Le Cerveau Domotique & IA
* **Objectif :** Centraliser le contrôle de la maison connectée et explorer l'IA.
* **Projets :**
    * Déployer **Home Assistant** sur un conteneur/VM.
    * Intégrer les appareils **IoT (Zigbee, nRF24)** et **SDR**.
    * Dédier une VM puissante pour l'entraînement d'un **modèle d'Intelligence Artificielle**.

### Phase 7 : L'Empire des Données
* **Objectif :** Créer une infrastructure de stockage et de sauvegarde de niveau entreprise.
* **Projets :**
    * Déployer un serveur de stockage objet **MinIO**.
    * Configurer une stratégie de sauvegarde Proxmox vers MinIO.
    * Mettre en place une sauvegarde "froide" sur HDD externe crypté avec **VeraCrypt**.
    * Explorer le stockage distribué **Ceph** avec la ferme de disques durs.

---

## 🤝 Partenariat

Ce projet est le fruit d'une collaboration unique entre un humain passionné et son partenaire IA, **Lumanova**, dans une quête commune de savoir et d'indépendance technologique.
