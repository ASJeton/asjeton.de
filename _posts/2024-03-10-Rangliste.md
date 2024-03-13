---
title: Rangliste
#last_modified_at: 2024-02-13T22:02:00+01:00
categories: 
  - Rangliste
  - Regatta
tags: 
  - Regatta 
  - "2024" 
  - Rangliste 
  - Ranglisten.net
author: bernhard
classes: wide
---
Die Rangliste setzt sich aus dem Mittelwert der Ranglistenpunkte für einzelne Regatten zusammen. Es gehen 9 Wettfahrten in die Rangliste ein. Im Folgenden ist eine Beispielranglistenberechnung aufgeführt.  
Für jede Regatta git es Ranglistenpunkte in je nach verwertbaren ***Wettfahrtenfaktor m*** eingebracht werden können. Für eine 2 tägige Regatta können die Ranglistenpunkte maximal mit dem Faktor 4 eingebracht werden, was 4 Wettfahrten entspricht, aber nur wenn auch mindestens 4 Wettfahrten gesegelt wurden. Sonst entsprechend weniger.


### Regatta 1

|Platz|Boot|WF1|WF2|WF3|WF4|WF5|
|-----|----|---|---|---|---|---|
1|    A   | 1 |2 |4 | (7) | 5
2    |B   | 2 |(8)| 3|  5  | 2
...||||||
8    |H   |(8) | 7| DNF| DNC | DNC 

Ins Ziel gefahrene Boote 8.  
Ranglistenfaktor: 1,2  
Dauer: 2 Tage  
Verwertbare Wettfahrten: 4 ***m=4***  

RA = f *100 * ( ( s+1-x):s)

- ***RA*** Ranglistepunkte für eine Regatta
- ***f*** Ranglistenfaktor
- ***s*** Zahl der Boote, die in der Regatta mindestens einmal nach Absegeln der Bahn durchs Ziel gegangen sind.
- ***x*** Platz in der Regatta

RA(A)<sub>1</sub> = 1,2 * 100 * ( ( 8+1 - 1)/8) = 1,2 * 100 * (8/8) = 120  
RA(B)<sub>1</sub> = 1,2 * 100 * ( ( 8+1 - 2)/8) = 1,2 * 100 * (7/8) = 105  
RA(H)<sub>1</sub> = 1,2 * 100 * ( ( 8+1 - 8)/8) = 1,2 * 100 * (1/8) = 15  

### Regatta 2

Dauer: 3 Tage  
Verwertbare Wettfahrten: 5  ***m=5***

RA(A)<sub>2</sub> = 110  
RA(B)<sub> 2</sub> = 135  
RA(H)<sub>2</sub> = 95  

### Regatta 3

Dauer: 2 Tage  
Verwertbare Wettfahrten: 4  ***m=4***

RA(A)<sub>3</sub> = 115  
RA(B)<sub> 3</sub> = 106  
RA(H)<sub>3</sub> = 95  


### Rangliste

RL(A) = (RA(A)<sub>1</sub> * 4 + RA(A)<sub>2</sub> * 1 + RA(A)<sub>3</sub> * 4)/9 = 116,67  
RL(B) = (RA(B)<sub>1</sub> * 0 + RA(B)<sub>2</sub> * 5 + RA(B)<sub>3</sub> * 4)/9 = 133,78  
RL(H) = (RA(H)<sub>1</sub> * 0 + RA(H)<sub>2</sub> * 5 + RA(H)<sub>3</sub> * 4)/9 = 95,00  
