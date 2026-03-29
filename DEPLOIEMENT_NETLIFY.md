# 🚀 Déploiement sur Netlify

## Étape 1: Préparer les fichiers

Assurez-vous que votre repository GitHub contient:
- ✅ index.html
- ✅ script.js
- ✅ style.css
- ✅ supabase-config.js
- ✅ logo.png
- ✅ berger.jpg
- ✅ netlify.toml (nouveau fichier créé)
- ✅ netlify/functions/chat.js (nouveau fichier créé)

---

## Étape 2: Uploader sur GitHub

1. Allez sur votre repository: https://github.com/edgaryao/IADestin-eGlorieuse
2. Uploadez les nouveaux fichiers:
   - `netlify.toml`
   - Créez un dossier `netlify`
   - Dans ce dossier, créez un sous-dossier `functions`
   - Uploadez `chat.js` dans `netlify/functions/`

---

## Étape 3: Déployer sur Netlify

**1. Allez sur Netlify:**
- https://netlify.com
- Connectez-vous avec GitHub

**2. Nouveau site:**
- Cliquez **"Add new site"** → **"Import an existing project"**
- Choisissez **"GitHub"**
- Sélectionnez votre repository `IADestin-eGlorieuse`

**3. Configuration:**
- Build command: (laissez vide)
- Publish directory: `.` (point)
- Cliquez **"Show advanced"**

**4. Variables d'environnement:**
- Cliquez **"New variable"**
- Key: `GROQ_API_KEY`
- Value: `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`
- Cliquez **"Add"**

**5. Déployer:**
- Cliquez **"Deploy site"**
- ⏳ Attendez 1-2 minutes
- ✅ Votre site est en ligne!

---

## Étape 4: Configurer Supabase

**Important:** Ajoutez votre URL Netlify dans Supabase

1. Allez sur: https://supabase.com
2. Votre projet → Authentication → URL Configuration
3. Dans "Site URL", ajoutez: `https://votre-site.netlify.app`
4. Dans "Redirect URLs", ajoutez: `https://votre-site.netlify.app/**`
5. Cliquez "Save"

---

## ✅ C'est terminé!

Votre site est maintenant en ligne avec:
- ✅ Frontend sur Netlify
- ✅ Backend Supabase (base de données)
- ✅ API Groq sécurisée (clé cachée)

**Votre URL:** `https://votre-nom.netlify.app`

---

## 🔄 Mises à jour futures

Pour mettre à jour votre site:
1. Modifiez vos fichiers sur GitHub
2. Netlify redéploie automatiquement!

Aucune autre action nécessaire.
