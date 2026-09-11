# 20-Agno-Team

App Streamlit d'analyse automatisée de contrats. L'utilisateur upload un contrat (PDF/DOCX/TXT), le texte est extrait (PyMuPDF), puis une équipe coordonnée de 3 agents spécialisés — Structure, Problèmes juridiques (citant les clauses exactes, signalant les risques/RGPD), et Stratégie de négociation — l'analysent conjointement ; un agent manager fusionne leurs sorties en un rapport markdown consolidé (résumé exécutif, contexte juridique, structure, négociation), téléchargeable.

## Tech stack

streamlit, agno (Agent, Team, mode coordinate), Groq (`openai/gpt-oss-120b` pour les agents, `openai/gpt-oss-20b` pour le leader), PyMuPDF, python-dotenv

## Lancer le projet

```bash
pip install -r requirements.txt
```

Créer un `.env` avec `GROQ_API_KEY=...`

```bash
streamlit run app.py
```
