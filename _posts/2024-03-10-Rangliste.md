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
Da es Fragen zur Berechnung der Rangliste gab, habe ich hier einmal versucht die verschiedenen Szenarien mit Beispielen zu unterlegen.
In dem vereinfachten Fall betrachten wir 3 Boote A,B und H, die an 3 Regatten teilgenommen haben und nun ihren Punkte für die Rangliste berechnen.  
Die Rangliste setzt sich aus dem Mittelwert der Ranglistenpunkte für einzelne Regatten zusammen. Es gehen 9 Wettfahrten in die Rangliste ein.   
Für jede Regatta gibt es Regattapunkte (RA) in je nach verwertbaren ***Wettfahrtenfaktor m*** eingebracht werden können. Für eine 2 tägige Regatta können die Regattapunkte maximal mit dem Faktor 4 eingebracht werden, was 4 gewerteten Wettfahrten entspricht, aber nur wenn auch mindestens 4 Wettfahrten gesegelt wurden. Sonst entsprechend weniger.  
Diese Regeln kann man in den [Ordnungen für Regatten](https://www.dsv.org/app/uploads/dsv-ordnungen-fur-regatten-ab-01012024.pdf) nachlesen.

#### Ranglistenpunkte
$$RA = f * 100  * \frac{s+1-x}{s}$$

- ***RA*** Regattapunkte für eine Regatta
- ***f*** Ranglistenfaktor
- ***s*** Zahl der Boote, die in der Regatta mindestens einmal nach Absegeln der Bahn durchs Ziel gegangen sind.
- ***x*** Platz in der Regatta

Im folgendem meint RA(Boot)<sub>Regatta</sub> die *Ranglistenpunkte* für ein *Boot* in einer *Regatta*.

### Regatta 1

|Platz|Boot|WF1|WF2|WF3|WF4|WF5|
|-----|----|---|---|---|---|---|
1|    A   | 1 |2 |4 | (7) | 5
2    |B   | 2 |(8)| 3|  5  | 2
...||||||
8    |H   |(8) | 7| DNF| DNC | DNC 

Ins Ziel gefahrene Boote: ***s=8***  
Ranglistenfaktor: ***f=1,2***  
Dauer: 2 Tage  
Verwertbare Wettfahrten: ***m&le;4***  

$$RA(A)_1 = 1,2 * 100 * \frac{8 + 1 - 1}{8} = 1,2 * 100 * \frac{8}{8} = 120$$    
$$RA(B)_1 = 1,2 * 100 * \frac{8 + 1 - 2}{8} = 1,2 * 100 * \frac{7}{8} = 105$$  
$$RA(H)_1 = 1,2 * 100 * \frac{8 + 1 - 8}{8} = 1,2 * 100 * \frac{1}{8} = 15$$   

### Regatta 2

Dauer: 3 Tage  
Verwertbare Wettfahrten: ***m&le;5***

RA(A)<sub>2</sub> = 110  
RA(B)<sub> 2</sub> = 135  
RA(H)<sub>2</sub> = 95  

### Regatta 3

Dauer: 2 Tage  
Verwertbare Wettfahrten: ***m&le;4***

RA(A)<sub>3</sub> = 115  
RA(B)<sub> 3</sub> = 106  
RA(H)<sub>3</sub> = 95  


### Rangliste
Die Punkte für die Rangliste setzen sich aus den Regattapunkten (RA<sub>i</sub>) für die Ranglistenregatten die mit einem Faktor $$n_i=[0\dots m]$$ eingehen, wobei $$\sum{n_i}=9$$.
Es werden insgesamt 9 Wertungen eingebracht, aus denen der Mittelwert gebildet wird.

$$RL=\frac{\sum{n_i*RA_i}}{9}$$

Aus den Ergebnissen ergeben sich dann folgende Ranglistenpunkte:  

RL(A) = (**4** * RA(A)<sub>1</sub> + **1** * RA(A)<sub>2</sub> + **4** * RA(A)<sub>3</sub>)/**9** = 116,67  
RL(B) = (**0** * RA(B)<sub>1</sub> + **5** * RA(B)<sub>2</sub> + **4** * RA(B)<sub>3</sub>)/**9** = 133,78  
RL(H) = (**0** * RA(H)<sub>1</sub> + **5** * RA(H)<sub>2</sub> + **4** * RA(H)<sub>3</sub>)/**9** = 95,00  
