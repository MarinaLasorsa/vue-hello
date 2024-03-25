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