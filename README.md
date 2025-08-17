#  chatbotIA — Chatbot Intelligent pour la Q&A sur Documents PDF

**chatbotIA** est un assistant intelligent développé en **Python** capable de répondre à des questions en se basant sur le contenu de fichiers PDF téléchargés par l’utilisateur.  
Ce projet a été réalisé dans le cadre de l’année universitaire **2024/2025** en filière **Génie Industriel — Intelligence Artificielle et Data Science**, encadré par **Mr. Masrour Tawfik**.

---

##  Objectifs du projet
- Traiter plusieurs fichiers PDF en même temps.
- Extraire et indexer leur contenu pour des recherches rapides.
- Fournir des réponses précises et contextuelles aux questions posées.
- Maintenir un historique complet des interactions.
- Afficher les documents utilisés et le temps de réponse.

---

##  Architecture de l’application

###  Technologies utilisées :
- **Python** — Langage principal.
- **Streamlit** — Interface utilisateur web.
- **Groq (Llama3-8b)** — Génération de réponses contextuelles.
- **FAISS** — Indexation et recherche rapide.
- **LangChain** — Orchestration des composants.
- **HuggingFaceEmbeddings** — Création des vecteurs sémantiques (embeddings).

###  Workflow technique :
1. **Téléversement** d’un ou plusieurs fichiers PDF.
2. **Découpage** du contenu en segments de texte (chunks).
3. **Génération d’embeddings** vectoriels.
4. **Indexation** avec FAISS.
5. **Recherche** des segments les plus pertinents pour la question.
6. **Génération** de la réponse avec Groq (Llama3-8b).
7. **Affichage** du contexte utilisé, du temps de réponse et de l’historique.

---

##  Aperçu
![Aperçu du chatbot](docs/images/demo.gif)  
*Exemple de session avec chatbotIA.*


---

##  Installation

1. **Cloner le dépôt** :
```bash
git clone https://github.com/kawahattaki/sphinx_docs
cd chatbotIA
