# R - Primer

## Variablen

Variablen muss man sich wie kleine Container vorstellen. Sie haben ei\en Namen z.B. `x` und einen Wert (hier `5`).

| Name | Inhalt |
|------|--------|
| x    | 5      |

Eine Variable wird mit einer Zuweisung (`<-`) belegt.

*Beispiel*

'''{r}
   x <- 5
'''


*Aufgabe* 

Belege die Variable `a` mit dem Wert `7` und die Variable `b` mit `"Hallo"`.

'''{r}
  #TODO
'''


Natuerlich kann man dann mit diesen Variablen rechnen.

'''{r}
   result <- x + a
'''

*Aufgabe* 

Berechne das Produjkt vom `x` und `a`

'''{r}
   #TODO
'''

*Bonusaufgabe*

Gegeben sind die Variablen `x1` und `x2` mit Werten `3` und `"test"`.
Aufgabe ist es die variablen zu tauschen, sodass `x1` `"test"` entspricht und `x2` `3`.

'''{r}
   x1 <- 3
   X2 <- "test"
   
   #TODO

'''


## Vektoren

Vektoren (auch Arrays genannt) sind quasi Variablen deren Wert eine Liste von Werten sind.

| Name | Wert          |
|------| --------------|
| x    | [1,2,3,4,5,6] |

'''{r}
   x <- 1:6
'''

Einzelne Werte eines Vektors koennen mit `[]` ausgelesen werden.

'''{r}
   x[2]
'''

*Aufgabe*

Lies den dritten und vierten Wert von `x` aus

'''{r}
   #TODO
'''

*Bonusaufgabe*

Berechne die Anzahl an Werten, die groesser als `5` im Vektor `y <- c(10,3,6,1,0,8,9,2)` sind.

> Tipp: die Funktion `length(x)` berechnet die Laenge eines Vektors.

'''{r}
   y <- c(10,3,6,1,0,8,9,2)
   #TODO
'''


## Funktionen

Funktionen sind Methoden, die Parameter aufnehmen und einen Rueckgabewert liefern. Am Besten schauen wir uns ein Beispiel an.

'''{r}
	square <- function(x) {
    	result <- x * x
        
        return(result)
    }
    square(4)
'''

Eine Funktion bekommt Parameter, die per Komma getrennt uebergeben werden. Eine Funktion wird mit ihrem Namen und den Parametern dahinter in Klammern aufgerufen

'''{r}
	square(3)
'''

*Aufgabe*

Schreibe eine Funktion die ihre zwei Parameter addiert und das Ergebnis zurueck gibt. Berechne dann mithilfe dieser die Summe von `3` und `9`.

'''{r}
	#TODO
'''

*Bonusaufgabe (schwer)*

Schreibe eine Funktion `sum` die einen Vektor an Zahlen als Parameter aufnimmt und die Summe der Zahlen zurueck gibt.

> Tipp: Nutze eine `for`-Schleife mit der Laenge des Vektors um die einzelnen Zahlen zu durchlaufen.


'''{r}
    #TODO
    
    sum(c(8,3,10,7,2,0))
'''

---

Auf dem Cheatsheet findet ihr eine Zusammenfassung der wichtigsten Befehle, quasi ein Spickzettel.
[Download](https://raw.githubusercontent.com/rstudio/cheatsheets/master/source/pdfs/base-r.pdf)

Wenn irgendwann mal Fragen auftauchen, schreibt mir einfach. [E-Mail](mailto:b.wittmann@tum.de)
