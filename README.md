# utility-matlab-fondamenti-di-automatica

Una semplice raccolta di script che possono essere utili alla preparazione dell'esame di fondamenti di automatica

## `schemi_generali.m`

Disegna in un'unica finestra:

 **I grafici in blu sono relativi alla funzione in anello aperto, quelli in rosso a quella in anello chiuso (vedi la sezione Uso per altri dettagli)**
 
  - Luogo delle radici diretto
  - Luogo delle radici inverso
  - Diagramma di Bode
  - Diagramma di Nyquist
  - Risposta al gradino
  - Risposta all'impulso
  - Risposta alla rampa
  - Tabella di Routh (il codice utilizzato è preso da [qui](https://it.mathworks.com/matlabcentral/fileexchange/17483-routh-hurwitz-stability-criterion))

### Uso
```
s = tf('s');
G = 1/s; %la vostra funzione di trasferimento
schemi_generali(G); disegna gli schemi descritti sopra
schemi_generali(G, [1, 4]); disegna gli schemi descritti sopra e gli schemi delle funzioni in ciclo chiuso con guadagno che varia da 1 a 4 incrementando di 1 ad ogni passo
schemi_generali(G, [1, 4], 0.5); come sopra ma il guadagno viene incrementato di 0.5 ad ogni passo
```
