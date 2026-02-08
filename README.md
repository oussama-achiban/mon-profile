"# 👨‍💻 Oussama Achiban - Portfolio Professionnel

Un portfolio personnel moderne et réactif créé avec **Next.js**, **React**, **TypeScript** et **Tailwind CSS**. Conçu pour présenter mes projets, certifications, compétences et expériences.

---

## ✨ Caractéristiques

### 🎯 Sections Principales
- **À propos** - Présentation professionnelle et motivations
- **Éducation** - Formation académique (Master 1 ISI, Licence, DEUG, BAC)
- **Compétences** - Programmation, développement web, data science/ML, langues
- **Projets** - 9 projets GitHub réels avec descriptions et technologies
- **Certifications** - 12 certifications DataCamp avec accès aux PDFs
- **Contact** - Formulaire de contact et informations de contact

### 🔧 Fonctionnalités Techniques
- ✅ **Responsive Design** - Adapté à tous les appareils (mobile, tablette, desktop)
- ✅ **Mode Sombre/Clair** - Thème commutable avec persistance
- ✅ **Navigation Fluide** - Scroll tracking et navigation intelligente
- ✅ **CV Téléchargeable** - Format HTML/CSS optimisé pour impression PDF
- ✅ **Intégration GitHub** - Projets chargés depuis GitHub API
- ✅ **Formulaire de Contact** - Contact direct via le site
- ✅ **Animations** - Transitions et effets visuels fluides
- ✅ **Accessibilité** - Structure sémantique et support clavier

---

## 🛠️ Stack Technologique

### Frontend
- **Framework**: Next.js 13+ (App Router)
- **Langage**: TypeScript
- **UI Library**: React 18
- **Styling**: Tailwind CSS 3
- **Components**: shadcn/ui (Button, Card, Badge, Input, Textarea, etc.)
- **Icons**: Lucide React + FontAwesome

### Outils & Services
- **Package Manager**: pnpm
- **Version Control**: Git & GitHub
- **Hosting**: Netlify (déploiement continu)
- **API**: GitHub REST API (données des projets)

### Documents
- **CV HTML**: Format web optimisé pour impression PDF
- **CV LaTeX**: Document professionnel (avec moderncv)

---

## 📦 Installation & Configuration

### Prérequis
- **Node.js** ≥ 18 (recommandé: v20)
- **pnpm** ≥ 8 (ou npm/yarn)
- **Git**

### Étapes d'Installation

```bash
# 1. Cloner le repository
git clone https://github.com/oussama-achiban/oussama-achiban-resume.git
cd oussama-achiban-resume

# 2. Installer les dépendances
pnpm install

# 3. Lancer le serveur de développement
pnpm dev

# 4. Ouvrir dans le navigateur
# Accéder à: http://localhost:3000
```

### Variables d'Environnement
Aucune variable d'environnement requise. Les données des projets sont chargées automatiquement via GitHub API.

---

## 🚀 Utilisation

### Navigation
- Cliquez sur les éléments du menu pour naviguer vers les sections
- La navigation suit automatiquement votre scroll
- Les liens mènent vers les projets GitHub et les certifications PDF

### Télécharger le CV
- Cliquez sur **"Télécharger CV"** dans la navigation
- Le CV s'ouvre dans un nouvel onglet (format HTML)
- Utilisez **Ctrl+P** (ou Cmd+P sur Mac) pour imprimer en PDF

### Formulaire de Contact
- Remplissez votre nom, email et message
- Cliquez sur "Envoyer"
- Confirmation visuelle du succès de l'envoi

### Consulter les Certifications
- Section "Certifications" affiche toutes les 12 certifications DataCamp
- Cliquez sur une certification pour voir le PDF correspondant
- Les certificats sont stockés localement pour un chargement rapide

---

## 📁 Structure du Projet

```
oussama-achiban-resume/
├── app/
│   ├── layout.tsx          # Layout principal avec App Router
│   ├── page.tsx            # Composant portfolio (section à section)
│   └── globals.css         # Styles globaux
├── components/
│   ├── theme-provider.tsx  # Gestion du thème sombre/clair
│   └── ui/                 # Composants shadcn/ui (50+)
├── hooks/
│   ├── use-mobile.ts       # Hook pour détecter appareils mobiles
│   └── use-toast.ts        # Hook pour notifications toast
├── lib/
│   └── utils.ts            # Utilitaires TypeScript/Tailwind
├── public/
│   ├── image.png           # Logo du site
│   ├── profil.png          # Photo de profil
│   ├── cv.html             # CV HTML téléchargeable
│   ├── cv.tex              # CV LaTeX (moderncv)
│   └── Certificates_pdf/   # 12 certificats DataCamp (PDFs)
├── styles/
│   └── globals.css         # Variables CSS et styles globaux
├── package.json            # Dépendances et scripts
├── tsconfig.json           # Configuration TypeScript
├── tailwind.config.ts      # Configuration Tailwind CSS
├── next.config.mjs         # Configuration Next.js
└── README.md               # Ce fichier
```

### Fichiers Clés

**`app/page.tsx`** (767 lignes)
- Composant principal du portfolio
- État: useState pour menu, section active, formulaire
- Contient: 9 projets GitHub, 12 certifications DataCamp, toutes les sections
- Helper: `formatTitleFromFilename()` pour noms de certificats

