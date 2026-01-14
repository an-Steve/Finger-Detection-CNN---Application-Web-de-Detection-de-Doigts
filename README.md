## Finger Detection CNN - Application Web de Détection de Doigts
# Réalisé par ANTON NELCON Steve -

<img width="1832" height="860" alt="image" src="https://github.com/user-attachments/assets/a69a39cf-63db-46f2-9b86-4e4f65e94604" />

<img width="1832" height="694" alt="image" src="https://github.com/user-attachments/assets/66a57b70-a2db-440b-bfa1-904c8715cece" />

# Fonctionnalités

    → Détection Précise : Reconnaît 0 à 5 doigts avec une haute précision

    → Multiples Sources : Importation d'images ou capture via webcam

    → Temps Réel : Analyse instantanée avec traitement client-side

    → Visualisations Détaillées : Probabilités par classe et indicateurs de confiance

    → Interface Moderne : Design responsive avec animations fluides

    → Vie Privée : Traitement 100% local, aucune donnée envoyée au serveur

# Capture d'écran
<img width="1428" height="667" alt="image" src="https://github.com/user-attachments/assets/a9d7e288-3fe6-4d5f-8eba-0f96ad8a3e20" />

 # Technologies Utilisées

    → TensorFlow.js - Machine learning dans le navigateur

    → HTML5/CSS3 - Interface utilisateur moderne

    → JavaScript ES6 - Logique applicative

    → Canvas API - Traitement d'images

# Architecture du Modèle


Entrée: 64×64×3 (RGB)
    ↓
Conv2D(32, 3×3) + BatchNorm + ReLU
    ↓
MaxPooling(2×2) + Dropout(25%)
    ↓
Conv2D(64, 3×3) + BatchNorm + ReLU
    ↓
MaxPooling(2×2) + Dropout(25%)
    ↓
Conv2D(128, 3×3) + BatchNorm + ReLU
    ↓
MaxPooling(2×2) + Dropout(25%)
    ↓
Flatten
    ↓
Dense(256) + Dropout(50%)
    ↓
Dense(128) + Dropout(30%)
    ↓
Dense(6) + Softmax → Sortie: 0-5 doigts


🎯 Meilleures Pratiques pour la Détection
✅ Conditions optimales :

    Main ouverte avec paume visible

    Doigts bien séparés

    Éclairage uniforme

    Fond simple et contrasté

    Distance modérée de la caméra

❌ À éviter :

    Mains partiellement coupées

    Fortes ombres

    Arrière-plan complexe

    Doigts superposés

    Faible luminosité

    MediaDevices API - Accès à la webcam

''
            Merci
