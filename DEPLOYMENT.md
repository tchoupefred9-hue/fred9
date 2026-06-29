# Guide de Déploiement sur Vercel

## 🚀 Déployer votre Portfolio

### Option 1 : Déploiement Direct (Recommandé)

1. **Allez sur Vercel** : https://vercel.com
2. **Connectez votre compte GitHub**
3. **Importez le project** :
   - Cliquez sur "Import Project"
   - Sélectionnez le repository `fred9`
4. **Vercel détectera automatiquement** :
   - Framework: Next.js ✓
   - Build Command: `npm run build` ✓
   - Output Directory: `.next` ✓
5. **Cliquez "Deploy"** et attendez 2-3 minutes

### Option 2 : CLI Vercel

```bash
npm i -g vercel
vercel
```

### Variables d'Environnement

Si vous avez des variables d'environnement, ajoutez-les dans :
Settings → Environment Variables

### Domain Personnalisé

1. Allez dans les settings du projet Vercel
2. Cliquez sur "Domains"
3. Ajoutez votre domaine personnalisé
4. Configurez les DNS records selon les instructions Vercel

## 📋 Checklist avant Déploiement

- [ ] Vérifier que `npm run build` fonctionne localement
- [ ] Vérifier que `npm run dev` fonctionne
- [ ] Vérifier les liens de navigation
- [ ] Tester les formulaires (s'il y en a)
- [ ] Vérifier les images se chargent correctement
- [ ] Tester sur mobile
- [ ] Vérifier le SEO meta tags

## 🔍 Après Déploiement

### Analyser les Performances

1. Allez sur : https://vercel.com/analytics
2. Vérifiez Web Vitals
3. Vérifiez les temps de réponse

### Configurer Analytics

Vercel fournit analytics gratuits, accessibles dans le dashboard

### Monitoring

- Vercel notifie automatiquement les builds échoués
- Consultez les logs : https://vercel.com/dashboard/project/fred9

## 🆘 Dépannage

### Build échoue ?
```bash
npm run build  # Test localement
npm run lint   # Vérifier les erreurs
```

### Images ne s'affichent pas ?
- Vérifiez les chemins dans `next.config.js`
- Assurez-vous que `unoptimized: true` est activé

### Performance lente ?
- Verifiez les Core Web Vitals dans les analytics
- Optimisez les images (AVIF, WebP)
- Utilisez lazy loading pour les composants

## 📞 Support

- Docs Vercel : https://vercel.com/docs
- Support Vercel : https://vercel.com/support

---

**Votre portfolio est prêt pour le déploiement ! 🎉**
