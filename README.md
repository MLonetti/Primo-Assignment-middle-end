# Compilatori Assignement
## 1. Primo Esercizio
### - Identità Algebrica
Consiste nel riconoscere operazioni ridondanti che mostrano elemento neutro.

```python
#Esempio
x = y + 0 -> y
c = z * 1 -> z
```
Una volta riconosciuta l'operazione è necessario:
- Rimpiazzare gli usi di queste istruzioni, direttamente con l'operando non neutro
- Eliminare queste istruzioni

Per fare ciò necessitiamo del metodo ```ReplaceAllUsesWith(Instruction)```.
Come possiamo notare, necessita di un ```Istruction``` come parametro, mentre nel contesto in esame è necessario operare con un ```Value``` (Classe di cui gli operandi sono <b>Oggetti</b>)<br>
Visto che ```Istruction``` è una classe che eredita da ```Value``` possiamo comunque utilizzare questo metodo con un oggetto della classe ```Istruction```.<br>
Pertanto è necessario sostitire tutte le istanze dell'istruzione ridondante, per poi eliminare quanto rimosso.

Per fare ciò 





###- Strength Reduction
###- Ottimizzazione multi-istruzione
