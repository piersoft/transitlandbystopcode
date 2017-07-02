# transitlandbystopcode

Questo codice interroga il Database di TransitLand tramite le sue API  (info https://transit.land/documentation/datastore/api-endpoints.html) per avere i prossimi passaggi di mezzi pubblici dato uno stop_code.

Lo stop_code è il codice identificativo della Fermata dei Trasporti Pubblici. In alcune città come Palermo, Lecce ect tale codice è espresso sulla Palina di ogni fermata. 

Prerequisiti: il Feed GTFS del proprio gestore di trasporti pubblici deve essere già presente nel DB di Transitland


1) Inserire nella dir GTFS il file stops.txt del proprio gestore di trasporti pubblici
2) Nel file stops.txt identificare la posizione dei campi stop_code, stop_lat e stop_lon e modificare nel file index.php l'indice nelle righe 24, 27,29.
3) lanciare index.php?stop_code=numerostopcode ad esempio index.php?stop_code=320

A titolo di esempio sono usati i dati di Palermo.

ps: alla data attuale AMAT ha i GTFS che scadono il 30.06.2017 per cui TransitLand non fornisce risposta utile.


Licenza MIT @piersoft
