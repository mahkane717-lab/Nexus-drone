# Nexus-drone
Drone agricole intelligent basé sur l'IA pour la détection des maladies, la prévention et l'irrigation ciblée.

#  NEXUS — Drone Agricole Intelligent

> Drone agricole intelligent basé sur l'Intelligence Artificielle, la Computer Vision et le GPS pour surveiller les cultures, détecter les maladies, prévenir les risques et permettre une irrigation ciblée.

##  Présentation

**NEXUS** est un projet de robotique et d'intelligence artificielle conçu pour répondre aux besoins de l'agriculture africaine.

Le système combine un drone autonome, une caméra, un ordinateur embarqué, l'IA et des capteurs afin d'analyser les cultures depuis les airs.

### Objectifs

- Surveiller les cultures
- Capturer des images aériennes
- Détecter les maladies avec l'IA
- Identifier les zones nécessitant une intervention
- Localiser les problèmes grâce au GPS
- Cartographier les parcelles
- Prévenir les risques agricoles
- Permettre une irrigation ciblée

---

## Intelligence Artificielle

L'IA de NEXUS analyse les images capturées par la caméra du drone.

### Pipeline IA

```text
📷 Caméra
    ↓
🖼️ Image de la culture
    ↓
🔍 Computer Vision
    ↓
🧠 Modèle IA
    ↓
🌱 Analyse de la plante
    ↓
⚠️ Détection d'un problème
    ↓
📍 Localisation GPS
    ↓
Rapport agricole
```

Les modèles pourront notamment utiliser :

- Python
- OpenCV
- TensorFlow / PyTorch
- YOLO
- MobileNet
- NumPy
- Pandas

---

## Architecture du drone

```text
                   NEXUS
                     │
          ┌──────────┴──────────┐
          │                     │
       Pixhawk             Raspberry Pi
          │                     │
     Contrôle du vol       Intelligence IA
          │                     │
    ┌─────┼─────┐             
    │     │     │           Caméra
   ESC   ESC   ESC              │
    │     │     │               ↓
  Moteurs  →  Vol         Analyse des cultures
                              │
                              ↓
                          GPS / IA
                              │
                              ↓
                        Intervention
```

---

##  Système électrique

Le prototype utilise principalement :

- Batterie LiPo 4S 14,8 V
- Power Module
- Power Distribution Board
- Pixhawk 2.4.8
- 4 ESC 30 A
- 4 moteurs brushless
- Raspberry Pi 4/5
- Raspberry Pi Camera
- GPS + compas
- Télémétrie
- Pompe 12 V
- Servos

Le schéma électrique détaillé se trouve dans :

`docs/NEXUS_Drone_Agricole_Composants_Schema_Electrique.pdf`

---

## Composants principaux

| Composant | Quantité |
|---|---:|
| Châssis quadricoptère | 1 |
| Moteurs brushless 2212 / 920 KV | 4 |
| ESC 30 A | 4 |
| Hélices | 2–3 jeux |
| Batterie LiPo 4S 5000 mAh | 1+ |
| Pixhawk 2.4.8 | 1 |
| GPS + compas | 1 |
| Raspberry Pi 4/5 | 1 |
| Caméra | 1 |
| Module télémétrie | 1 paire |
| Radiocommande + récepteur | 1 |
| Pompe DC 12 V | 1 |
| Réservoir 1–2 L | 1 |
| Capteurs environnementaux | 1 lot |

---

## Budget prototype

Budget cible :

**7 000 DH**

Le budget est réparti entre :

- Propulsion
- Contrôleur de vol
- GPS et télémétrie
- Raspberry Pi
- Caméra
- Batterie
- Capteurs
- Système d'irrigation
- Câblage et sécurité

> Les prix peuvent varier selon les fournisseurs et la disponibilité des composants au Maroc.

---

##  Irrigation ciblée

NEXUS pourra identifier les zones nécessitant une intervention.

```text
Culture
    ↓
  Image
    ↓
   IA
    ↓
Zone à risque détectée
    ↓
   GPS
    ↓
 Intervention ciblée
```

Le prototype sera d'abord testé avec de l'eau avant toute utilisation agricole réelle.

---

## Navigation

Le système de navigation repose sur :

- Pixhawk
- ArduPilot
- GPS
- Compas
- IMU
- Télémétrie
- Radiocommande

Fonctions prévues :

- Stabilisation
- Vol manuel
- Maintien de position
- Missions GPS
- Retour au point de départ
- Géorepérage
- Surveillance de la batterie

---

## 💻 Technologies

### Intelligence artificielle
- Python
- TensorFlow / PyTorch
- OpenCV
- YOLO
- MobileNet

### Robotique
- Pixhawk
- ArduPilot
- MAVLink
- Raspberry Pi

### Développement
- GitHub
- VS Code
- Linux
- Python
- JavaScript

---

## 📅 Calendrier du projet

| Période | Travail |
|---|---|
| Semaines 1–2 | Conception |
| Semaines 3–4 | Assemblage du drone |
| Semaines 5–6 | Pixhawk + GPS |
| Semaines 7–8 | Premiers vols |
| Semaines 9–10 | Raspberry Pi + caméra |
| Semaines 11–12 | Développement IA |
| Semaine 13 | IA + GPS |
| Semaine 14 | Système d'irrigation |
| Semaine 15 | Dashboard |
| Semaine 16 | Tests et démonstration |

---

## 📂 Structure du projet

```text
NEXUS-Drone/
│
├── README.md
│
├── docs/
│   └── NEXUS_Drone_Agricole_Composants_Schema_Electrique.pdf
│
├── hardware/
│   ├── components.md
│   └── wiring/
│
├── ai/
│   ├── datasets/
│   ├── training/
│   ├── models/
│   └── inference/
│
├── flight/
│   ├── ardupilot/
│   └── missions/
│
├── irrigation/
│   ├── pump.py
│   └── servo.py
│
└── software/
    ├── vision/
    ├── mavlink/
    └── dashboard/
```

---

## 🚀 Vision du projet

NEXUS a pour ambition de développer une solution technologique adaptée aux réalités de l'agriculture africaine.

À long terme, le projet pourra évoluer vers :

- 🌾 Agriculture de précision
- 🛰️ Cartographie intelligente
- 🤖 Détection précoce des maladies
- 💧 Gestion intelligente de l'eau
- 📊 Analyse des parcelles
- 📱 Application mobile agricole
- 🚁 Flotte de drones agricoles

---

## 👩‍💻 Projet

**NEXUS — Drone Agricole Intelligent**

Projet de robotique, Intelligence Artificielle et agriculture de précision.

**Développeuse : Mah Kane**

📍 Maroc  
🎓 Ingénierie Informatique & Intelligence Artificielle

---

## ⭐ Statut

🚧 **Projet en cours de développement**

Le prototype matériel, le système IA et les logiciels embarqués sont progressivement développés et testés.
