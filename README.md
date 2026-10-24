# AgriPlus
AgrisPlus est un système multi-agents de gouvernance phytosanitaire pour le Cameroun, visant à détecter les maladies phytosanitaires et fournir des recommandations pertinentes. Elle repose sur une base de connaissance vérifiée qui alimente des agents, afin de les permettre de jouer leur rôle institutionnel de manière efficace.

# AgriPlus v2 – Système multi-agents de gouvernance phytosanitaire pour le Cameroun
ITU AI for Good Lab Hackathon (Émirats arabes unis). Finale : 8 décembre 2026. Soumission : avant le 10 novembre 2026.

# Principe
Une base de connaissances vérifiée (lois, décrets, arrêtés, règlements régionaux) alimente des agents qui jouent des rôles institutionnels. Face à un incident, ils donnent des avis sous des mandats différents, citent leurs sources, laissent une trace d'audit et révèlent les écarts de politiques. Le dispositif IoT (capteurs, caméras, Raspberry Pi) est la couche terrain.
# Règle d'or 
Si aucune source ne soutient une réponse, l'agent répond « aucune base juridique trouvée » et le signale comme écart. Il n'invente jamais.

# Structure du dépôt
Dossier	Contenu
`kb/`	Corpus brut (`raw`), version nettoyée (`clean`), schémas de métadonnées (`schema`), scripts d'ingestion (`scripts`), liste des sources (`sources_a_collecter.csv`), jeu de 30 questions-réponses étalon
`agents/`	Définition des agents et mandats (`agents.yaml`), schéma des messages (`message_schema.json`), spécification déclarative (`agriplus_intent.yaml`)
`audit/`	Schéma du journal d'audit, journal, vue lisible, outil de vérification de la chaîne
`scenarios/`	Scénarios en étapes, information libérée par morceaux
`iot/`	Code du Raspberry Pi, intégration du modèle, application mobile
`report/`	Rapport de 5 pages, tableaux de mapping, sources avec liens
`docs/`	Notes de travail
Installation en 5 commandes
À compléter au fil du projet (J9).
```
1. git clone <url-du-depot>
2. cd agriplus
3. (à définir : environnement)
4. (à définir : ingestion de la base de connaissances)
5. (à définir : lancement du scénario)
```
Licence
À décider (voir `DECISIONS.md`, D10).
Statut des sources
Aucun texte n'est cité tant qu'il n'a pas été contrôlé contre un texte primaire par deux personnes. Voir `kb/sources_a_collecter.csv`.
