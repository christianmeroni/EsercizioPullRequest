# Come contribuire (regole della classe)

Grazie per la tua collaborazione! Questo repository serve ad allenarci con il workflow Git
usato da ogni squadra di sviluppo vera. Segui queste regole: sono le stesse che troverai
nei progetti open source.

## 1. Non si scrive mai direttamente su `main`

Il ramo `main` è **protetto**. Ogni modifica passa da una Pull Request.
Un push diretto su `main` verrà rifiutato da GitHub.

## 2. Nome dei branch

Usa questo formato:

| Prefisso | Quando si usa | Esempio |
|---|---|---|
| `sport/` | Esercizio "Il mio sport preferito" | `sport/rossi` |
| `feature/` | Nuova funzionalità | `feature/dizionario` |
| `fix/` | Correzione di un bug | `fix/errore-pag-12` |
| `docs/` | Solo documentazione | `docs/nuovo-readme` |

## 3. Messaggi dei commit

Formato consigliato (inglese o italiano, ma coerenti):

```
Aggiunge sport preferito di Rossi
Corregge refuso nel titolo della pagina 12
```

Niente "asdf", "modifiche", "cose varie".

## 4. La Pull Request

- Titolo che riassume il cambiamento.
- Descrizione compilata usando il **modello** che GitHub vi propone (vedi `.github/PULL_REQUEST_TEMPLATE.md`).
- **Almeno 1 review** da un compagno diverso da te, con approvazione.
- Tutti i commenti della review vanno **risolti** prima del merge.

## 5. Dopo il merge

- Chi ha aperto la PR clicca **Delete branch**.
- Tutti aggiornano la copia locale:

```bash
git checkout main
git pull
```

## 6. Se qualcosa va storto

- Conflitto? Non disperare: è normale. Chiedi al docente o a un compagno.
- Errori a cascata? `git log --oneline` per capire dove siete, e **mai** fare `push --force` su `main`.
