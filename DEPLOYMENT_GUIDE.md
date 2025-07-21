# 🚀 Guide de Déploiement Vercel - Pomme Croquer

## Étape 1: Préparer le projet

✅ **Déjà fait :**
- Configuration Next.js ✓
- Fichier vercel.json ✓
- Fichiers PWA (manifest.json) ✓
- Optimisations SEO ✓

## Étape 2: Créer un compte GitHub (si nécessaire)

1. Allez sur [github.com](https://github.com)
2. Cliquez sur "Sign up" si vous n'avez pas de compte
3. Suivez les instructions d'inscription

## Étape 3: Créer un repository GitHub

1. Connectez-vous à GitHub
2. Cliquez sur le bouton vert "New" ou "+" → "New repository"
3. Nommez votre repository : `pomme-croquer`
4. Ajoutez une description : "Gestionnaire iOS complet - Alternative 3uTools"
5. Laissez en "Public" (gratuit)
6. ✅ Cochez "Add a README file"
7. Cliquez sur "Create repository"

## Étape 4: Uploader votre code

### Option A: Via l'interface GitHub (plus simple)
1. Dans votre nouveau repository, cliquez sur "uploading an existing file"
2. Glissez-déposez tous vos fichiers du projet SAUF :
   - node_modules/
   - .next/
   - .env.local
3. Écrivez un message de commit : "Initial commit - Pomme Croquer"
4. Cliquez sur "Commit changes"

### Option B: Via Git (si vous avez Git installé)
```bash
# Dans le dossier de votre projet
git init
git add .
git commit -m "Initial commit - Pomme Croquer"
git branch -M main
git remote add origin https://github.com/VOTRE-USERNAME/pomme-croquer.git
git push -u origin main
```

## Étape 5: Déployer sur Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Cliquez sur "Sign up" puis "Continue with GitHub"
3. Autorisez Vercel à accéder à votre GitHub
4. Cliquez sur "Import Project"
5. Trouvez votre repository "pomme-croquer" et cliquez "Import"
6. **Configuration du projet :**
   - Project Name: `pomme-croquer`
   - Framework Preset: `Next.js` (détecté automatiquement)
   - Root Directory: `./` (par défaut)
   - Build Command: `npm run build` (par défaut)
   - Output Directory: `.next` (par défaut)
7. Cliquez sur "Deploy"

## Étape 6: Attendre le déploiement

⏳ Vercel va :
1. Installer les dépendances
2. Construire l'application
3. Déployer sur leur CDN global
4. Vous donner une URL publique

## Étape 7: Votre URL publique

🎉 **Votre application sera disponible à :**
- URL principale : `https://pomme-croquer.vercel.app`
- URL alternative : `https://pomme-croquer-VOTRE-USERNAME.vercel.app`

## Étape 8: Configuration du domaine personnalisé (optionnel)

Si vous voulez `pomme-croquer.com` :
1. Dans Vercel, allez dans Settings → Domains
2. Ajoutez votre domaine personnalisé
3. Configurez les DNS selon les instructions

## Étape 9: Mises à jour automatiques

✨ **Avantage :** Chaque fois que vous modifiez votre code sur GitHub, Vercel redéploie automatiquement !

## 🔧 Dépannage

### Erreur de build ?
- Vérifiez que tous les fichiers sont uploadés
- Assurez-vous que package.json est présent
- Consultez les logs de build dans Vercel

### Problème d'icônes PWA ?
- Les icônes seront générées automatiquement
- Ou ajoutez vos propres icônes dans le dossier `public/`

## 📱 Test de l'installation PWA

Une fois déployé :
1. Ouvrez l'URL dans Chrome/Edge
2. Cherchez l'icône d'installation dans la barre d'adresse
3. Installez l'application sur votre ordinateur !

---

**🎯 Résultat final :** Votre application "Pomme Croquer" sera accessible mondialement via une URL publique et installable sur tous les ordinateurs !
