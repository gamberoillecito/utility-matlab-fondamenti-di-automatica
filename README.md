# utility-matlab-fondamenti-di-automatica

Una semplice raccolta di script che possono essere utili alla preparazione dell'esame di fondamenti di automatica

## `schemi_generali.m`

Disegna in un'unica finestra:
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
schemi_generali(G);
```
