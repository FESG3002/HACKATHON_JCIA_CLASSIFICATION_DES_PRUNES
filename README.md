🎯 HACKATHON_JCIA_CLASSIFICATION_DE_PRUNE
Pipeline complète de classification d'images de prunes africaines avec application desktop
Ce dépôt contient une solution end-to-end pour la classification automatique de prunes africaines, depuis le prétraitement des images jusqu'au déploiement dans une application desktop intuitive (via Custom Tkinter). Le projet a été développé lors du hackathon JCIA et s'appuie sur une architecture robuste de Machine Learning et Deep Learning.

📌 Fonctionnalités clés
1. Pipeline de traitement des données
Chargement des données :

Lecture à partir d'un fichier pickle (image_data_with_Images.pkl) contenant images, étiquettes (unaffected, unripe, defective), et types de défauts (bruised, cracked, etc.).

Prétraitement avancé :

Redimensionnement (512x512), suppression de l'arrière-plan (rembg), et augmentation des données (Albumentations) pour équilibrer les classes.

Création de datasets :

Division stratifiée en ensembles d'entraînement (70%), validation (15%), et test (15%).

2. Modèles de classification
Deux modèles fine-tunés :

global_model : Classe les prunes en saines, immatures, ou défectueuses.

defect_model : Identifie le type de défaut (meurtries, fissurées, pourries, tachetées).

Architecture flexible :

Modèles pré-entraînés (ResNet18, ResNet50, VGG16, etc.) avec couches fully connected personnalisées (CustomFC).

Optimisation via Adam/SGD et suivi des métriques (précision, rappel, F1-score).

3. Application Desktop (Custom Tkinter)
Interface utilisateur moderne :

Thèmes personnalisables, boutons interactifs, et visualisation des résultats.

Fonctionnalités :

Chargement d'images (drag & drop ou sélection manuelle).

Prédiction en temps réel avec affichage des scores de confiance.

Export des résultats (logs, images annotées).

🛠 Technologies utilisées
Backend :

Python, PyTorch, OpenCV, Albumentations, rembg.

Frontend (App Desktop) :

Custom Tkinter pour une interface graphique responsive et esthétique.

Gestion de projet :

Jupyter Notebook, Git/GitHub, Pipenv (gestion des dépendances).

🚀 Workflow complet
Préparation des données → 2. Entraînement des modèles → 3. Évaluation → 4. Déploiement dans l'app desktop.

Scénario de test en production :

Les modèles sauvegardés (global_model.pth, defect_model.pth) sont intégrés à l'application pour des prédictions locales sans serveur.

📊 Résultats et livrables
Rapports de classification (précision > 90% sur les classes majeures).

Courbes d'apprentissage (visualisation de la loss et de l'accuracy).

Application desktop prête à l'emploi pour les agriculteurs/inspecteurs qualité.

*Projet réalisé dans le cadre du hackathon de la journe camerounaise de l'intelligence artificielle .

✨ Pourquoi ce projet ?
Solution clé en main : Combine une pipeline ML robuste et une interface accessible pour l'industrie agricole.

Innovation : Utilisation de Custom Tkinter pour démocratiser l'IA hors des environnements cloud.

Cette description met en valeur à la fois la rigueur technique (via les détails du workflow documenté) et l'aspect utilisateur final (app desktop). Vous pouvez y ajouter des captures d'écran de l'interface ou des graphiques pour renforcer l'impact ! 🌟
