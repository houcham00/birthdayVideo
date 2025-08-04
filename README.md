# Vidéo d'anniversaire animée express - Landing Page

Une landing page responsive pour un service de vidéos d'anniversaire personnalisées à 10 000 FCFA.

## Fonctionnalités

✅ **3 sections principales** :
- Hero avec prix et CTAs
- Aperçu des templates avec modales vidéo
- Processus de paiement et formulaire

✅ **Design responsive** :
- Mobile-first layout
- 2 colonnes max sur smartphone
- Boutons et textes optimisés mobile

✅ **Intégrations** :
- Moneroo pour le paiement
- Typeform pour la collecte d'informations
- Canva pour les aperçus vidéo

## Configuration

### 1. Paiement Moneroo

Remplacez dans le fichier `index.html` :
```javascript
const MONEROO_PUBLIC_KEY = 'YOUR_MONEROO_PUBLIC_KEY';
```

### 2. Formulaire Typeform

Remplacez dans le fichier `index.html` :
```javascript
const TYPEFORM_URL = 'https://form.typeform.com/to/YOUR_TYPEFORM_ID';
```

### 3. Vidéos Canva

Remplacez les URLs dans l'objet `templateVideos` :
```javascript
const templateVideos = {
    template1: 'https://player.canva.com/YOUR_VIDEO_ID_1',
    template2: 'https://player.canva.com/YOUR_VIDEO_ID_2',
    template3: 'https://player.canva.com/YOUR_VIDEO_ID_3',
    template4: 'https://player.canva.com/YOUR_VIDEO_ID_4'
};
```

## Structure des fichiers

```
birthdayVideo/
├── index.html          # Page principale (< 300 lignes)
├── README.md           # Ce fichier
└── assets/             # Dossier pour les images (optionnel)
```

## Utilisation

1. Ouvrez `index.html` dans un navigateur
2. La page fonctionne sans serveur (fichier statique)
3. Pour production, configurez les clés API réelles

## Optimisations

- **Performance** : CSS inline, JS minimal (< 5KB)
- **SEO** : HTML sémantique, meta tags appropriés
- **Accessibilité** : Alt texts, boutons avec labels clairs
- **Mobile** : Design mobile-first, touch-friendly

## Workflow utilisateur

1. **Landing** → Utilisateur voit le prix et les options
2. **Templates** → Aperçu des vidéos disponibles
3. **Choix** → Sélection template ou sur-mesure
4. **Paiement** → Moneroo/Axa Zara
5. **Formulaire** → Typeform pour les détails
6. **Livraison** → Vidéo personnalisée

## Support

- Testé sur Chrome, Firefox, Safari
- Compatible iOS/Android
- Fonctionne sans JavaScript (dégradation gracieuse)
