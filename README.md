ZEN Home - Form

This small static form is prepared for Netlify (uses Netlify Forms attributes). UI is modern, responsive, and in French.

Fichiers:
- form.html — page principale (français). Form logic is kept intact for Netlify.
- styles.css — responsive styles and animations.

Tester localement
1. Ouvrez `form.html` dans un navigateur, ou servez-le via un simple serveur local.
   - Avec Python 3 (PowerShell):

```powershell
python -m http.server 8000
# puis ouvrez http://localhost:8000/form.html
```

2. Le formulaire envoie un POST vers `/`. En local le serveur statique renverra 404; pour tester l'expérience complète, déployez sur Netlify.

Déployer sur Netlify
1. Créez un nouveau site sur Netlify en connectant votre dépôt (ou en "Drag & Drop" du dossier `zen-home-form`).
2. Netlify détecte automatiquement les formulaires grâce à `data-netlify="true"` et au champ caché `form-name`.
3. Soumettez un formulaire depuis le site déployé et vérifiez les soumissions dans le tableau de bord Netlify > Forms.

Améliorations possibles
- Ajouter des validations côté client plus avancées.
- Ajouter tests d'intégration (puppeteer/playwright) pour vérifier la soumission.
- Externaliser les traductions si d'autres langues sont nécessaires.
