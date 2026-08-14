# 🏆 Champions du CP

Application d'apprentissage (style Lingokids) pour un enfant qui entre au **CP**.
Trois sports, trois matières, couvrant le programme des **4 premiers mois de CP** :

| Sport | Matière | Ce qui est travaillé |
|------|---------|----------------------|
| 🏀 Basket | **Mathématiques** | compter jusqu'à 10 puis 20, plus/moins, ranger les nombres, additions, compléments à 10, formes géométriques |
| ⚽ Foot | **Écriture** | tracer les voyelles, les consonnes et les chiffres au doigt, majuscule/minuscule, écrire des mots, écrire son prénom |
| 🎾 Tennis | **Lecture** | les voyelles, lire des syllabes, première lettre, « commence pareil », compter les syllabes, lire des mots |

## ✨ Ce qui est inclus
- **100 % hors-ligne** une fois installée (aucune connexion requise).
- **Voix française** intégrée : les consignes sont lues à voix haute (idéal avant de savoir lire) — utilise la synthèse vocale du téléphone.
- **Gamification** : étoiles (1 à 3 par défi), coupes bronze/argent/or, **vitrine des coupes**, confettis, mascotte animée, trophée de champion quand un sport est terminé.
- **Prénom personnalisable** : l'enfant saisit son prénom au premier lancement (utilisé dans l'accueil et le défi « Écris ton prénom »).
- **Réglages** (roue crantée) : changer le prénom, couper le son, remettre les coupes à zéro.
- Exercices **maths générés à l'infini** (rejouables sans se répéter), contenus de lecture/écriture soignés.

## 📲 Installer sur le téléphone Android (via GitHub Pages)
1. Créer un dépôt GitHub (ex. `champions-cp`) et y **déposer tous les fichiers** de ce dossier
   (`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`).
2. Dans le dépôt : **Settings → Pages → Build and deployment → Source : `Deploy from a branch`**,
   branche `main`, dossier `/ (root)`, puis **Save**.
3. Attendre 1–2 minutes : GitHub affiche une adresse du type
   `https://<ton-pseudo>.github.io/champions-cp/`.
4. Ouvrir cette adresse dans **Chrome sur le téléphone** → menu ⋮ → **« Ajouter à l'écran d'accueil »**.
   L'appli s'installe avec son icône et fonctionne ensuite **sans internet**.

> Astuce : après la première ouverture en ligne, tout est mis en cache. Les fois suivantes, l'appli
> démarre même en mode avion. Si tu mets à jour les fichiers plus tard, change `champions-cp-v1`
> en `-v2` dans `sw.js` pour forcer la mise à jour sur le téléphone.

## 🔊 La voix ne parle pas ?
- Vérifier que le son n'est pas coupé dans les **Réglages** de l'appli (roue crantée).
- Sur Android : *Paramètres → Langues et saisie → Synthèse vocale* — installer/activer une voix **française**.
- La voix se déclenche après le premier appui à l'écran (sécurité des navigateurs).

## 🛠️ Tester en local (optionnel)
```bash
cd champions-cp
python3 -m http.server 8000
# puis ouvrir http://localhost:8000
```
(Un simple serveur est nécessaire pour que le service worker fonctionne — un double-clic sur le fichier
suffit pour jouer, mais pas pour installer l'appli.)
