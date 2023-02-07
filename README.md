# Elaborato sis

---
## FSMD.blif
Questa è la parte principale del programma, dove avviene il sugoma.

Questa parte permette di:
 - avviare "accensione.blif" e inserire i posti occupati.
 - controllare se i posti dei vari settori sono occupati.
 - aprire il cancello nel caso il settore immesso sia corretto e non pieno.
 - chiudere il cancello qualche secondo dopo averlo aperto.
 - avviare "sommatore.blif" e "sottrattore.blif" nel caso il cancello sia aperto e verrà scelto uno dei due programmi in base all'entrata o uscita.

---
## accensione.blif
Questa parte di programma permette di modificare gli stati: on, off, a, b, c.

- off: il dispositivo è spento (occorre attivarlo inserendo 11111).
- on: il dispositivo è acceso e viene mantenuto tale (per spegnerlo: 00000).
- a: se on attivo(1) permette di inserire i posti occupati presenti nel settore A.
- b: se on attivo(1) permette di inserire i posti occupati presenti nel settore B.
- c: se on attivo(1) permette di inserire i posti occupati presenti nel settore C.

---
## acc_jedi.blif
Versione di "accensione.blif" con memoria.

Comandi da usare sul terminale:
1) rl accensione.blif (legge il dile "accensione.blif")
2) state_sign jedi (trasforma il file in tipologia jedi)
3) wl acc_jedi.blif (scrive il programma nel file "acc_jedi.blif")

---
## sommatore.blif
Questa parte di programma permette di ricevere in input 5 bit e restituire il numero corrente sommato di 1.

_`(ATTENZIONE: la seguente situazione non dovrà mai verificarsi)`_
_Nel caso il risultato assuma il numero massimo possibile, verrà sempre restituito il numero limite._

---
## sottrattore.blif
Questa parte di programma permette di ricevere in input 5 bit e restituire il numero corrente sottratto di 1.

_`(ATTENZIONE: la seguente situazione non dovrà mai verificarsi)`_
_Nel caso il risultato assuma un numero minore di 0, verrà sempre restituito il numero._
