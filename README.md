# Competition Datathon - PolyFinance 2024
## Question à résoudre : Comment exploiter l’IA générative pour apporter un support efficace aux analystes financiers ?


## Projet : Exploitation de l'IA Générative pour le Support aux Analystes Financiers

### Description du Défi
Les analystes financiers traitent des volumes importants de données et de rapports pour générer des insights, évaluer la performance d’entreprises et analyser les données. L’IA générative est une technologie puissante qui pourrait aider à analyser ces quantités importantes de données.

### Enjeux
1) Volume de Données : Les analystes doivent gérer des ensembles de données de plus en plus vastes, ce qui rend l'analyse manuelle inefficace.
2) Extraction d'Insights : Identifier rapidement des informations pertinentes à partir de données complexes est un défi constant.
3) Technologie Avancée : L'adoption de l'IA générative pourrait révolutionner la façon dont les analyses financières sont effectuées.

### Objectif du Projet
1) Conception de Solutions IA : Développer des solutions basées sur l'IA qui aident les analystes financiers à analyser des données financières.
2) Suivi des Tendances : Permettre le suivi en temps réel des tendances du marché financier.
3) Utilisation de Données en Temps Réel : Intégrer des indicateurs de performance et des analyses de risques pour offrir une vision précise de l’évolution du marché.

### Valeur Ajoutée Attendue
1) Simplification des Analyses : Une solution basée sur l’IA générative capable de simplifier les analyses pour les analystes financiers.
2) Insights Clairs et Exploitables : Fournir des informations claires et actionnables pour faciliter la prise de décision.
3) Efficacité Améliorée : Réduire le temps nécessaire pour traiter et analyser les données financières.


[Notre environnement de developpement est Cloud9]
On va utiliser Amazon Bedrock to build LLMs - build n scale genAI apps: 
--> Guardrails (only answers one type of answer) 
--> Agents (to access outside the LLM): Agents can execute multistep tasks , basically it can touch other system to do an action
--> Studio (To create agents and chatbots easiear)
--> Customization, Custom Model Imports, Amazon Models (Create and customize out own LLMs)

Retrieval Augmented Generation (RAG): 
--> We connect to a database and on that database we get for example information on a company - we pair that by using the already existent intelligence in the LLM + the specific information we give him to get more precise answers

### Working with Amazon Bedrock:
1) Temperature: While using a model always keep the "temperature" of the model at 0 for data analysis because we only want facts no creativity
2) Top K & TopP: Top-k and Top-p are techniques used in the sampling process of language models to control the randomness and quality of generated text. These methods help in managing the balance between diversity and coherence in generated outputs.
   --> In Top-k sampling, the model limits the pool of candidate tokens to only the top k most probable tokens and samples from this reduced set. The other tokens are disregarded, even if they have non-zero probabilities. Standardized at 250.
   --> Top-p sampling, also known as nucleus sampling, considers the smallest possible set of tokens whose cumulative probability exceeds a threshold p. Instead of a fixed number of tokens, the set's size can vary dynamically based on the distribution. If p is set to 0.9, the model includes tokens until their cumulative probability sum reaches 90%, regardless of how many tokens that may include. Standardized at 250 0.99.
#### Bedrock Studio 
Helps ease the developpement of solutions

hello






