Vorlesung: Analysis I*
Autor: Marius Gawrisch
Matrikelnummer: 545346
Zettel: Übungsblatt 6
Gruppe: Do 11-13, Fromm
Vorlage: zettel

**Aufgabe 1**

**(i)**

pagebreak
header

**Aufgabe 2**

**(i)**

Sei  (x_n)  beschränkte reelle Folge.  a := limn sup x_n  ist der größte Häufungspunkt.  b_n = sup \{x_k : k ≥ n\}.  

Zu zeigen:  limn b_n = a.  

Ein Wert ist genau dann Häufungspunkt einer Folge, wenn es eine Teilfolge gibt, die gegen diesen Wert konvergiert. Es gibt also eine Teilfolge von  (x_n),  die gegen  a  konvergiert. Sei  (y_n)  eine solche Teilfolge.

Sei  (z_n)  die (möglicherweise endliche) Teilfolge von  (x_n),  die alle Folgenglieder enthält, für die gilt:  x_n ≥ a.  Sei  (a_n)  die "Vereinigung" von  (y_n)  und  (z_n).  (sollte hier auf Ebene der Filterfolge argumentieren.)  (z_n)  war aber entweder endlich, dann ist  limn a_n = limn y_n = a.  War  (z_n)  unendlich, dann konvergiert  (z_n)  gegen  a.  (Warum muss  (z_n)  konvergieren? Beschränktheit ist leicht, aber  (z_n)  muss nicht monoton sein.) Würde  (z_n)  gegen ein  b neq a  konvergieren, dann wäre  b  Häufungspunkt von  (x_n). \; b  wäre dann aber  > a,  da alle  z_n  nach Definition  > a  sind. Dann wäre  b  größerer Häufungspunkt als  a,  was Wiederspruch zur Annahme ist. Wenn aber zwei konvergente Folgen mit demselben Grenzwert vereinigt werden, dann hat die resultierenden Folge auch diesen Grenzwert (ist das so?).

Sei außerdem  (c_n)  eine Teilfolge von  (b_n),  die durch dieselbe "Filterfolge" entstanden ist. Nach Konstruktion konvergiert  (c_n)  gegen  a. \; (b_n)  ist konvergente Folge. Damit auch  (b_n),  da der Grenzwert einer konvergenten Folge immer mit dem Grenzwert jeder Teilfolge übereinstimmt.
