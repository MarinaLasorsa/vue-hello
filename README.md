# VUE

## INTRODUCTION

- In Vue, è possibile dichiarare direttamente in Javascript ciò che poi vedremo dall'HTML. 
Inoltre, mantiene aggiornate nel DOM le informazioni dichiarate anche dopo che vengono cambiate in Javascript.

- Per creare componenti di Vue, si raccomanda di includere il codice Javascript, il template HTML e lo stile CSS del componente in un file SFC (Single File Component)

- I componenti di Vue si possono scrivere con API Options o Composition. Noi utilizzeremo l'API Options.
(Cosa vuol dire API?)

- Con l'API Options, rendiamo la logica attraverso le opzioni contenute in un oggetto. Queste opzioni sono data, methods e mounted. 
Le varie proprietà definite in data possono essere richiamate e utilizzate in methods e mounted tramite funzioni this.nomeproprietà.

- Con l'API Composition, scrivi tutto il codice in un file script che importa varie funzioni, utilizzabili grazie all'attributo setup. (non mi è super chiaro...)

- Per creare applicazioni complete è meglio l'API composition, è più flessibile e customizzabile, ma per i principianti e chi vuole solo utilizzare Vue per ottimizzare il proprio progetto, è più semplice l'API Options.


## TEMPLATE SYNTAX

- I template di Vue sono utilizzabili in HTML e legano il DOM all'opzione data dichiarata in Javascript.

- L'esempio più basico è la sintassi "Mustache", cioé la doppia parentesi graffa. 
Nelle parentesi viene inserito il nome della proprietà definita in data, che rimarrà sempre aggiornata.

- Le informazioni in data vengono interpretate dalla "Mustache" come testo, se si vuole inserire del codice HTML è necessario utilizzare la direttiva v-html="proprietà", e non la doppia parentesi graffa.

- Non si può utilizzare la "Mustache" negli attributi HTML, è quindi necessario utilizzare la direttiva v-bind.
Per esempio: v-bind:id="proprietà" per dare all'elemento html l'id definito dalla proprietà inserita.
    - La direttiva v-bind si può accorciare in :id="proprietà"
    - Se la proprietà ha lo stesso nome dell'attributo, si può ulteriormente accorciare in :id (o v-bind:id)
    - Se la proprietà inserita contiene più attributi, si possono abbinare allo stesso elemento usando v-bind="proprietàDiAttributi", senza il :

- La direttiva v-on ascolta gli eventi del DOM, per esempio il click: v-on:click="proprietà".
    - La direttiva v-on si può accorciare in @click="proprietà".

- Gli argomenti delle direttive (ad es. id in v-bind e click in v-on) possono essere espressioni Javascript, in quel caso sono delimitate da parentesi quadre.

- Per dare limiti o modifiche alle direttive si utilizza il punto dopo l'argomento, con il modificatore che vogliamo applicare, ad es. @submit.prevent="proprietà" (non mi è super chiaro neanche questo)