**`public/cv.html`**
- CV professionnel en HTML/CSS
- Imprimable en PDF via navigateur
- Responsive et print-friendly

**`tailwind.config.ts`**
- Palette: Émeraude (primaire), Ardoise (secondaire)
- Mode sombre activé par défaut
- Variables CSS pour cohérence

---

## 📊 Projets GitHub Intégrés

1. **MonProjetFinEtud** - Application diagnostic médical (PHP/SQL)
2. **Mozeria** - Gestion de restaurants (Python)
3. **Course Summary and Exercises ML** - Ressources d'apprentissage (Python/ML)
4. **Mon Profile** - Portfolio personnel (TypeScript)
5. **Manipulation des Pointeurs** - Exercices C (C)
6. **Projet Gestion Étudiants** - Gestion académique (C)
7. **SpaceHTML** - Conception web créative (CSS/HTML)
8. **TP Programmation C** - Travaux pratiques (C)
9. **PHP TP1** - Exercices PHP (PHP/HTML)

Les données sont automatiquement synchronisées via GitHub API.

---

## 🎓 Certifications

12 certifications DataCamp complétées:
- **Python**: Introduction to Python, Intermediate Python, Advanced Python, Python Data Science, Data Science 101
- **Data Science**: Introduction to Data Science, Advanced Data Science Techniques
- **Deep Learning**: Deep Learning with TensorFlow, Neural Networks Advanced
- **Java**: Java Fundamentals
- **Machine Learning**: Machine Learning Fundamentals

Tous les certificats en PDF sont accessibles via le site.

---

## 🎨 Personnalisation

### Couleurs
Modifiez `tailwind.config.ts` pour changer la palette:
```typescript
// Présenté par défaut: emerald-400 (primaire), slate (secondaire)
colors: {
  emerald: '#10b981',
  slate: '#475569'
}
```

### Ajouter des Projets
Mettez à jour le tableau `projects` dans `app/page.tsx`:
```typescript
const projects = [
  {
    title: "Nom du Projet",
    description: "Description brève",
    technologies: ["Tech1", "Tech2"],
    date: "YYYY-MM-DD",
    github: "https://github.com/...",
    featured: true
  },
  // ...
]
```

### Ajouter des Certifications
Ajoutez des entrées au tableau `certificates` dans `app/page.tsx`:
```typescript
const certificates = [
  {
    title: "Titre Certifi",
    issuer: "Organisme",
    date: "2024",
    icon: "python", // ou autre
    pdfUrl: "/Certificates_pdf/nomfichier.pdf"
  },
  // ...
]
```

---

## 🚢 Déploiement

### Netlify (Recommandé)
```bash
# Connecter votre GitHub à Netlify
# Configuration automatique pour Next.js
# Chaque push déclenche un déploiement
```

### Autres Hébergeurs
Compatible avec Vercel, GitHub Pages, AWS, etc.
Assurez-vous que Node.js ≥ 18 est supporté.

---

## 📝 Scripts npm/pnpm

```bash
# Développement
pnpm dev          # Lancer serveur (http://localhost:3000)

# Build
pnpm build        # Compiler pour production

# Production
pnpm start        # Lancer serveur production

# Validation
pnpm lint         # Vérifier ESLint
```

---

## 🔒 Sécurité

- Aucune clé API sensible stockée côté client
- Formulaire de contact validé côté serveur
- Pas de base de données exposée
- GitHub API utilisée en lecture seule
- CORS configuré correctement

---

## 🐛 Dépannage

### CV ne s'ouvre pas
- Vérifier que `/public/cv.html` existe
- Nettoyer le cache du navigateur (Ctrl+Shift+Delete)

### Les projets ne s'affichent pas
- Vérifier la connexion internet
- GitHub API peut avoir des limitations de débit (60 req/h non authentifiée)
- Consulter: https://api.github.com/users/oussama-achiban/repos

### Certificats PDF vides
- Vérifier que les fichiers PDF existent dans `/public/Certificates_pdf/`
- Vérifier les chemins URL dans le tableau `certificates`

### Page ne répond pas
- Vider le cache: `rm -rf .next`
- Réinstaller: `pnpm install`
- Relancer: `pnpm dev`

---

## 📞 Contact

**Email**: oussama.achiban@example.com  
**GitHub**: [github.com/oussama-achiban](https://github.com/oussama-achiban)  
**LinkedIn**: [linkedin.com/in/oussama-achiban](https://linkedin.com/in/oussama-achiban)  
**Site Web**: [oussama-achiban-resume.netlify.app](https://oussama-achiban-resume.netlify.app)

---

## 📄 Licence

Ce projet est distribué sous la licence **MIT**. Voir [LICENSE](LICENSE) pour détails.

---

## 🙏 Remerciements

- **Next.js** - Framework React moderne
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - Composants réutilisables
- **Lucide React** - Icônes vectorielles
- **GitHub API** - Données des projets

---

**Dernière mise à jour**: Janvier 2025  
**Créé par**: Oussama Achiban  
**Version**: 1.0.0

" 
#   p o r t f l i o  
 