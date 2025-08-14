Architecture de l'application
=============================

Technologies utilisées
----------------------
- **Streamlit** : interface utilisateur web.
- **Groq (Llama3-8b)** : génération de réponses.
- **FAISS** : indexation et recherche rapide.
- **LangChain** : orchestration des composants.
- **HuggingFaceEmbeddings** : création des embeddings.

Flux de traitement
------------------
1. Téléversement de fichiers PDF.
2. Découpage en segments de texte.
3. Génération d’embeddings vectoriels.
4. Indexation avec FAISS.
5. Recherche de segments pertinents.
6. Génération de la réponse via Groq.
7. Affichage à l’utilisateur avec détails et historique.
