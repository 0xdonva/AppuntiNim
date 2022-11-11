## Tipi di dato
#### Interi
Gli _interi_ sono numeri che non hanno la parte frazionaria, vengono dichiarati in maniera molto semplice, come negli altri linguaggi.
L'unica novità è che può essere usato il carattere `_` come separatore per le migliaia, es. `var a = 10_000_000` equivale a `var a = 10000000`

#### Float
I numeri __floating point__ sono una rappresentazione _approssimata_ dei numeri reali.
Per esempio: `2.73`, `-3.14`, `5.0`, `4e7`. Da notare che si può usare la notazione scientifica per i grandi float, infatti `4e7` è la rappresentazione di `4 * 10 ^ 7`.

#### Carattere
Il tipo `char` è usato per rappresentare un singolo __carattere__ della tabella ASCII.
I `char` devono essere scritti tra due singoli apici, es. `var prova: char = 'a'`

#### Stringa
Le __stringhe__ possono essere descritte come una serie di caratteri, il loro contenuto deve essere inserito tra due doppi apici, es. `var prova: string = "prova"`

##### Caratteri speciali
In Nim ci sono parecchi caratteri che hanno significati speciali, sono usati mettendo prima il carattere di escape `\`: es. `\n` per andare a capo, `\t` per il tab, ecc.
Se si vuole evitare che in una stringa vengano letti i caratteri di escape bisogna definirla come una _raw string_, es. `echo r"some\nim\tips"`

##### Concatenazione di stringhe
Le stringhe sono oggetti mutable, tramite la funzione `add` possiamo concatenare una stringa o un char alla nostra stringa, oppure possiamo utilizzare l'operatore `&`:
```nim
var
	p = "abc"
	q = "xy"

echo "Concatenazione: ", p & q
#Qui p e q restano invariate
p.add(q)
echo "Append: ", p
```

#### Boolean
Un operatore __booleano__ è un operatore che può assumere il valore `true` o `false`.