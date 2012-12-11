Vorlesung: Analysis I*
Autor: Marius Gawrisch
Matrikelnummer: 545346
Zettel: Übungsblatt 8
Gruppe: Do. 11-13 bei V. Fromm
Vorlage: zettel

**Aufgabe 2**

**(i)**

Sei  (x_n)  beschränkte reelle Folge,  a := limn sup x_n  der größte Häufungspunkt,  b_n := sup \{x_k : k ≥ n\}.  

Zu zeigen:  limn b_n = a.  

  (b_n)  ist monoton fallend, da die Menge der Folgenglieder, von denen das Supremum gebildet wird, mit jedem Schritt kleiner wird. Es kann also kein größeres Element dazukommen, dass das Supremum der Menge erhöhen würde. Daraus folgt:  forall N in NN, x in RR: (b_N < x) \;=>\; (forall n > N: b_n < x).  

  (b_n)  ist nach unten durch  a  beschränkt, das heißt  forall n in NN: b_n ≥ a.  Das gilt, da in jeder beliebig kleinen Umgebung um  a  unendlich viele Folgenglieder von  (x_n)  liegen.

Aus der Tatsache, dass  a  größter Häufungspunkt ist, folgt  (*):\; forall eps > 0 \;exists N in NN \;forall n > N : x_n < a+eps.  Das lässt sich durch Kontraposition zeigen: Nehmen wir an, es gäbe ein  eps > 0,  so dass sich "hinter" jedem  N in NN  ein  x_{n_0} > a+eps  finden lässt. Dann gibt es schon unendlich viele  x_n  mit dieser Eigenschaft, da man die Annahme immer wieder für ein  N>n_0  anwenden kann. Dann gibt es aber eine *unendliche* Teilfolge, die durch  a+eps  nach unten *beschränkt* ist. Sie "erbt" außerdem die Beschränktheit nach oben von  (x_n),  die nach Voraussetzung beschränkt ist. Damit gäbe es aber einen Häufungspunkt  h ≥ a+eps,  was Widerspruch zur Definition von  a  ist. Damit gilt  (*).  

  (**)  Um nun zu zeigen, dass  (b_n)  gegen  a  konvergiert, muss man zeigen, dass man für jedes beliebige  eps > 0  ein  N in NN  finden kann, ab dem alle Folgenglieder in dem Bereich  (a-eps, a+eps)  liegen, das heißt  forall n > N: a-eps < b_n < a+eps.  

Der erste Teil der Ungleichung ist aber geschenkt, da wie oben gezeigt immer gilt:  b_n > a.  Außerdem reicht es wegen der fallenden Monotonie jeweils zu zeigen, dass  b_N < a+eps.  

Aus  (*)  wissen wir, dass es für alle  eps_1  ein  N in NN  gibt, so dass  forall n>N: x_n < a+eps_1.  Wenn aber ab einem Punkt alle Folgenglieder kleiner als ein Wert sind, dann gilt für das Supremum dieser Werte:  b_N = sup \{x_n, n ≥ N\} ≤ a+eps_1.  

Um für ein beliebiges  eps > 0  das entsprechende  N  aus  (**)  zu finden, geht man folgendermaßen vor: Man nehme ein  eps_1 in RR  mit  eps > eps_1 > 0.  Dann ist wie eben gezeigt  b_{N(eps_1)} ≤ a+eps_1.  Wegen  eps_1 < eps  gilt  b_N < a+eps.  Damit gilt mithilfe der Vorüberlegungen, dass  limn b_n = a. qed  
