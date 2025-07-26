# 🎨 Générateur de Cartes - Communauté USD

Un générateur de cartes personnalisées pour les membres de la communauté USD (Innovation & Tech). Cette application web permet de créer et télécharger des cartes de participation aux événements avec un design moderne et professionnel.

## ✨ Fonctionnalités

### 🖊️ Personnalisation
- **Informations personnelles** : Nom, rôle, entreprise
- **Détails de l'événement** : Date, lieu, type de session
- **Photo de profil** : Upload d'image avec redimensionnement automatique
- **Message personnalisé** : Texte libre pour personnaliser la carte
- **Numéro de cohorte** : Système de numérotation des groupes

### 🎨 Design
- **Interface moderne** : Design responsive avec dégradés et animations
- **Charte graphique cohérente** : Variables CSS personnalisables
- **Preview en temps réel** : Aperçu instantané des modifications
- **Layout adaptatif** : Compatible desktop et mobile

### 📥 Export
- **Téléchargement PNG** : Carte haute qualité (2x scale)
- **Format desktop forcé** : Layout optimal même sur mobile
- **Nom de fichier intelligent** : `carte-usd-[nom]-cohorte[X].png`
- **Bordures supprimées** : Rendu propre sans arrondi

## 🚀 Installation

### Prérequis
- Navigateur web moderne (Chrome, Firefox, Safari, Edge)
- Connexion internet (pour les polices et icônes)

### Utilisation
1. Ouvrez le fichier `index.html` dans votre navigateur
2. Remplissez le formulaire avec vos informations
3. Ajoutez votre photo (optionnel)
4. Personnalisez le message si souhaité
5. Cliquez sur "Télécharger la carte (PNG)"

## 📁 Structure du projet

```
générateur-cartes-usd/
├── index.html          # Application principale
├── README.md          # Documentation
└── image/             # Dossier pour les assets (optionnel)
    ├── logo.png       # Logo de fond (watermark)
    └── logo-complete.png  # Logo principal
```

## 🎨 Personnalisation

### Variables CSS
Modifiez les couleurs dans `:root` :

```css
:root {
    --primary-color: #33e08d;      /* Vert principal */
    --secondary-color: #F1C40F;    /* Jaune accent */
    --accent-color: #E67E22;       /* Orange boutons */
    --gradient-start: #33e08d;     /* Début dégradé */
    --gradient-end: #022132;       /* Fin dégradé */
}
```

### Configuration JavaScript
Personnalisez les textes dans l'objet `CONFIG` :

```javascript
const CONFIG = {
    communityName: "COMMUNAUTÉ USD",
    subtitle: "Construire l'avenir numérique ensemble",
    logoText: "LOGO USD",
    defaultMessage: "Membre actif de la communauté USD"
};
```

## 🛠️ Technologies utilisées

- **HTML5** : Structure sémantique
- **CSS3** : Animations, Grid, Flexbox, Variables CSS
- **JavaScript ES6+** : Logique interactive, gestion des événements
- **html2canvas** : Capture et export PNG
- **Font Awesome** : Icônes des réseaux sociaux
- **Google Fonts** : Polices Poppins et Pacifico

## 📱 Responsive Design

### Desktop (> 768px)
- Layout en grille 2 colonnes
- Formulaire à gauche, aperçu à droite
- Aperçu fixe (sticky)

### Mobile (≤ 768px)
- Layout vertical empilé
- Formulaire puis aperçu
- Adaptation des éléments de la carte

### Export
- **Toujours en format desktop** pour l'image exportée
- Largeur fixe de 600px pour un rendu optimal
- Layout horizontal forcé même sur mobile

## ⚡ Performances

### Optimisations
- **Lazy loading** des polices externes
- **Debouncing** des mises à jour de preview
- **Compression PNG** avec qualité maximale
- **Cache des ressources** externes via CDN

### Compatibilité
- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

## 🔧 Dépannage

### Problèmes courants

**Le téléchargement ne fonctionne pas**
- Vérifiez que JavaScript est activé
- Testez dans un autre navigateur
- Vérifiez la console pour les erreurs

**Les polices ne s'affichent pas**
- Vérifiez votre connexion internet
- Les polices Google Fonts doivent être accessibles

**La photo ne s'affiche pas**
- Formats supportés : JPG, PNG, GIF, WebP
- Taille recommandée : < 5MB
- Vérifiez que le fichier n'est pas corrompu

**L'export a une mauvaise qualité**
- L'export utilise un scale 2x automatiquement
- Assurez-vous que la photo source est en bonne résolution

## 🎯 Utilisation recommandée

### Photos de profil
- **Format** : Carré (1:1) pour un meilleur rendu
- **Résolution** : Minimum 300x300px
- **Type** : Photo professionnelle, visage visible
- **Éclairage** : Bonne luminosité, arrière-plan neutre

### Informations
- **Nom** : Prénom et nom complets
- **Rôle** : Poste actuel ou domaine d'expertise
- **Entreprise** : Nom complet de l'organisation
- **Lieu** : Format "Ville, Pays" recommandé

## 📄 Licence

Ce projet est libre d'utilisation pour les membres de la communauté USD. 

---

**Créé avec ❤️ pour la communauté USD Innovation & Tech**

Pour toute question ou suggestion d'amélioration, n'hésitez pas à contribuer ou contacter l'équipe de développement.# usds-event-flyers-generator
