
# 🧬 Cancer Detection App

Détection assistée par intelligence artificielle des anomalies médicales sur des images telles que radiographies, IRM ou rayons X.  
Cette application fullstack combine **Computer Vision**, **Cloud**, et **DevOps** pour offrir une solution professionnelle et évolutive.

---

## 🌟 Pourquoi ce projet ?

Ce projet personnel a pour objectif de :
- **Détecter automatiquement** des anomalies sur des images médicales (cancer / non cancer)
- **Héberger une application robuste** dans le cloud (AWS, Kubernetes)
- **Développer un outil complet** : Backend, Frontend et IA intégrée
- **Améliorer mes compétences** en Computer Vision, Java, Cloud et DevOps

---

## 🚀 Fonctionnalités principales

✅ Authentification via AuthKey (JWT)  
✅ Upload d’images médicales (rayons X, IRM, etc.)  
✅ Analyse automatique via modèle IA (Cancer/Non cancer)  
✅ Historique des résultats avec filtres  
✅ Interface utilisateur (ElectronJS)  
✅ Déploiement Cloud (AWS EKS, S3, DynamoDB)  

---

## 🏗️ Stack technique

| Module        | Technologies principales                              |
|---------------|--------------------------------------------------------|
| Backend       | Java 17 / Spring Boot / JWT / REST API                |
| Frontend      | ElectronJS / HTML / CSS / JS                           |
| IA / Modèle   | Python / PyTorch / FastAPI / OpenCV / Albumentations   |
| Cloud & Infra | Docker / Kubernetes / AWS (EKS, S3, DynamoDB)          |

---

## 🧩 Schéma d’architecture (simplifié)

```
┌──────────────────────────────┐
│         Utilisateur          │
└──────────────┬───────────────┘
               │ (AuthKey / JWT)
┌──────────────▼───────────────┐
│        Frontend Electron     │
│  - Upload images             │
│  - Lancer analyse            │
│  - Historique des résultats  │
└──────────────┬───────────────┘
               │ REST API
┌──────────────▼───────────────┐
│        Backend Java API      │
│  - Authentification JWT      │
│  - Upload / Analyse          │
│  - Historique / Filtres      │
└──────────────┬───────────────┘
               │
        ┌──────▼───────────────┐
        │  Serveur IA (Python) │
        │  - Analyse d'image   │
        └──────┬───────────────┘
               │
        ┌──────▼─────────────────────┐
        │        Stockage Cloud      |
        │  - S3 : images             │
        │  - DynamoDB : résultats    │
        └────────────────────────────┘
```

---

## 📂 Structure du projet

```
cancer-detection-app/
├── backend/         # API Java (Spring Boot)
├── frontend/        # App ElectronJS
├── model/           # IA (Python) et données
├── k8s/             # Fichiers Kubernetes (YAML)
└── README.md
```

---

## 📦 Setup rapide

### Backend (Java)
```
cd backend
./mvnw spring-boot:run
```

### Frontend (Electron)
```
cd frontend
npm install
npm start
```

### IA (Python)
```
cd model
python train_model.py
```

---

## 📊 Roadmap du projet

✅ Authentification (JWT)  
✅ Upload et gestion d’images  
✅ Entraînement modèle IA (Cancer/Non cancer)  
✅ Découpe et génération d’images augmentées  
✅ Intégration API/Modèle  
✅ Frontend Electron (Upload, Analyse, Historique)  
✅ Dockerisation complète  
✅ Déploiement AWS (EKS, S3, DynamoDB)  
✅ Tests unitaires et end-to-end  
✅ Documentation finale  

---

## 📌 Datasets et ressources

- [The Cancer Imaging Archive (TCIA)](https://www.cancerimagingarchive.net/)
- [Kaggle - Cancer Datasets](https://www.kaggle.com/datasets)
- [ChestX-ray14 (NIH)](https://nihcc.app.box.com/v/ChestXray-NIHCC)

---

## 🙌 Auteur

Fabien Amet – Ingénieur IA passionné par le Computer Vision et le développement cloud.  
Projet personnel dans le cadre de ma montée en compétences.

---

## 📫 Contact

Pour toute question ou collaboration :  
[LinkedIn](www.linkedin.com/in/fabien-a-670883146)  
fabienamet@gmail.com (à adapter 😉)
