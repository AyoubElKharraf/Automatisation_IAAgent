# Automatisation IA Agent

Travaux pratiques d'automatisation et d'agents IA.

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
