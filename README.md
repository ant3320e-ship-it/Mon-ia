# Mon IA — version web autonome

Ton IA open source tourne **directement dans le navigateur de ton téléphone**
grâce à [WebLLM](https://github.com/mlc-ai/web-llm) : pas d'ordinateur, pas de
serveur, pas d'API d'IA. Le modèle (Qwen 2.5 1.5B par défaut) est téléchargé
une seule fois depuis Hugging Face puis reste sur le téléphone, utilisable
hors ligne.

- Navigateur requis : Chrome sur Android, Safari sur iPhone (iOS 26+),
  Chrome/Edge sur ordinateur (WebGPU).
- Modèles au choix : Qwen 2.5 0.5B / 1.5B, Llama 3.2 1B / 3B.
- Internet : recherche Wikipédia avant de répondre + lecture des liens envoyés
  (via r.jina.ai), sources affichées sous la réponse.
- Nom, personnalité, créativité personnalisables ; historique gardé sur le
  téléphone ; installable sur l'écran d'accueil (« Ajouter à l'écran d'accueil »).

Fichiers : `index.html` (toute l'app), `manifest.webmanifest`, `icon.svg`.
Aucune étape de build : il suffit d'héberger ces fichiers (GitHub Pages,
Netlify…). Test local : `python3 -m http.server` puis http://localhost:8000.
