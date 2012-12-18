Vorlesung: Analysis I*
Autor: Marius Gawrisch
Matrikelnummer: 545346
Zettel: Übungsblatt 9
Gruppe: Do. 11-13 bei V. Fromm
Vorlage: zettel

**Aufgabe 1**

**(i)**

Die Reihe  sum_{n=0}^infty frac{(n+1)^{n-1}}{(-n)^n}  ist auf Konvergenz zu untersuchen.

Für die Folgenglieder gilt  frac{(n+1)^{n-1}}{(-n)^n} = (-1)^n frac{(n+1)^{n-1}}{n^n} = (-1)^n a_n.  Nach dem Leibniz-Kriterium konvergiert die Reihe also, falls  a_n  eine Nullfolge ist.

Es gilt aber  a_n = frac{(n+1)^{n-1}}{n^n} = left(frac{n+1}{n}right)^n frac 1{n+1}.  Jede Produktreihe konvergenter Reihen konvergiert gegen das Produkt der Grenzwerte der beiden Reihen. Aus  limn left(frac{n+1}{n}right)^n = e  und  limn frac 1{n+1} = 0  folgt also  limn a_n = 0.  Damit ist das Leibniz-Kriterium erfüllt und die Reihe konvergiert.

Weiterhin ist die Reihe  sum_{n=1}^infty frac{2^nn!}{n^n}  zu untersuchen.

Wir wenden das Wurzelkriterium an, es ist ein  q in (0,1)  zu finden mit  sqrt[n]{|a_n|} <= q  für fast alle  n in NN.  

Behauptung: Das ist erfüllt für  q=frac 2 e + frac{1}{10} < 1.  

Beweis:  sqrt[n]{|a_n|} = sqrt[n]{frac{2^nn!}{n^n}} = frac 2 n sqrt[n]{n!}.  Nach Übungsblatt 8 wissen wir, dass  frac{n}{sqrt[n]{n!}}  gegen  e  konvergiert.  frac 2 n sqrt[n]{n!}  konvergiert also gegen  frac 2 e,  damit gilt nach der Definiton von Konvergenz  frac 2 n sqrt[n]{n!} <= q  für fast alle n. Damit ist die Reihe absolut konvergent.

**(ii)**

Gesucht ist der Konvergenzradius der Potenzreihe  sum_{n=0}^infty a_n x^n = sum_{n=0}^infty frac{n(n+1)}{2}x^n.  

Es gilt  q := limn left|frac{a_{n+1}}{a_n}right| = limn frac{(n+1)(n+2)}{2} cdot frac{2}{n(n+1)} = limn frac{n+2}{n} = limn (1 + frac{2}{n}) = 1.  

Nach VL beträgt der Konvergenzradius damit  1/q = 1.  

pagebreak
header

**Aufgabe 2**

**(i)**

Die ersten zehn Folgenglieder sind  1, frac 1 2, frac 1 3, frac 1 4, frac 1 6, frac 1 9, frac{1}{12}, frac{1}{16}  und  frac{1}{18}.  

Die ersten zehn Folgenglieder des Cauchy-Produktes von  sum frac{1}{2^n}  und  sum frac{1}{3^n}  sind  1, frac 1 3, frac 1 2, frac 1 9, frac 1 6, frac 1 4, frac{1}{27}, frac{1}{18}, frac{1}{12}  und  frac 1 8.  

**(i)**

Aus der Entwicklung des Cauchy-Produkts oben sieht man, dass  sum frac{1}{n_k}  gerade das Cauchy-Produkt von  sum frac{1}{2^n}  und  sum frac{1}{3^n}  ist. Dies sind beides konvergente geometrische Reihen.  sum_{n=0}^infty frac{1}{2^n} = frac{1}{1-frac 1 2} = 2  und  sum_{n=0}^infty frac{1}{3^n} = frac{1}{1-frac 1 3} = frac 3 2.  Damit gilt  sum_{k=0}^infty frac{1}{n_k} = sum_{n=0}^infty frac{1}{2^n} cdot sum_{n=0}^infty frac{1}{3^n} = 2 cdot frac 3 2 = 3.  

pagebreak
header

**Aufgabe 3**

**(i)**

Seien  (z_n)  und  (w_n)  quadratsummierbare Folgen.

Zu zeigen ist, dass die Folge  (z_nw_n)  summierbar ist, das heißt, dass  sum |z_nw_n|  konvergiert.

Da für  z_1, z_2 in CC  gilt, dass  |z_1z_2| = |z_1||z_2|  reicht es zu zeigen, dass  sum |z_n||w_n|  konvergiert.

Dafür teilen wir die Folge  (|z_n||w_n|)  in zwei Teilfolgen  a_n  und  b_n  auf. In  a_n  kommen all diejenigen Folgenglieder, für die gilt, dass  |z_n| >= |w_n|,  in  b_n  die anderen.

Damit ist  sum |z_n|^2  Majorante von  sum a_n,  zudem ist  sum |w_n|^2  Majorante von  sum b_n.  Da beide Majoranten nach Voraussetzung konvergieren, sind auch  sum a_n  und  sum b_n  konvergent. Da alle Folgenglieder positiv sind, sind die Reihen sogar absolut konvergent. In absolut konvergenten Reihen kann man die Folgenglieder aber (nach VL) beliebig vertauschen. Da  a_n  und  b_n  eine Partition der ursprünglichen Folge bilden, gilt somit  sum a_n + sum b_n = sum |z_n||w_n|. \; (z_nw_n)  ist also summierbar.  qed  

**(ii)**

Zu zeigen ist, dass die Folge  (z_n+w_n)  quadratsummierbar ist, das heißt, dass  sum |z_n+w_n|^2  konvergiert.

Da für  z_1, z_2 in CC  gilt, dass  |z_1+z_2| = |z_1|+|z_2|  ergibt sich  sum (|z_n|^2 + 2|z_nw_n| + |w_n|^2).  Wir wissen aber nach Voraussetzung und nach Teil (i), dass sowohl  sum |z_n|^2  als auch  sum |z_nw_n|  als auch  sum |w_n|^2  konvergent sind. Nach VL gilt damit, dass auch die "summierte" Reihe aus diesen 3 Einzelreihen konvergiert, damit gilt die Behauptung.  qed  
