# 📁 Guide pour Uploader les Fichiers sur GitHub

## 🎯 Méthode Simple : Glisser-Déposer sur GitHub

### Étape 1: Préparer vos fichiers
Vous devez uploader TOUS ces fichiers et dossiers :

**📄 Fichiers à la racine :**
- `.gitignore`
- `components.json`
- `DEPLOYMENT_GUIDE.md`
- `eslint.config.mjs`
- `next.config.ts`
- `package-lock.json`
- `package.json` ⭐ (TRÈS IMPORTANT)
- `postcss.config.mjs`
- `README.md`
- `tsconfig.json`
- `vercel.json`

**📁 Dossiers complets :**
- `public/` (avec tous ses fichiers)
- `src/` (avec tous ses sous-dossiers)

### Étape 2: Créer le repository GitHub

1. Allez sur [github.com](https://github.com)
2. Connectez-vous à votre compte
3. Cliquez sur le bouton vert **"New"** ou **"+"** → **"New repository"**
4. Remplissez :
   - Repository name: `pomme-croquer`
   - Description: `Gestionnaire iOS complet - Alternative 3uTools`
   - ✅ Cochez **"Add a README file"**
   - Laissez en **"Public"**
5. Cliquez sur **"Create repository"**

### Étape 3: Uploader les fichiers (Méthode Glisser-Déposer)

#### Option A: Upload par Glisser-Déposer (RECOMMANDÉ)

1. **Dans votre nouveau repository GitHub**, cliquez sur **"uploading an existing file"**

2. **Préparez vos fichiers :**
   - Ouvrez l'explorateur de fichiers de votre ordinateur
   - Naviguez vers votre dossier projet "Pomme Croquer"
   - Sélectionnez TOUS les fichiers et dossiers SAUF :
     - ❌ `node_modules/` (ne pas inclure)
     - ❌ `.next/` (ne pas inclure)
     - ❌ `.env.local` (ne pas inclure)

3. **Glissez-déposez :**
   - Sélectionnez tous les fichiers/dossiers autorisés
   - Glissez-les dans la zone de drop de GitHub
   - Attendez que tous les fichiers se chargent

4. **Commit les changements :**
   - Message de commit : `Initial commit - Pomme Croquer`
   - Cliquez sur **"Commit changes"**

#### Option B: Upload dossier par dossier (si Option A ne marche pas)

1. **Uploadez d'abord les fichiers racine :**
   - Glissez tous les fichiers `.json`, `.md`, `.ts`, etc.
   - Commit avec message : "Add root files"

2. **Uploadez le dossier public/ :**
   - Cliquez sur "Add file" → "Upload files"
   - Glissez tout le contenu du dossier `public/`
   - Commit avec message : "Add public folder"

3. **Uploadez le dossier src/ :**
   - Répétez pour le dossier `src/` complet
   - Commit avec message : "Add src folder"

### Étape 4: Vérifier l'upload

Votre repository doit contenir :
```
pomme-croquer/
├── .gitignore
├── components.json
├── DEPLOYMENT_GUIDE.md
├── eslint.config.mjs
├── next.config.ts
├── package.json ⭐
├── package-lock.json
├── postcss.config.mjs
├── README.md
├── tsconfig.json
├── vercel.json
├── public/
│   ├── manifest.json
│   ├── robots.txt
│   ├── sitemap.xml
│   └── (autres fichiers)
└── src/
    ├── app/
    │   ├── globals.css
    │   ├── layout.tsx
    │   └── page.tsx
    ├── components/
    │   ├── AppleLogo.tsx
    │   ├── DownloadButton.tsx
    │   ├── InstallationGuide.tsx
    │   ├── InstallPrompt.tsx
    │   └── ui/ (tous les composants)
    ├── hooks/
    └── lib/
```

### 🚨 Points Importants :

1. **NE PAS inclure :**
   - ❌ `node_modules/` (trop lourd, sera recréé)
   - ❌ `.next/` (fichiers de build temporaires)
   - ❌ `.env.local` (fichiers secrets)

2. **ABSOLUMENT inclure :**
   - ✅ `package.json` (liste des dépendances)
   - ✅ `package-lock.json` (versions exactes)
   - ✅ Tous les fichiers `.tsx`, `.ts`, `.css`
   - ✅ Dossier `public/` complet
   - ✅ Dossier `src/` complet

### Étape 5: Après l'upload réussi

Une fois tous vos fichiers uploadés :
1. Votre repository GitHub est prêt ! 🎉
2. Passez à l'étape suivante : **Déploiement sur Vercel**
3. Suivez le guide `DEPLOYMENT_GUIDE.md`

---

## 🆘 En cas de problème :

**Erreur "File too large" ?**
- Vérifiez que vous n'uploadez pas `node_modules/`
- Uploadez par petits groupes de fichiers

**Certains fichiers ne s'uploadent pas ?**
- Essayez l'Option B (dossier par dossier)
- Vérifiez votre connexion internet

**Repository vide après upload ?**
- Assurez-vous d'avoir cliqué sur "Commit changes"
- Rafraîchissez la page GitHub
