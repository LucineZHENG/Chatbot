# ✈️ VoyageAssistant : Chatbot multilingue de réservation de vols

VoyageAssistant est un système conversationnel de réservation de vols basé sur les **grands modèles de langage (LLM)**.  
Ce projet a été réalisé dans le cadre du **Master 2 “Langue et Informatique” à Sorbonne Université**.

Le système permet aux utilisateurs d’effectuer des **requêtes de réservation de vols via un dialogue en langage naturel**, incluant la recherche, la comparaison et la confirmation de réservation.  
Il prend en charge **trois langues : français, anglais et chinois**.

---

## ✨ Fonctionnalités principales

### 🌍 Support multilingue
Interaction en langage naturel en **français, anglais et chinois**.

### 🧠 Compréhension du langage naturel (NLU)
Grâce au **Prompt Engineering avec LLM**, le système identifie :

- l’**intention** de l’utilisateur (*intent*)
- les **informations clés** (*slots*)

Par exemple :

- ville de départ  
- ville d’arrivée  
- date du vol  
- compagnie aérienne  

### 🗣 Génération du langage naturel (NLG)
Le système génère des réponses naturelles en fonction :

- du contexte du dialogue  
- des résultats de recherche dans la base de données des vols.

### 🔄 Gestion du dialogue multi-tour
Le chatbot gère l’ensemble du processus de réservation :

Recherche → Comparaison → Sélection → Confirmation de réservation

---

## 📂 Structure du projet

### `VoyageAssistant_fixed.ipynb`
Notebook principal contenant :

- la gestion du dialogue
- les appels à l’API LLM
- les modules NLU et NLG

### `flights_database_v2.json`
Base de données simulée de vols contenant environ **300 vols**.

### `lexique_voyage_v2.json`
Lexique multilingue et règles de prompts :

- intents  
- slots  
- instructions pour le LLM

### `airtalk_600_multilingual_fixed.json`
Corpus multilingue contenant **600 énoncés utilisateurs annotés**.

### `dialogues_voyage.json`
20 scénarios de dialogues multi-tours utilisés pour tester le système.
