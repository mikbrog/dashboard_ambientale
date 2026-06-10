# API

In questo progetto le API sono simulate dal file ```data.json```

## Dati contenuti

Contiene metadata per la creazione del header di una tabella per la rappresentazione di dati e una lista di items che rappresentano le localita da visualizzare nella dashboard

## ```meta```

 Json contenente i metadata per la costurzione di una tabella

### ```projectTitle```

Campo contenente stringa che rappresenta il titolo del progtto.  
Tipo string.  
In questa versione non viene usato nel progetto.

### ```dataSource```

Campo che indica l'origine dei dati.  
Tipo string.  
In questa versione non viene usato nel progetto.

### ```description```

Campo contenente breve descrizione dell'obbietivo del progetto.  
Tipo string.  
In qesta versione non viene usato nel progetto.

### ```columns```

Campo contenente lista di json chhe saranno descritti sotto la voce ```column```.  
Tipo array.  
Viene recuperato da ```script.js``` per la costruzione di una tabella nella pagina ```dati.html``` per la visualizzazione dei dati.

#### ```column```

Json che contiene metadati per la creazione di una colonna per la tabella nella pagina ```dati.html```.  
Tipo json.

#### ```key```

Campo di ```column``` che rappresenta la key del json ```item``` da cui prendere i dati da inserire nella colonna della tabella.  
Tipo string.

#### ```label```

Campo di ```column``` che rappresenta i label della tabella nella pagina ```dati.html```.  
Tipo string.

## ```items```

Lista contentente molteplici ```item``` recuperata da ```script.js```
Tipo array.

### ```item```

Json che rappresenta una località di cui abbiamo i dati ambientali.
Tipo json.

### ```id```

Campo di ```item``` che identifica il singolo item.
Tipo int.

### ```title```

Campo di ```item``` contenente il titolo dell'item(nome della località).
Viene utilizzato come titolo per le card e come campo 'località' nella tabella in ```dati.html```  
Tipo string.

### ```subtitle```

Campo di ```item``` contenente il sottotitolo dell'item. Viene utilizzato nelle card in ```dati.html```
Tipo string.

### ```category``` 

Campo di ```item``` contenente la categoria dell'item. Viene utilizzato in ```dati.html``` per: la funzionalità di  filtro e ricerca; le card; nel campo 'Area' della tabella.
Tipo string.

### ```description```

Campo di ```item``` contenente la descrizione dell'item. Viene utilizzato in ```dati.html``` nelle card.
Tipo string.

### ```fields```

Json contenuto in ```item``` contenente delle varie informazioni legate all'item.
Tipo json

### ``` temperatura```

Campo di ```fields``` contenente la temperatura di uno specifico item.
Utilizzato in ```dati.html``` per: le card; il campo 'Temperatura' della tabella.
Tipo string.

### ```qualita_aria``` 

Campo di ```fields``` che rappresenta la qualità dell'aria di una località.
Utilizzato in ```dati.html``` per: le card, il campo 'Qualità aria' della tabella.
Tipo string.

### ```umidita```

Campo di ```fields``` che rappresenta l'umidità dell' aria di una località.
Utilizzato in ```dati.html``` per: le card, il campo 'Umidità` della tabella.
Tipo string.


### ```rumore```

Campo di ```fields``` che rappresenta il rumore medio(inquinamento acustico) di una località.
Utilizzato in ```dati.html``` per le card.
Tipo string.

