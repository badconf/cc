# Respiration 365

Une interface web simple et élégante pour pratiquer la respiration 365, technique de cohérence cardiaque basée sur la synchronisation du rythme cardiaque avec la respiration.

## 📖 Description

Cette page propose un guide visuel interactif pour la pratique de la cohérence cardiaque selon le protocole standard : **5 secondes d'inspiration, 5 secondes d'expiration**, soit 6 respirations par minute.

L'interface présente une courbe sinusoïdale animée avec un point de repère qui monte et descend de façon fluide. L'utilisateur suit simplement ce mouvement :
- **Montée du point** = **Inspiration**
- **Descente du point** = **Expiration**

## ✨ Fonctionnalités

- **Interface minimaliste** : Design épuré centré sur l'essentiel
- **Animation fluide** : Courbe sinusoïdale avec point de repère animé
- **Indicateur textuel** : Affichage "INSPIREZ" / "EXPIREZ" avec codes couleur
- **Responsive** : Adaptation automatique à tous les écrans (desktop, tablette, mobile)
- **Effets visuels** : Dégradé de fond, transparences et effet de flou (glassmorphism)
- **Pulsation** : Effet de pulsation sur le point de repère
- **Hors ligne** : Fonctionne sans connexion internet une fois chargée

## 🎯 Bénéfices de la cohérence cardiaque

La cohérence cardiaque est une technique de respiration qui :
- Réduit le stress et l'anxiété
- Améliore la concentration et la clarté mentale
- Régule la variabilité du rythme cardiaque
- Favorise un meilleur sommeil
- Renforce le système immunitaire

Ces bénéfices restent à nuancer (voir l'article de l'[INSERM](https://presse.inserm.fr/canal-detox/la-coherence-cardiaque-une-technique-pour-ameliorer-sa-sante-vraiment/)).

## 🚀 Utilisation

### En ligne
Accédez directement à l'interface via votre navigateur : [URL de votre choix]

### En local
1. Clonez ou téléchargez le repository
2. Ouvrez le fichier `365.html` dans votre navigateur
3. Commencez votre session de cohérence cardiaque

### Instructions d'utilisation
1. Installez-vous confortablement dans un environnement calme
2. Regardez le point sur la courbe sinusoïdale
3. **Inspirez** lorsque le point monte (indication verte "INSPIREZ")
4. **Expirez** lorsque le point descend (indication bleue "EXPIREZ")
5. Continuez pendant 5 minutes minimum (durée recommandée)

## 🛠 Aspects techniques

### Technologies utilisées
- **HTML5** : Structure sémantique et métadonnées
- **CSS3** : Design moderne avec dégradés, transparences et responsive design
- **JavaScript ES6+** : Animation canvas et logique de l'application
- **Canvas API** : Rendu graphique de la courbe sinusoïdale

### Architecture du code

#### Structure HTML
- Container principal responsive
- Canvas pour l'animation graphique  
- Indicateurs textuels de phase respiratoire
- Métadonnées pour le SEO et l'accessibilité

#### Logique JavaScript
```javascript
class CoherenceCardiaque {
    setupCanvas()      // Configuration responsive du canvas
    initializeVariables() // Variables de timing et d'animation
    drawAxes()         // Axes de repère
    drawSineCurve()    // Courbe sinusoïdale animée
    drawBreathingPoint() // Point de repère avec pulsation
    animate()          // Boucle d'animation principal
}
```

#### Paramètres de respiration
- **Cycle complet** : 10 secondes (5s inspiration + 5s expiration)
- **Fréquence** : 6 respirations par minute
- **Fonction mathématique** : Sinusoïde avec offset temporel
- **Animation** : 60 FPS via `requestAnimationFrame`

### Responsive design
- Adaptation automatique des dimensions du canvas
- Points de rupture pour mobile/tablette/desktop
- Redimensionnement dynamique lors du changement d'orientation

### Optimisations
- Rendu canvas optimisé avec limitation des calculs
- Gestion des événements de redimensionnement
- Code modulaire et orienté objet
- Pas de dépendances externes

## 📱 Compatibilité

- **Navigateurs modernes** : Chrome, Firefox, Safari, Edge
- **Appareils** : Desktop, tablette, smartphone
- **Systèmes** : Windows, macOS, Linux, iOS, Android
- **PWA Ready** : Métadonnées pour installation en tant qu'application

## 📄 Licence

Ce projet est distribué sous licence **BSD-3-Clause**. Voir le fichier `LICENSE` pour plus de détails.

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour proposer des améliorations :

1. Forkez le projet
2. Créez une branche pour votre fonctionnalité (`git checkout -b feature/nouvelle-fonctionnalite`)
3. Committez vos modifications (`git commit -am 'Ajout d'une nouvelle fonctionnalité'`)
4. Poussez vers la branche (`git push origin feature/nouvelle-fonctionnalite`)
5. Ouvrez une Pull Request

## 💡 Améliorations possibles

- [ ] Choix de durée de session (3, 5, 10 minutes)
- [ ] Sons ou musique d'ambiance optionnels
- [ ] Différents thèmes visuels
- [ ] Sauvegarde des statistiques de pratique
- [ ] Mode sombre/clair
- [ ] Vibrations pour les appareils mobiles
- [ ] Export en PWA complète

## 📧 Contact

Pour toute question ou suggestion concernant cette application, n'hésitez pas à ouvrir une issue sur ce repository.

---

*Prenez soin de votre bien-être. Respirez.*
