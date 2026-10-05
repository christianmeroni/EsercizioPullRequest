# classe-4ib-practice

Repository di allenamento per la classe **4IB**: qui si impara il workflow Git + Pull Request.

> ⚠️ **Il ramo `main` è protetto**: ogni modifica passa obbligatoriamente da una **Pull Request** con la review di un compagno.

## Come si lavora (regole della classe)

```
branch → commit → push → Pull Request → review → approve → merge → pull
```

1. **Mai pushare direttamente su `main`** (GitHub te lo impedisce comunque).
2. Si lavora sempre su un branch con nome `<prefisso>/<tuo-nome>`, es. `sport/rossi`.
3. Ogni PR deve essere reviewata da **un compagno diverso dall'autore**.
4. Il messaggio del commit spiega *cosa* e *perché*.
5. Dopo il merge: `git checkout main && git pull`.

## Struttura del repository

```
├── README.md                ← questo file
├── CONTRIBUTING.md          ← regole di collaborazione (legtelo prima di iniziare)
├── .github/
│   └── PULL_REQUEST_TEMPLATE.md   ← modello da compilare a ogni PR
└── sport/
    └── esempio.md           ← file di esempio: fate il vostro seguendo questo
```

## Avvio rapido (per gli studenti)

```bash
git clone https://github.com/NOME-ORG/classe-4ib-practice.git
cd classe-4ib-practice
git checkout -b sport/<tuo-cognome>
# crea il file sport/<tuo-cognome>.md seguendo sport/esempio.md
git add sport/
git commit -m "Aggiunge sport preferito di <cognome>"
git push origin sport/<tuo-cognome>
# → apri la Pull Request su GitHub e chiedi la review a un compagno
```
