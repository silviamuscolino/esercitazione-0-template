# Osservazioni — Esercitazione 0

Gruppo: c18

Componenti (nome, cognome e username GitHub di entrambi): Silvia Muscolino, username: silviamuscolino; Lavinia Palumbo, username: laviniapalumbo

URL del repository condiviso:

Chi ha usato la tastiera nello step 1 e nello step 2: nello step 1 Silvia Muscolino, nello step 2 Lavinia Palumbo

Compilate insieme le osservazioni e discutete le risposte: entrambi dovete
saper spiegare le prove svolte.

## Step 1 — Hello World: compilazione ed esecuzione

Comando di compilazione: gcc -std=c17 -Wall -Wextra -Wpedantic hello.c -o hello

Comando di esecuzione e risultato osservato:  ./hello  il risultato osservato è la scritta stampata richiesta

Che cosa ho capito su sorgente ed eseguibile: con hello.c che è la sorgente si scrive il codice.  hello, l'eseguibile, dopo la compilazione esegue e stampa su schermo l'output richiesto

Output richiesto e comportamento del programma prima della modifica: l'output richiesto è "hello, computational physics", prima della modifica il programma compilava correttamente senza stampare nulla

Esito dopo la modifica e spiegazione della correzione: dopo la modifica compilando l'eseguibile stampa la stringa richiesta, la correzione è avvenuta inserendo l'istruzione printf con il messaggio richiesto e ricompilando

## Step 1 — Git

Quali file ho incluso nel commit e perché: i file inclusi sono hello.c e osservazioni.md perchè includo solo i file sorgente e di documentazione in quanto l'eseguibile può essere rigenerato compilando

Come ho verificato che la versione provata sia presente su GitHub: con il comando git log --oneline controllo la cronologia e apro il file per verificarne il contenuto. ricaricata la pagina su github, vedo i file aggiornati.

Che cosa ho osservato prima e dopo `git pull`, e perché non serve un nuovo clone:  prima di git pull il file sul computer non aveva le modifiche effettuate su github, dopo git pull le modifiche fatte su github sono state scaricate nel repository locale del computer. Non serve un nuovo clone perchè git pull aggiorna in automatico le modifiche effettuate

## Step 2 — Eco: prima prova

Argomenti passati, comando e risultato:  Gli argomenti passati sono"gatto" e "cane", il comando per compilare è ./eco, il risultato è che viene stampato su schermo tramite argv[] le due parole scelte gatto e cane

Che cosa posso concludere: tramite l'array argv[] il main riceve gli argomenti e li stampa nel terminale eseguendo il programma

## Step 2 — Eco: seconda prova

Argomenti passati, comando e risultato: gli argomenti passati sono skric  29 6.7, il comando  è ./eco e il risultato è che il programma legge gli argomenti e converte la stringa 29 nell'intero 29 usando atoi e la stringa 6.7 nel numero decimale usando atof, e stampa correttamente attraverso printf skric 29 6.70000

Che cosa ho capito su testo, conversioni e stampa: i parametri inseriti nel terminale per eseguire arrivano sottoforma di testo al programma, che converte il testo in valore numerico tramite le funzioni atoi e atof, stampando testo, valore intero e valore decimale correttamente.

## Step 2 — Risultato ed errori

Previsioni per l'esecuzione con argomenti validi e per quella con `dodici`:con argomenti validi come i numeri 29 e 6.7 le conversioni hanno successo. se uso invece la parola "dodici" al posto dei numeri interi,stampa 0 sul terminale perchè non riesce a convertire le lettere come numeri.

Contenuto di `eco.txt`, messaggi nel terminale e codici di uscita osservati: eseguendo ./eco skric 29 6.7 > eco.txt, l'output di testo viene reindirizzato e salvato nel file eco.txt. eseguendo il programma senz argomenti, il messaggio di errori viene restituito sul terminale.

Come un controllo automatico può riconoscere un errore: verificando il valore return 2 (in caso di errore) oppure controllando che il canale di uscita degli errori contenga il messaggio di uso.

## Step 2 — Parametri e calcolo fisico

Quando serve ricompilare e quando basta cambiare gli argomenti: serve ricompilare quando si applica una modifica al codice sorgente in C (eco.c). basta cambiare gli argomenti quando il codice sorgente rimane uguale e si vuole variare solo i dati di input.
## Step 2 — Git

Come riconosco nella cronologia i commit dei due step: eseguendo git log-- onelie, riconosco i commit nella cronologia dal messaggio inserito durate il commit e dai codici identificativi (hash).

Come ho verificato che la versione finale sia presente su GitHub: dopo git push, ho ricaricato la pagina repository su github verificando così che l'ultimo commit fosse visibile e che il file osservazioni.dm avesse al suo interno tutte le risposte aggiornate.
