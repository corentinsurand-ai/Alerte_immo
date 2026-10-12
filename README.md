# 🏠 Alerte Immo Locatif — Val de Saône / Beaujolais

Ce dépôt est le **canal de notification** de Corentin pour sa veille d'investissement locatif :

- **Cible** : biens À TRAVAUX (appartements, maisons, **immeubles de rapport**) sur 6 communes : Villefranche-sur-Saône, Trévoux, Neuville-sur-Saône, Anse, Chazay-d'Azergues, Limonest.
- **Stratégie** : location meublée (LMNP) ou revente après travaux — rendement brut ≥ 6 %, pas de budget fixé (immeuble accepté si le rendement le justifie).
- **Pour chaque bien** : loyer meublé zone estimé + rendement brut, prix de revente fini estimé + plus-value, budget travaux ; pour les immeubles : nombre de lots divisibles + option revente à la découpe.
- **Mécanisme** : tous les matins à 10h00, la tâche Vibe cherche les nouvelles annonces et pousse un fichier `alerts/AAAA-MM-JJ.md`. Le workflow GitHub Actions (`.github/workflows/alerte.yml`) transforme ce fichier en **issue créée par le bot github-actions avec une mention @corentinsurand-ai** → GitHub envoie l'email de notification.

⚠️ Les issues ne doivent **jamais** être créées directement depuis le compte corentinsurand-ai : GitHub ne notifie pas ta propre activité. Seul le bot déclenche l'email.

Une issue par jour : « 🏠 … » ou « ✅ Rien de nouveau ».

*Ferme les issues après lecture, elles ne servent que de boîte de réception.*
