# Introduction to TypeScript
Sito ufficiale di [Typescript](https://www.typescriptlang.org)

[Wiki](https://github.com/Microsoft/TypeScript/wiki) su github

## String

var brand: string = 'Chevrolet';

Si possono usare le virgolette singole o doppie. Si possono definire string di testo multi riga con il supporto di text 
interpolation usando variabili placeholder e backticks ( `` , per scriverle alt + 96, sono diverse da '')

Es

var brand: string = 'Chevrolet';

var message: string = `Today it's a happy day! I just bought a new 
${brand} car`;

sul file .md, con backtick evidenza il testo così: `test`

## The let keyword

non usare var per dichiarare le variabili: la ragione è che in ES5 ha solo ambito funzionale, cioè, una variabile è 
unica nel contesto di una funzione.

function test() { <br>
    var x;<br>
}

Non può esserci nessun'altra variabile dichiarata come x in questa funzione. Se ne dichiariamo un'altra, allora la stiamo
effettivamente re definendo. ci sono casi in cui lo scoping non è applicabile come i loops

## The const keyword
Indica che quella variabile non dovrebbe cambiare 

## Number
const age: number= 7;
const height: number = 5.6;

## Boolean
const isZeroGreaterThanOne: boolean= false;

## Array
const brands: string[] = ['1', '2', '3'];
const ages: number[] = [1, 2, 3];

## Dynamic typing with no type
let distance: any;

## Custom types
type Animal = 'Cheetah' | 'Lion';
const animal: Animal = 'Cheetah';

In pratica è un tipo con un finito numero permesso di valori.

const animal: Animal = 'Turtle'; -> errore: Type 'Turtle' is not assignable to type 'Animal'

## Enum
Il tipo enum è un insieme di valori numerici unici che rappresentiamo dall'assegnamento di un nome user-friendly a 
ognuno. Incominciano da zero se non ci sono espliciti numeri assegnati.

enum Brands { Ford, Tesla, Ferrari };

Se si inizia con un numero, quelli dopo sono incrementali
enum Brands2 {Tesla = 1, GMC};
GMC avrà il valore 2

Possiamo guardare al nome del membro mappato con il valore numerico

const myCar: string = Brands[1];
