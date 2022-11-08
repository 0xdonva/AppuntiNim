Nim è un linguaggio di programmazione statico, questo vuol dire che deve essere dichiarato prima il tipo di dato che viene assegnato ad una variabile.
In Nim esiste un'ulteriore distinzione tra variabili:
- `var`: usato per le variabili che cambiano il proprio valore durante l'esecuzione del programma.
- `const`: usato per le costanti, il valore deve esser conosciuto a tempo di compilazione e non cambia durante l'esecuzione.
- `let`: usato per le variabili di cui non conosciamo il valore a tempo di compilazione ma può essere assegnata ad un valore una volta.
```nim
var a
const b = 32
let c
c = 3
```
