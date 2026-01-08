# Generic Maintenance Page

Une page de secours universelle et esthétique pour éviter d'afficher des erreurs serveurs brutes (type **Gateway Timeout**) à vos utilisateurs.

**Démo Live :** [https://maintenance-page-puce.vercel.app](https://maintenance-page-puce.vercel.app)

---

###  Pourquoi utiliser cette page ?

En production, un serveur peut être indisponible pour plusieurs raisons :

* **Déploiement :** Redémarrage de l'application.
* **Erreur critique :** Saturation ou crash du conteneur.
* **Démarrage à froid :** Le conteneur est "UP" mais l'application n'est pas encore prête.
* **Maintenance :** Mise à jour programmée.

Plutôt que de laisser le navigateur afficher un **Gateway Timeout par exemple** froid et technique, cette page intercepte la requête pour protéger votre image de marque et rassurer vos visiteurs.

---

### Exemple de configuration (Coolify / Proxy)

Branchez simplement l'URI de redirection dans votre configuration de proxy :

1.  Allez dans **Serveur** > **Proxy** > **Configuration**.
2.  Cochez la case **"Override default request handler"**.
3.  Dans le champ **"Redirect to"**, collez : `https://maintenance-page-puce.vercel.app`
4.  Cliquez sur **Save**.
5.  Oublier pas **restart le proxy**.

---

###  Contributions

Le design se veut volontairement simple et "KISS". N'hésitez pas à envoyer une **Pull Request** si vous souhaitez améliorer l'UI ou proposer de nouvelles variantes ! :)

---
