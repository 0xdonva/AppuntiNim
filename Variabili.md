Nim è un linguaggio di programmazione statico, questo vuol dire che deve essere dichiarato prima il tipo di dato che viene assegnato ad una variabile.

## Tipi di variabili
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

## Assegnazione di un tipo
Per assegnare ad una _variabile_ un tipo di [[dato]] si può fare in due modi:
- _Manuale_: `var <nome>: <tipo> = <valore>` oppure `var <nome>: <tipo>`
- _Automatico_: `var <nome> = <valore>

### Assegnazione multipla
In Nim possono essere assegnato simultaneamente più variabili, la cosa importante è mantenere l'_indentazione corretta_.
```nim
var
	d = -11
	e = "Ciao"
	f = 123.643
```