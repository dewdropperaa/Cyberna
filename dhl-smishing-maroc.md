# Cyberna Alert: DHL Maroc – Phishing par SMS (Smishing)

** Date :** 16 Avril 2025  
** Cible :** Utilisateurs DHL Maroc via SMS de phishing  
** URL :** [https://dhl.com-postage.sbs/track](https://dhl.com-postage.sbs/track)  
** Domaine :** `dhl.com-postage.sbs`  
** Statut :** Inactif (domaine non enregistré au 16 avril 2025)  
**Source :** SMS depuis le numéro `+63 912 327 0564` (Philippines)

---

##  Résumé

Un SMS prétendant venir de **DHL Maroc** informait la victime qu’un colis était bloqué à cause d’un **code postal invalide**. Le message demandait de confirmer l’adresse sous 24 heures via un lien et contenait des instructions étranges : **répondre "Y"**, quitter le message, puis **ouvrir le lien dans Safari**. L’objectif : **voler des données personnelles via un faux site DHL**.

---

##  Indicateurs de Phishing

- **Expéditeur inconnu :** Numéro philippin `+63`, aucun lien avec DHL ou le Maroc.
- **Domaine frauduleux :** `dhl.com-postage.sbs` n'est **pas un domaine officiel**. Les seuls valides sont :
  - `www.dhl.com`
  - `dhl.ma`
- **Tactique d'urgence :** Limite de 24 heures pour manipuler la victime.
- **Instructions inhabituelles :** Répondre "Y" + Safari = tentative de contourner les protections iMessage.

---

##  Investigation Technique

| Outil         | Détails |
|---------------|---------|
| **URLScan.io** | Domaine actif vers décembre 2024 – page légère (502 bytes), hébergé aux **États-Unis**. |
| **VirusTotal** | 9/97 moteurs (ESET, Fortinet, Google Safebrowsing, G-Data) ont identifié le lien comme **phishing/malware**. Dernière analyse : 30 mars 2025. |
| **Whois**      | Domaine **désenregistré** au 16 avril 2025. Activité fluctuante, 2 IP et changements d’hébergement en 1 an. |
| **PhishTank**  | Signalé comme phishing le 15 avril 2025. En cours de validation. |

---

## Conseils de Sécurité

- Ne cliquez **jamais** sur des liens contenus dans des SMS non sollicités.
- Accédez à DHL uniquement via :
  - `www.dhl.com`
  - `dhl.ma`
- Signalez les SMS suspects à **Cyberna**, **GhostGuardian**, ou directement sur [PhishTank](https://phishtank.com).

---

##  Contexte

Ce type d’attaque s’inscrit dans une **tendance croissante en Afrique** :  
> Les attaques **smishing** ont augmenté de **22 % en 2024**, ciblant notamment les services postaux (DHL, Poste Maroc).

La campagne **Darcula** a été liée à des attaques similaires, avec utilisation de domaines `lookalike` (.sbs, .click) pour tromper les utilisateurs marocains.

---

##  À retenir

> **“Ce n’est pas parce qu’un SMS contient un logo connu qu’il est légitime.”**  
> Vérifie. Analyse.  Protège.  
>  
> Contribue à Cyberna pour exposer ces arnaques et éduquer notre communauté marocaine.

---

**Tags :** `#phishing` `#smishing` `#Morocco` `#DHL `#Cyberna` `#TLP-CLEAR`

