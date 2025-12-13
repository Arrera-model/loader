# ArreraIALoad

Charge et exécute directement des modèles d’IA à partir de leurs fichiers.  
Cette classe agit comme un conteneur pour un modèle chargé en mémoire.

## Methode

### Private

- **__predict_arrera_2026_model** : Gère l’envoi de requêtes au modèle de texte d’Arrera. Prend en paramètre *sentence*, qui correspond à la phrase de l’utilisateur, et *confidence_threshold*, qui correspond au seuil de confiance.
- **__predict_gguf_model** : Gère l’envoi de requêtes à des modèles locaux (.gguf) chargés au préalable

## Public

- **send_request** : Permet d’envoyer des requêtes au modèle chargé. Prend les mêmes paramètres que les méthodes privées *predict* correspondant à chaque modèle.
- **loadArreraModel2026** : Charge les modèles d’IA développés par Arrera en 2026.
- **load_help_file** : Charge un fichier d'aide pour donner des instruction en plus a l'IA
- **unload_help** : decharge le fichier d'aide
- **load_model_gguf** : Charge les modèles d’IA téléchargés en local au format .gguf 