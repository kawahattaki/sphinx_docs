Installation
============

Prérequis
---------
- Python 3.11 ou supérieur
- pip installé
- (Optionnel) Un environnement virtuel

Remarques importantes
---------------------
- Le fichier `.env` n’est pas fourni dans ce projet car il contient la clé API personnelle.
  Vous devez créer ce fichier manuellement à la racine du projet et y ajouter votre clé API :

  .. code-block:: text

     GROQ_API_KEY=votre_cle_api

- Les fichiers volumineux générés par FAISS (index de vecteurs) ne sont pas inclus dans le dépôt.
  Ils seront créés automatiquement lors du premier téléversement de documents PDF dans l’application.

Étapes
------
1. Cloner le dépôt :
   .. code-block:: bash

      git clone  https://github.com/kawahattaki/sphinx_docs
      cd chatbotIA

2. (Optionnel) Créer un environnement virtuel :
   .. code-block:: bash

      python -m venv venv
      venv\Scripts\activate   # Windows
      source venv/bin/activate   # Linux/Mac

3. Installer les dépendances :
   .. code-block:: bash

      pip install -r requirements.txt

4. Lancer l’application :
   .. code-block:: bash

      streamlit run app_mod.py
