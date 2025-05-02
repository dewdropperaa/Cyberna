# N3R Alert: DHL Maroc – Nouvelle Campagne de Smishing  
**Date :** 2 Mai 2025  
**Cible :** Clients DHL Maroc via SMS  
**URL Frauduleuse :** `https://dhl.onlineparcel.cfd`  
**Domaine :** `onlineparcel.cfd`  
**Statut :** Suspendu (`clientHold` par NameSilo)  
**Source :** SMS depuis `+63 910 629 3543` (Philippines)  

---

## **Résumé**  
Un SMS frauduleux imitant **DHL Maroc** annonce un colis bloqué à cause d’une **adresse incomplète**. Le message contient un lien malveillant et des instructions suspectes :  
- **Répondre "Y"** pour "activer" le lien (tentative de contournement des filtres anti-spam).  
- **Ouvrir dans Safari** (évite les bloqueurs sur iMessage).  

**Objectif :** Vol de données via un faux portail DHL.  

---

## **Indicateurs de Compromission (IoC)**  
| **Type**       | **Valeur**                      | **Détails**                     |  
|----------------|---------------------------------|---------------------------------|  
| **Domaine**    | `onlineparcel.cfd`              | `.cfd` = TLD suspect            |  
| **IP**         | `196.251.70.233` (Seychelles)   | Hébergement "bulletproof"       |  
| **ASN**        | `AS401120` (CHEAPY-HOST)        | Nouveau fournisseur (mai 2024)  |  
| **Registrar**  | NameSilo, LLC                   | Domaine créé le **11 avril 2025** |  

---

## **Investigation Technique**  
### **1. Analyse du Domaine**  
- **WHOIS** :  
  - Statut : `clientHold` (suspendu pour abus).  
  - Hébergeur : **Cheapy-Host** (Seychelles) → Héberge 38 autres sites frauduleux.  
- **URLScan.io** :  
  - Redirection vers une fausse page DHL (copie du design officiel).  
  - Code JavaScript pour voler les identifiants.  

### **2. Réputation de l’IP**  
- **AbuseIPDB** : Score de **98/100** (lié à des campagnes de phishing).  
- **VirusTotal** : 12/97 moteurs détectent le domaine comme malveillant.  

### **3. Tactiques de l’Attaquant (MITRE ATT&CK)**  
- **T1566.001** : Phishing par SMS.  
- **T1583.001** : Utilisation de domaines frauduleux.  

---

## **Conseils de Sécurité**  
✅ **Pour les utilisateurs :**  
- Ignorez les SMS non sollicités, même avec un logo DHL.  
- Vérifiez les domaines : **DHL n’utilise jamais `.cfd` ou `.sbs`**.  

✅ **Pour les entreprises :**  
- Bloquez les TLD suspects (`.cfd`, `.click`, `.sbs`) via des filtres DNS.  
- Formez les employés aux attaques par SMS.  

---

## **Contexte Régional**  
- **Augmentation de 30%** des attaques smishing au Maroc en 2025 (source : DGSN).  
- Liens possibles avec la campagne **"Darcula"** (utilisation de `.sbs` en 2024).  

---

## **Actions Recommandées**  
1. **Signaler** à :  
   - [PhishTank](https://phishtank.com)  
   - `abuse@namesilo.com` (registrar)  
2. **Surveiller** les nouveaux domaines sous `DNSOWL.COM`.  

---

## **À Retenir**  
> **"Un SMS urgent est souvent une arnaque."**  
> Restez sceptique. Vérifiez. Signalez.  

**Tags :** `#phishing` `#smishing` `#Maroc` `#DHL` `#CyberSecurity` `#TLP-CLEAR`  
