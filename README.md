# Automatisation et agents IA — Travaux pratiques

Ce dépôt rassemble progressivement les travaux pratiques et les exercices que je réalise dans le domaine de l'automatisation et de l'intelligence artificielle. L'objectif est de maîtriser les notions étudiées en les mettant en application : expérimenter différentes approches, écrire des programmes, tester les résultats et documenter les étapes ainsi que les concepts appris.

Chaque TP est organisé dans son propre dossier et accompagné, lorsque c'est utile, d'un guide expliquant les objectifs, les notions, les commandes et les résultats obtenus. Le dépôt évoluera au fil des exercices.

## Travaux pratiques

| Dossier | Sujet | Contenu |
|---|---|---|
| [`TP1/`](./TP1/) | Automatisation RPA avec Python | Lecture de données Excel, automatisation d'un formulaire avec Selenium, Playwright et PyAutoGUI, et envoi d'un email de test. |

## TP1 — RPA avec Python

Le dossier [`TP1/`](./TP1/) contient les scripts et le guide du TP d'automatisation d'un formulaire à partir d'Excel avec Selenium, Playwright et PyAutoGUI.

### Installation rapide (Windows / PowerShell)

Depuis la racine du dépôt :

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
Copy-Item .\TP1\contacts.example.xlsx .\TP1\contacts.xlsx
python .\TP1\tp1.py
```

Les scripts Selenium et Playwright utilisent le formulaire local `TP1/formulaire_test.html`. PyAutoGUI pilote la fenêtre active ; consulte le guide avant de le lancer.

Les emails sont désactivés par défaut. Le classeur personnel `TP1/contacts.xlsx`, les secrets et l'environnement virtuel ne doivent pas être publiés. Pour le test email sécurisé et les explications détaillées, consulte [`TP1/GUIDE_TP_RPA.md`](./TP1/GUIDE_TP_RPA.md).
