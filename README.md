Voici une version optimisée pour un README GitHub, intégrant tous les éléments demandés avec une mise en forme professionnelle :


## 📊 African Plums Classification System

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red)
![CustomTkinter](https://img.shields.io/badge/UI-CustomTkinter-green)

**Solution complète de classification des prunes africaines avec interface desktop**  
*Projet développé lors du Hackathon JCIA 2023*

## ✨ Fonctionnalités Principales
- 🖼️ **Traitement avancé des images** : suppression de fond, augmentation des données
- 🤖 **Double modèle CNN** : classification globale + détection des défauts
- 💻 **Interface utilisateur intuitive** (CustomTkinter)
- 📊 **Rapports détaillés** : métriques, courbes d'apprentissage
- 🚀 **Prédiction en temps réel**

**## 📊 Choix Techniques**

### Modèles Retenus
| Modèle        | Architecture       | Justification                                                                 |
|---------------|--------------------|-------------------------------------------------------------------------------|
| Global Model  | ResNet18 fine-tuné | Bon compromis précision/performance pour la classification binaire            |
| Defect Model  | ResNet18 fine-tuné    | Excellente détection des petits défauts grâce à sa structure compacte         |

### Pourquoi une Application Desktop ?
- 🔒 **Souveraineté des données** : traitement local sans cloud
- 🌍 **Accessibilité** : fonctionne sans internet en zones rurales
- ⚡ **Performance** : latence réduite vs solution web
- 🛠️ **Maintenance simplifiée** : déploiement unique





## 📊 Installation
```bash
# 1. Cloner le dépôt
git clone https://github.com/HACKATHON_JCIA_CLASSIFICATION_DES_PRUNES/african-plums-classifier.git
cd african-plums-classifier
```

# 2. Créer l'environnement
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
.\venv\Scripts\activate  # Windows
```
# 3. Installer les dépendances
```bash
pip install -r requirements.txt
```

## 🚀 Utilisation
```bash
# Mode entraînement
python train.py --epochs 50 --batch_size 32
```
# Mode interface
python PlumClassifier_Interface.py


## 📊 Performance
| Métrique       | Global Model | Defect Model |
|----------------|-------------|-------------|
| Précision      | 80.9%       | 82.7%       |
| Rappel         | 85.5%       | 86.2%       |
| F1-score       | 0.85        | 0.87        |

## 👥 Équipe
- **FOTSING ENGOULOU Simon Gaetan**
- **BALEKAMEN LANDRY** 
- **LEUMEN JOYCE** 

## 📜 Licence
Apache 2.0 - [Voir le fichier LICENSE](LICENSE)

