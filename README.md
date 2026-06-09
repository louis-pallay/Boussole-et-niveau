# Boussole-et-niveau
# SAÉ 204 — Système Embarqué : Boussole et Niveau Numérique

## 📝 Description du projet
Ce projet a été réalisé dans le cadre de la SAÉ 204 du BUT Réseaux et Télécommunications (IUT de Marseille, site Luminy). 

L'objectif est de concevoir et de programmer une application embarquée sur un module **M5Stack Grey** faisant office de boussole électronique et de niveau à bulle numérique en temps réel. Le système exploite la centrale inertielle (IMU) intégrée pour mesurer précisément l'orientation et l'inclinaison spatiale.

### 🎯 Fonctionnalités principales
* **Mode Boussole :** Calcul et affichage du cap (en degrés) par rapport au Nord magnétique, combinant les données de l'accéléromètre et du magnétomètre.
* **Mode Niveau à bulle :** Visualisation de l'inclinaison sur les axes X et Y pour vérifier la planéité d'une surface, simulant graphiquement un niveau à bulle traditionnel.
* **Interface Utilisateur (UI) :** Exploitation de l'écran LCD et des **boutons physiques du M5Stack (A, B, C)** pour basculer facilement entre les différents modes d'affichage ou calibrer les capteurs.

---

## 🛠️ Spécifications Techniques

### Matériel utilisé
* **Microcontrôleur :** M5Stack Grey (basé sur un ESP32, 16MB Flash, écran LCD 240x320).
* **Capteurs internes :** Centrale inertielle IMU 9-axes (MPU6886 + BMM150 pour la gestion du magnétomètre).

### Environnement de développement et Langages
* **Langage :** C++ (Framework Arduino) / MicroPython *(conserve uniquement ton langage)*
* **Outils :** Git & GitHub pour le versioning

---

## 🚀 Algorithmes & Traitement du signal
Le programme intègre une logique de traitement pour assurer la précision des instruments :
* **Calcul trigonométrique :** Utilisation des fonctions mathématiques pour convertir les données brutes des axes de l'IMU en angles exploitables (calcul du cap et de la matrice d'inclinaison).
* **Optimisation de l'affichage :** Gestion du rafraîchissement de l'écran pour éviter les scintillements lors des déplacements rapides de la bulle ou de l'aiguille.

---

## 👥 Membres de l'équipe
* **Louis PALLAY**
* **Alex Margherio**
* **Nacim Djemel**
