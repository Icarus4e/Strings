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
 
> **La funzione `ConvertToUppercase` converte ogni lettera minuscola in maiuscola nella stringa di input, lasciando intatti tutti gli altri caratteri. La funzione utilizza un loop for per iterare attraverso ogni carattere della stringa di input e utilizza la funzione `ToUpper` per convertire ogni lettera minuscola in maiuscola. Infine, la funzione restituisce la stringa convertita**

![Maiuscolo](https://user-images.githubusercontent.com/113766707/232234417-5be3fdc0-36b3-47ee-a331-178f11cc6852.png)

 2. Minuscola

> **La funzione `ConvertToLowercase` converte ogni lettera maiuscola in minuscola nella stringa di input, lasciando intatti tutti gli altri caratteri. La funzione utilizza un loop for per iterare attraverso ogni carattere della stringa di input e utilizza la funzione `ToLower` per convertire ogni lettera maiuscola in minuscola. Infine, la funzione restituisce la stringa convertita.**

![Minuscolo](https://user-images.githubusercontent.com/113766707/232234397-116c4633-1579-4b83-a319-d204c62b97c4.png)

 3. Caratteri Alfabetici
 
> **La funzione `IsOnlyLetters` verifica se la stringa di input è composta solo da lettere alfabetiche. La funzione utilizza un loop foreach per iterare attraverso ogni carattere della stringa di input e utilizza la funzione `char.IsLetter` per verificare se il carattere è una lettera alfabetica. Se un carattere non è una lettera alfabetica, la funzione restituisce `false` per indicare che la stringa non contiene solo lettere. Se tutti i caratteri della stringa sono lettere, la funzione restituisce `true`.**

![OnlyLetters](https://user-images.githubusercontent.com/113766707/232234463-cfafebfd-2b47-48b2-8f83-9a313c058fd4.png)

 4. Numero di lettere
 
> **La funzione `CountLetters` conta il numero di lettere presenti nella stringa di input. La funzione scorre ogni carattere della stringa di input e, se il carattere è una lettera dell'alfabeto (cioè se si trova nell'intervallo 'A'-'Z' o nell'intervallo 'a'-'z'), incrementa un contatore di lettere. Alla fine, la funzione restituisce il valore del contatore.**

![CountLetters](https://user-images.githubusercontent.com/113766707/232234476-4ab31d38-8d9b-41f8-a0e4-69a9ea817203.png)

 5. Alfanumerici
 
> **La funzione `IsAlphanumeric` controlla se la stringa di input contiene solo caratteri alfanumerici. La funzione scorre ogni carattere della stringa di input e, se il carattere non è una lettera dell'alfabeto (cioè non si trova nell'intervallo 'A'-'Z' o nell'intervallo 'a'-'z') e non è un numero (cioè non si trova nell'intervallo '0'-'9'), restituisce `false`. Se alla fine della scansione tutti i caratteri della stringa sono alfanumerici, la funzione restituisce `true`.**

![Alfanumerico](https://user-images.githubusercontent.com/113766707/232234487-faea7242-2215-4161-9a43-a03281eb7f36.png)

 6. Rovesciata
 
> **La funzione `ReverseString` inverte una stringa. Utilizza un ciclo for per iterare sulla stringa di input in ordine inverso e concatenare ogni carattere all'output. La funzione restituisce l'output invertito**

![Reverse](https://user-images.githubusercontent.com/113766707/232234500-2aa11722-ad7b-4a89-8425-dd865f6bbbd8.png)

 7. Numero di parole
 
>**La funzione `CountWords` conta il numero di parole in una stringa. Utilizza un ciclo for per iterare sulla stringa di input. Viene utilizzata una variabile booleana `isWord` per tenere traccia se il carattere corrente fa parte di una parola o meno. Se il carattere corrente è una lettera e `isWord` è false, viene incrementato il contatore `count` e `isWord` viene impostato a true. Se il carattere corrente non è una lettera, `isWord` viene impostato a false. La funzione restituisce il valore del contatore `count`, ovvero il numero di parole trovate nella stringa di input.**

![CountWords](https://user-images.githubusercontent.com/113766707/232234510-878cbe1b-3a53-4725-8a8b-aa31cf1037ee.png)

 8. Capitalized
 
> **Il metodo `ConvertToCapitalized` riceve una stringa `input` e restituisce una nuova stringa in cui la prima lettera di ogni parola è maiuscola e le altre lettere sono minuscole. Per fare ciò, viene utilizzato un flag `isNewWord` per tenere traccia se il carattere attuale è il primo di una nuova parola. Se è il primo carattere di una nuova parola, viene convertito in maiuscolo e il flag viene impostato su `false`. Altrimenti, viene convertito in minuscolo. Se il carattere non è una lettera, viene aggiunto alla stringa di output e il flag viene impostato su `true` per indicare l'inizio di una nuova parola. Alla fine viene restituita la stringa di output.**

![Capitalized](https://user-images.githubusercontent.com/113766707/232234519-6b8c4464-e7fc-4ce2-ba1e-b91cbfc6ae5f.png)

 9. Palindroma
 
> **La funzione `IsPalindrome` prende una stringa `input` e verifica se è un palindromo, ovvero se può essere letta allo stesso modo sia da sinistra che da destra. La funzione rimuove gli spazi e converte tutti i caratteri in minuscolo per semplificare il confronto tra le lettere. Successivamente, utilizza un algoritmo di "due puntatori" per confrontare il primo e l'ultimo carattere della stringa e proseguire verso il centro finché i due puntatori non si incontrano. Se la stringa è un palindromo, la funzione restituisce `true`, altrimenti restituisce `false`.**

![Palindromo](https://user-images.githubusercontent.com/113766707/232234530-6998b5ec-f48a-4b6a-bf4b-aeb0103cf5f0.png)

