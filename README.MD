Presentazione
---
Per il seguente test, si chiede di generare un csv sommando due csv di partenza, presenti nella
cartella [resource/](https://link), il file [a.csv](https://link) e [b.csv](https://link).

Il programma può essere scritto in uno dei seguenti linguaggi di programmazione: *php, java o javascript*.

Il primo csv, [a.csv](https://link), è formato dalle seguenti colonne:
```csv
CKY_ART;DESCR;CATEGORIA;COSTO\n
```

Il secondo csv, [b.csv](https://link), invece:
```csv
CKY_ART;EAN13;MARCA\n
```

Generare un'unico csv, con il nome file *out.csv*, che sia la somma di tutte le colonne dei due csv di base più una nuova colonna, `PREZZO`, che deve contenere il contenuto della colonna `COSTO` + un ricarico del 5%:
```csv
CKY_ART;DESCR;CATEGORIA;COSTO;PREZZO;EAN13;MARCA\n
```
Il formato dei csv [a.csv](https://link) e [b.csv](https://link) è:
- separatore di colonna: `;`
- separatore di campo: *nessuno*
- carattere di escape: `\\`

lo stesso formato va bene anche per il file di output *out.csv*.

Svolgimento
---
L'associazione dei campi del primo csv, [a.csv](https://link), a quelli del secondo, [b.csv](https://link), avviene confrontanto la colonna `CKY_ART`. Fare attenzione che nel csv [b.csv](https://link) potrebbe non esserci la riga relativa al csv [a.csv](https://link), ovvero, i campi `EAN13` e `MARCA` non esistono per tutti gli articoli; in questo caso i campi `EAN13` e `MARCA` del csv finale, *out.csv*, vanno lascati vuoti.

Fornire il codice sorgente e le istruzioni per poterlo eseguire per poi confrontare il risultato di output *out.csv* messo nella cartella radice del sorgente stesso.