# find_snapshot_app
Ricerca sugli application server glassfish quali sono le applicazioni di tipo SNAPSHOT (app maven); Crea un file di resoconto

# descrizione
vengono analizzati tutti i server di produzione che soddisfano nell'inventory_hostname la nomenclatura
*-ecas*
*-as*

(non ricerchiamo inutilmente su server che non hanno installato Glassfish4)

Il file di resoconto viene prodotto sul server ansible.
Il path assoluto del file è:

/tmp/resoconto_find_snapshot_app.csv

per ogni riga, la struttura è questa:

<inventory_hostname>;app1;app2;....;appn
