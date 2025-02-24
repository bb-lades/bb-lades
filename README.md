- 👋 Hi, I’m @bb-lades
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
bb-lades/bb-lades is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Guide d'installation et de configuration de ML-Agents avec Unity et Python

1. Prérequis

Avant d'installer ML-Agents, assurez-vous d'avoir les bonnes versions des outils suivants :

Unity : Version récente recommandée (2022.3 ou plus)

Python : 3.10.11 ou 3.10.12 (Les autres versions peuvent poser problème)

Git : Dernière version installée

Unity ML-Agents : Version 1.1.0 (testée et fonctionnelle)

2. Installation de ML-Agents dans Unity

ML-Agents n'est pas disponible directement dans le Package Manager d'Unity. Il faut l'ajouter via Git.

Étape 1 : Ajouter ML-Agents dans Unity

Ouvrez Unity et allez dans Window > Package Manager

Cliquez sur le bouton + en haut à gauche

Sélectionnez Add package from git URL

Entrez l'URL suivante :

https://github.com/Unity-Technologies/ml-agents.git?path=com.unity.ml-agents

Cliquez sur Add et attendez que l'installation se termine.

Si l'installation est réussie, vous verrez ML-Agents dans le Package Manager sous "Other".

3. Installation de ML-Agents dans Python

Pour établir une connexion entre Unity et Python, vous devez installer mlagents_envs.

Ouvrez un terminal (CMD, PowerShell ou Terminal sur macOS/Linux)

Installez le package avec la commande suivante :

python -m pip install mlagents_envs==1.1.0

Attention : Assurez-vous que Python est bien en version 3.10.11 ou 3.10.12.

4. Lancer ML-Agents dans Unity

Dans Unity, allez dans Window > ML-Agents

Sélectionnez ML-Agents Editor

Configurez vos agents et environnements

Lancez l'entraînement ou testez vos agents en simulation

5. Éviter les erreurs fréquentes

Conflit de ports entre Unity et Python

ML-Agents utilise des ports pour la communication, ce qui peut causer des conflits.

Solution : Fermez Unity complètement avant de redémarrer un nouvel environnement.

Unity ne détecte pas ML-Agents

Vérifiez que l'installation via Git a bien été faite

Relancez Unity après l'ajout du package

Erreur "ModuleNotFoundError: No module named 'mlagents_envs'"

Vérifiez que Python est bien en version 3.10.11 ou 3.10.12

Réinstallez avec : python -m pip install mlagents_envs==1.1.0
