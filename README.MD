Presentazione
---
Per il seguente test, si chiede di generare un csv sommando due csv di partenza, presenti nella
cartella [resource/](https://github.com/trexon-ict/hiring-test-1/tree/master/resources), il file [a.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/a.csv) e [b.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/b.csv).

Il programma può essere scritto in uno dei seguenti linguaggi di programmazione: *php, java o javascript*.

Il primo csv, [a.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/a.csv), è formato dalle seguenti colonne:
```csv
CKY_ART;DESCR;CATEGORIA;COSTO\r\n
```

Il secondo csv, [b.csv](https://link), invece:
```csv
CKY_ART;EAN13;MARCA\r\n
```

Generare un'unico csv, con il nome file *out.csv*, che sia la somma di tutte le colonne dei due csv di base più una nuova colonna, `PREZZO`, che deve contenere il contenuto della colonna `COSTO` + un ricarico del 5%:
```csv
CKY_ART;DESCR;CATEGORIA;COSTO;PREZZO;EAN13;MARCA\r\n
```
Il formato dei csv [a.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/a.csv) e [b.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/b.csv) è:
- separatore di colonna: `;`
- separatore di campo: *nessuno*
- carattere di escape: `\\`
- separatore di riga: `\r\n`(CarrierReturn+LineFeed)

lo stesso formato va bene anche per il file di output *out.csv*.

Svolgimento
---
L'associazione dei campi del primo csv, [a.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/a.csv), a quelli del secondo, [b.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/b.csv), avviene confrontanto la colonna `CKY_ART`. Fare attenzione che nel csv [b.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/b.csv) potrebbe non esserci la riga relativa al csv [a.csv](https://github.com/trexon-ict/hiring-test-1/blob/master/resources/a.csv), ovvero, i campi `EAN13` e `MARCA` non esistono per tutti gli articoli; in questo caso i campi `EAN13` e `MARCA` del csv finale, *out.csv*, vanno lascati vuoti.

Fornire il codice sorgente e le istruzioni per poterlo eseguire per poi confrontare il risultato di output *out.csv*, salvandolo nella cartella radice del sorgente stesso.

Il tempo di consegna del test, come anche la documentazione nel sorgente e la spiegazione dello svolgimento, costituiscono punti a favore per la valutazione finale.

La consegna è preferibile sia fatta stesso tramite un repository personale su github.com, in modo da poter già iniziare ad imparare ed usare git.