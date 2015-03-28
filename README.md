# Produttore-Consumatore
## Autori
    Angeli Emanuele  
    Infanti Enrico
    
## Versione
    5.0

## Data release
    28/03/2015
    
##Descrizione programma
    
    Il funzionamento di questo programma Produttore/Consumatore è molto semplice, in poche parole abbiamo due thread:
    -Produttore: Genera dei numeri casuali all'interno di un range scelto da noi (Es: da 0 a 9) con una sua velocità e 
                 un suo tempo, questi numeri vengono inseriti all'interno di un Buffer.
    -Consumatore: Preleva dal Buffer i numeri o gli elementi inseriti dal thread Produttore e gli stampa in maniera 
                  ordinata in base a come gli ha prelevati.
    Da qui però, essendoci tempi e velocità diverse nel 'produrre' e 'consumare' gli elementi, nasce il problema del Busy
    Waiting, (Il problema di chi deve entrare nel buffer per primo).
    Questo problema viene risolto usando una variabile booleana (Flag) che se è impostata a 'True' fa in modo che uno dei     due thread rimane obbligatoriamente in attesa che l'altro abbia finito il suo lavoro. Se è impostata a 'False' su uno     dei due thread da la possiblità all'altro di entrare e compiere il suo compito.
