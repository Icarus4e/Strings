# Strings

Questo progetto nasce con l'obiettivo di offrire uno strumento utile per lo studio delle stringhe ASCII 7 bit, senza l'uso di caratteri unicode.

L'applicazione, disponibile per sistemi Linux anche in versione console, permette di elaborare una stringa in ingresso e visualizzarne:

 - la sua versione Maiuscola
 - la sua versione Minuscola
 - se contiene solo caratteri Alfabetici
 - di quante lettere è formata
  - se contiene solo caratteri Alfanumerici
 - la sua versione rovesciata
 - di quante parole e formata
 - la versione Capitalized 
 - se è Palindroma
 
Per garantire la massima usabilità, l'applicazione è stata progettata per essere eseguita su sistemi Linux anche in versione console.

L'implementazione dell'applicazione ha richiesto l'utilizzo di operatori logici and, or e xor, nonché di alcune funzioni predefinite del linguaggio di programmazione utilizzato.


# Metodi

 

 1. Maiuscolo 
 

> **La funzione `ConvertToUppercase` converte ogni lettera minuscola in maiuscola nella stringa di input, lasciando intatti tutti gli altri caratteri. La funzione utilizza un loop for per iterare attraverso ogni carattere della stringa di input e utilizza la funzione `ToUpper` per convertire ogni lettera minuscola in maiuscola. Infine, la funzione restituisce la stringa convertita.**

 2. Minuscola
 

**> La funzione `ConvertToLowercase` converte ogni lettera maiuscola in minuscola nella stringa di input, lasciando intatti tutti gli altri caratteri. La funzione utilizza un loop for per iterare attraverso ogni carattere della stringa di input e utilizza la funzione `ToLower` per convertire ogni lettera maiuscola in minuscola. Infine, la funzione restituisce la stringa convertita**.

 4. Caratteri Alfabetici
 

> **La funzione `IsOnlyLetters` verifica se la stringa di input è composta solo da lettere alfabetiche. La funzione utilizza un loop foreach per iterare attraverso ogni carattere della stringa di input e utilizza la funzione `char.IsLetter` per verificare se il carattere è una lettera alfabetica. Se un carattere non è una lettera alfabetica, la funzione restituisce `false` per indicare che la stringa non contiene solo lettere. Se tutti i caratteri della stringa sono lettere, la funzione restituisce `true`.**

 6. Numero di lettere
 

**> La funzione `CountLetters` conta il numero di lettere presenti nella stringa di input. La funzione scorre ogni carattere della stringa di input e, se il carattere è una lettera dell'alfabeto (cioè se si trova nell'intervallo 'A'-'Z' o nell'intervallo 'a'-'z'), incrementa un contatore di lettere. Alla fine, la funzione restituisce il valore del contatore.**

 8. Alfanumerici
 

> **La funzione `IsAlphanumeric` controlla se la stringa di input contiene solo caratteri alfanumerici. La funzione scorre ogni carattere della stringa di input e, se il carattere non è una lettera dell'alfabeto (cioè non si trova nell'intervallo 'A'-'Z' o nell'intervallo 'a'-'z') e non è un numero (cioè non si trova nell'intervallo '0'-'9'), restituisce `false`. Se alla fine della scansione tutti i caratteri della stringa sono alfanumerici, la funzione restituisce `true`.**

 10. Rovesciata
 

> **La funzione `ReverseString` inverte una stringa. Utilizza un ciclo for per iterare sulla stringa di input in ordine inverso e concatenare ogni carattere all'output. La funzione restituisce l'output invertito**

 12. Numero di parole
 

>**La funzione `CountWords` conta il numero di parole in una stringa. Utilizza un ciclo for per iterare sulla stringa di input. Viene utilizzata una variabile booleana `isWord` per tenere traccia se il carattere corrente fa parte di una parola o meno. Se il carattere corrente è una lettera e `isWord` è false, viene incrementato il contatore `count` e `isWord` viene impostato a true. Se il carattere corrente non è una lettera, `isWord` viene impostato a false. La funzione restituisce il valore del contatore `count`, ovvero il numero di parole trovate nella stringa di input.**

 14. Capitalized
 

> **Il metodo `ConvertToCapitalized` riceve una stringa `input` e restituisce una nuova stringa in cui la prima lettera di ogni parola è maiuscola e le altre lettere sono minuscole. Per fare ciò, viene utilizzato un flag `isNewWord` per tenere traccia se il carattere attuale è il primo di una nuova parola. Se è il primo carattere di una nuova parola, viene convertito in maiuscolo e il flag viene impostato su `false`. Altrimenti, viene convertito in minuscolo. Se il carattere non è una lettera, viene aggiunto alla stringa di output e il flag viene impostato su `true` per indicare l'inizio di una nuova parola. Alla fine viene restituita la stringa di output.**

 16. Palindroma
 

> **La funzione `IsPalindrome` prende una stringa `input` e verifica se è un palindromo, ovvero se può essere letta allo stesso modo sia da sinistra che da destra. La funzione rimuove gli spazi e converte tutti i caratteri in minuscolo per semplificare il confronto tra le lettere. Successivamente, utilizza un algoritmo di "due puntatori" per confrontare il primo e l'ultimo carattere della stringa e proseguire verso il centro finché i due puntatori non si incontrano. Se la stringa è un palindromo, la funzione restituisce `true`, altrimenti restituisce `false`.**



