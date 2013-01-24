Titel: Analysis I*
Vorlage: math

# Okt 30. Angeordneter Körper

Def..  QQ := \{frac p q : p,q in ZZ, q neq 0\}, \; frac p q = frac r s :<=> ps=qr, \; frac p q + frac r s := frac{ps+rq}{qs}, \; frac p q cdot frac r s := frac{pr}{qs}, \; q,s >0 : frac p q < frac r s :<=> ps < qr.  

Bmk..  (QQ, <=)  ist geordnete Menge.

Def (Anordnungsaxiom). Körper  KK  heißt **angeordnet**, falls eine Teilmenge  KK_+ subset KK  folgendes erfüllt: (A1) Für jedes  a in KK  gilt *entweder*  (a in KK_+)  *oder*  (-a in KK_+)  *oder*  a=0.  (A2) Für alle  a,b in KK_+  gilt:  a+b in KK_+  *und*  a cdot b in KK_+. \; KK_+  werden auch die **positiven** Elemente von  KK  genannt.

Def..  (a>0) :<=> a in KK_+.  

Def..  KK  Körper,  a,b in KK. \; a>b :<=> (a-b)>0.  

(...)

# Nov 1. Supremumseigenschaft der reellen Zahlen

Satz.. Es gibt keine rationale Zahl  x in QQ  mit  x^2 = 2.  

(Reelle Zahlen:  RR supset QQ. \; +, cdot, <=  auf  QQ  wie bei  QQ.)  

Def.. Menge mit Ordnungsrelation gegeben.. (i) Eine Teilmenge  M neq varnothing  heißt **nach oben beschränkt** falls es ein Element  s  (nicht notwendigerweise in  M)  gibt mitt:  forall x in M: x <= s..  (ii) Analog **nach unten beschränkt**.. (iii)  s  heißt **Supremum von**  M,  falls  s  *kleinste* obere Schranke ist.. (iv) **Infimum** analog.. (v) **Maximum**, falls Supremum  s in M..  (vi) Analog **Minimum**.

(Vollständigkeitsaxiom bringt die reellen Zahlen)

Satz..  NN subset RR  ist unbeschränkt.

**Satz von Eudoxos**.. Sei  x in RR, \; x > 0.  Dann existiert  n in NN  mit  frac 1 n < x.  

# Nov 6. Existenz der *n*-ten Wurzel, Intervallschachtelung

**Existenz der n-ten Wurzel**..  n in NN, n >= 1, a in RR, a > 0.  Für jedes  a  gibt es  x in RR, x > 0  mit  x^n = a.  Schreibweise:  sqrt[n] a := a^{frac 1 n} := x.  

Satz.. Die rationalen Zahlen liegen in den reellen Zahlen dicht, das heißt für je zwei reelle Zahlen  x,y in RR  mit  x<y  existiert ein  a in QQ  mit  x<a<y.  

Def.. Seien  a,b in RR, \; a <b.  Dann  [a,b] := \{x in RR : a <= x <= b\}  heißt **abgeschlossenes Intervall**..  (a,b) := \{x in RR : a < x <b\}  **offenes Intervall**.. Halboffene Intervalle  (a, b]  und  [a,b)..  Sei  I  Intervall. Dann heißt  |I| := (b-a)  **Länge des Intervalls**.. **Intervallschachtelung** ist Folge von Intervallen  I_0, I_1, I_2, ...  mit  I_{n+1} sse I_n  und zu jedem  eps > 0  gibt es ein  n in NN  mit  |I_n| < eps.  

**Intervallschachtelungsprinzip**.. Für jede Intervallschachtelung *abgeschlossener* Intervalle existiert genau ein Element im Durchschnitt:  \{x\} = bigcap_{n=0}^infty I_n.  

# Nov 8. Abzählbarkeit, komplexe Zahlen

Bmk.. (i) Allgemein gilt für Intervalle  I_n  mit  I_n sse I_{n+1}  immer  bigcap_{n=0}^infty I_n neq varnothing  (?).. (ii) Supremumseigenschaft und Intervallschachtelung sind äquivalent.. (iii) Intervallschachtelungsprinzip gilt nicht für offene/halboffene Intervalle  I_n.  

Def.. Eine unendliche Menge heißt **abzählbar**, wenn es eine *bijektive* von den natürlichen Zahlen in diese Menge gibt.

Satz.. Die Menge der reellen Zahlen ist nicht abzählbar.

Def..  CC:=\{a+ib : a,b in RR\} cong RR^2.  

Satz..  CC  ist eine Körper mit  0+i0  als Null und  1+i0  als Eins. Das Reziproke (multiplikativ Inverse) von  a+ib neq 0  ist gegeben durch  frac{1}{a+ib} := frac{a-ib}{a^2+b^2}.  

# Nov 13. Konvergenz

Satz.. (1) Quadratwurzeln existieren für jede komplexe Zahl.  +- z = +- sqrt w = +- sqrt r (cos frac phi 2 + i sin frac phi 2).  (2) Erhalten somit immer Lösung einer quadratischen Gleichung. (3) (Fundamentalsatz der Algebra) Jedes nicht-konstante Polynom mit Koeffizienten in  CC  besitzt eine Nullstelle.

Def.. Eine **Folge**  (a_n)_{n in NN}  ist Abbildung  a : NN to CC. a_n in CC  mit  a_n := a(n).  Eine Folge  (a_n)_{n in NN}  heißt **konvergent**, falls es eine komplexe Zahl  a in CC  gibt mit folgender Eigenschaft: Für jedes  eps > 0  gibt es ein  N in NN  mit: für jedes  n > N  gilt:  |a_n - a| < eps. \; a  heißt dann **Grenzwert** der Folge. Man sagt:  (a_n)  konvergiert gegen  a  oder:  limn a_n = a.  

# Nov 15. Grenzwerte

Bmk..  eps > 0. \; \triangle(a, eps) := \{z in CC : |z-a| < eps \}  "Epsilon-Scheibe".  (a_n)_{n in NN}  konvergiert gegen  a in CC,  gdw.  exists N in NN : forall n > N  gilt  a_n in \triangle(a, eps).  

Satz..  (a_n)_{n in NN}  konvergiert gegen  a in CC  gdw.  (a_n - a)_{n in NN}  eine **Nullfolge** ist, d.h. gegen  0 in CC  konvergiert. (1)  s in QQ_+  gilt  limn 1/n^s = 0.  (2) Für  a > 0  gilt  limn sqrt[n]{a} = 1, \; (n ≥ 1).  (3)  limn sqrt[n]{n} = 1, \; (n≥1).  (4)  z in CC, |z| < 1 : limn z^n = 0.  (5)  z in CC, s in Q_+, |z| > 1 : limn n^s/z^n > 0.  

Satz.. Der Limes ist eindeutig bestimmt, wenn er existiert. Beweis Forster S. 34.

# Nov 15. Abzählbarkeit (Übung)

Satz.. Ist  M  unendlich und es gibt *surjektive* Abildung  g: NN to M,  dann ist  M  abzählbar.

Satz.. Ist  M  abzählbar, und ist  N sse M  unendlich, dann ist auch  N  abzählbar.

Satz.. Eine unendliche Vereinigung abzählbar unendlicher Mengen ist abzählbar.

Satz.. Eine disjunkte abzählbar unendliche Vereinigung nichtleerer endlicher Mengen ist abzählbar.

# Nov 20. Rechenregeln für Grenzwerte

Def.. Sei  (a_n)_{n in NN}  eine Folge. (1) Sie heißt **divergent**, wenn sie nicht konvergiert. (2) Falls für eine reelle Folge gilt: Für jedes  C>0  gibt es ein  N in NN,  so dass für alle  n in NN, n ≥ N  gilt:  a_n > C,  dann schreibt man  limn a_n = + infty.  Analog  limn a_n = - infty.  

Satz.. Eine reelle Folge  (a_n)_{n in NN}  konvergiert gegen  + infty,  gdw. die Folge  (1/a_n)_{n in NN}  ab einem gewissen Folgenglied definiert ist und positiv ist und  limn 1/a_n = 0.  

Satz.. Seien  (a_n)_{n in NN}, (b_n)_{n in NN}  konvergente Folgen,  a, b  deren Grenzwerte. (1) Dann sind  (a_n+b_n)_{n in NN}, (a_n cdot b_n)_{n in NN}  ebenfalls konvergent,  (a+b)  bzw.  (a cdot b)  ihre zugehörigen Grenzwerte. (2) Ist  b neq 0,  so gibt es  N_0 in NN,  s.d.  b_n neq 0  falls  n ≥ N_0  und  limn 1/b_n = 1/b = 1/limn b_n.  (3) Dann sind auch  (|a_n|), (Re a_n), (Im a_n), (overline a_n)  konvergent und es gelten  limn |a_n| = |a|, limn (Re a_n) = Re a,  usw. Beweis Forster S. 34--36.

Satz..  (a_n)_{n in NN}, (b_n)_{n in NN}  reelle, konvergente Folgen. Es sei  a_n ≤ b_n  für  n ≥ N  mit  N in NN.  Dann folgt  limn a_n ≤ limn b_n.  Beweis Forster S. 37.

Folgerung.. (1) Gilt für konvergente Folge  (a_n)_{n in NN},  dass  a_n in [c, d],  falls  n ≥ N.  Dann ist  limn a_n in [c, d].  (2) Ist  (c_n)  eine weitere beliebige Folge und  a_n ≤ c_n ≤ b_n  für  n ≥ N  und  limn a_n = limn b_n = a = b.  Dann ist  (c_n)  konvergent und  limn c_n = a.  

# Nov 22. Monotonie

Satz..  a_n ≤ c_n ≤ b_n, \; limn a_n = limn b_n = a.  Dann ist  (c_n)  eine konvergente Folge und  limn c_n = a.  

Def.. Eine *reelle* Folge  (a_n)_{n in NN}  heißt **monoton wachsend** falls gilt:  a_{n+1} ≥ a_n  für alle  n in NN,  **monoton fallend**, falls  a_{n+1} ≤ a_n  für  n in NN.  Gilt sogar  a_{n+1} > a_n (a_{n+1} < a_n)  für alle  n in NN,  dann heißt sie **streng monoton wachsend (fallend)**.

Satz.. Eine *beschränkte*, monoton wachsende Folge ist konvergent. Mit  A=\{a_n : n in NN\}  gilt:  limn a_n = sup A.  Ist  (a_n)  monoton fallend und beschränkt, so gilt  limn a_n = inf A.  

# Nov 22. Optimale Schranke

Def..  a in A sse RR  heißt **Schranke** von  A,  wenn  a  untere oder obere Schranke von  A  ist.  a  heißt **optimale Schranke**, wenn  a  kleinste obere oder größte untere Schranke von  A  ist.

# Nov 27. Euler-Zahl, Häufungspunkt

Def.. Der Grenzwert der Folge  a_n = (1+frac 1 n)^n  heißt **Euler-Zahl** und wird mit  e:= limn (1+frac 1 n)^n  bezeichnet.

Def..  (a_n)_{n in NN}  sei Folge (in  CC).  Dann heißt ein  h in CC  **Häufungspunkt**, falls für beliebiges  eps > 0  die Menge  \{n : a_n in triangle(h, eps)\}  unendlich ist, d.h. in jeder Epsilon-Scheibe von  h  liegen unendlich viele Folgenglieder von  (a_n).  

Def.. Für eine Folge  (a_n)_{n in NN}  und eine Folge  (n_k)_{k in NN}  *natürlicher* Zahlen, die streng monoton wächst, bezeichnet man  (a_{n_k})_{k in NN}  als **Teilfolge** von  (a_n).  

**Satz von Bolzano-Weierstraß**.. (1) Ist  (a_n)_{n in NN}  eine beschränkte Folge, so besitzt sie einen Häufungspunkt. (2) Ist  (a_n)_{n in NN}  reell und beschränkt, so gibt es einen kleinsten sowie einen größten Häufungspunkt,  h_*  und  h^*.  Es gilt:  NN setminus \{n : h_* - eps < a_n < h^* + eps\}  ist endlich für jedes  eps > 0.  

Def..  h_*  heißt **Limes inferior** der Folge,  h^*  heißt **Limes superior**.

# Nov 29. Cauchy-Folge, Reihe

Def.. Sei  (a_n)  reelle Folge. Dann ist  limn sup a_n := infty  für nach oben unbeschränkte  a_n,  sonst  limn sup a_n := limn (sup \{a_k : k ≥ n\}). \; limn inf a_n  analog.

Def.. Eine Folge  (a_n)  heißt **Cauchy-Folge**, falls gilt: Für jedes  eps > 0  gibt es ein  N in N,  so dass für alle  m, n in NN, \; m, n ≥ N  gilt:  |a_n-a_m| < eps.  

**Cauchy-Kriterium**.. Eine Folge  (a_n)  in  CC  ist konvergent genau dann, wenn sie eine Cauchy-Folge ist.

Bmk.. Das Cauchy-Kriterium folgt aus Supremumeigenschaft von  RR,  beide Eigenschaften sind sogar äquivalent.

Def.. Sei  (a_n)  Folge in  CC  und  s_n := sum_{k=0}^n a_k.  Die Folge  (s_n)  heißt **Reihe**, die  a_n  **Glieder der Reihe**, die  s_n  **Partialsummen**. Eine Reihe heißt **konvergent**, falls die Folge  (s_n)  konvergiert. Dann wird der Grenzwert mit  sum_{k=0}^infty a_k := limn s_n  bezeichnet. (Achtung: Mit  sum_{k=0}^infty a_k  wird gewöhnlich auch die *Reihe*  (s_n)  bezeichnet.)

Bsp.. Für ein  z in CC  heißt  sum_{k=0}^infty z^k  die [**geometrische Reihe**](http://www.proofwiki.org/wiki/Geometric_Series). Für  z neq 1  ist  s_n = sum_{k=0}^n z^k = frac{1-z^{n+1}}{1-z}.  Also für  |z| < 1 : sum_{k=0}^infty z^k = frac 1 {1-z}.  

# Dez 4. Konvergenzkriterien

Satz.. Sei  sum^infty_{k=0} a_k  konvergent und  k_0 in NN.  Dann sich auch  sum^infty_{k=k_0} a_k  und  sum^infty_{k=-k_0} a_k  konvergent. Anders gesagt: Das Hinzufügen oder Entfernen *endlich vieler* Summanden ändert nichts an der Konvergenz der Reihe (am Grenzwert möglicherweise schon).

Bsp..  sum^infty_{k=1} frac 1 {k(k+1)}; \; s_n = sum^n_{k=1} frac 1 {k(k+1)} = 1 - frac 1 {k+1}, \; limn s_n = 1 - limn frac 1 {n+1} = 1.  

Bsp..  sum^infty_{k=0} (-1)^k  divergent.  s_n = 1  für  n  ungerade,  s_n = 0  sonst.

[**Harmonische Reihe**.](http://www.proofwiki.org/wiki/Sum_of_Reciprocals_is_Divergent)
  \quad sum_{k=1}^infty frac 1 k = infty.  

Satz..  sum_{k=0}^infty a_k  konvergiert genau dann, wenn für jedes  eps > 0  existiert ein  N in NN,  so dass für  n > m ≥ N : |sum_{k=m+1}^n a_k| < eps.  

Folgerung.. [1)](http://www.proofwiki.org/wiki/Terms_in_Convergent_Series_Converge_to_Zero) Konvergiert  sum_{k=0}^infty a_k  so ist die Folge ihrer Glieder  (a_k)_{k in NN}  eine Nullfolge. 2) Das Abändern *endlich vieler* Reihenglieder ändert nichts am Konvergenzverhalten der Reihe.

[**Majorantenkriterium**](http://www.proofwiki.org/wiki/Comparison_Test)..
Sei  |a_n| ≤ b_n  für alle  n in NN.  Wenn  sum_{k=0}^infty b_k  konvergiert, so konvergiert auch  sum_{k=0}^infty a_k.  Man sagt:  (b_n)  ist (konvergierende) Majorante von  (a_n).  

Satz.. Sei  a_n ≥ 0  für alle  n in NN.  Dann konvergiert  sum_{k=0}^infty a_k  genau dann, wenn ihre Partialsummenfolge beschränkt ist.

[**Hyperharmonische Reihe**](http://www.proofwiki.org/wiki/P-Series_Converge_Absolutely)..
  sum_{k=1}^infty k^{-p}  divergiert für  0 < p ≤ 1.  Sie konvergiert absolut für  p > 1.  

Bmk..  \zeta (s) := sum_{k=1}^infty frac 1 {k^s}  (der Grenzwert einer konvergenten hyperharmonischen Reihe) heißt **Riemannsche Zetafunktion** und ist höchst rätselhaft.

[**Leibniz-Kriterium**](http://www.proofwiki.com/wiki/Alternating_Series_Test)..
Sei  (a_n)  eine monoton fallende Nullfolge, dann konvergiert die alternierende Reihe  sum_{k=0}^infty (-1)^k a_k.  

Bmk..  s_{2n+1} ≤ s ≤ s_{2n}  für  n in NN  beliebig.

# Dez 6. Absolute Konvergenz, Produktreihe

**Riemannscher Umordnungssatz**..
Sei  (a_n)_{n in NN}  Nullfolge positiver Zahlen mit  sum_{n=0}^{infty} a_n = infty.  Dann gibt es für jedes  lam in RR cup \{-infty, +infty\}  eine Bijektion  sigma : NN to NN,  so dass  sum_{n=0}^infty (-1)^{sigma(n)}a_{sigma(n)} = lam.  

Def.. Eine Reihe  sum a_k  heißt **absolut konvergent**, falls  sum |a_k|  konvergiert.

Bmk.. Wenn  sum |a_k|  konvergiert, dann konvergiert auch  sum a_k.  

Satz.. Sei  sum a_k  absolut konvergent. Dann ist für jede Bijektion  sigma : NN to NN  auch die umgeordnete Reihe  sum_{k=0}^infty a_{sigma(k)}  absolut konvergent mit dem Grenzwert  sum a_k.  

Satz..  sum(a_k+b_k) = sum a_k + sum b_k. quad sum(Re a_k) = Re (sum a_k). quad sum Im a_k = Im sum a_k. quad sum overline{a_k} = overline{sum a_k}.  

Def.. Seien  sum a_k  und  sum b_k  zwei Reihen. Weiterhin sei  sigma : NN to NN^2  bijektiv und  sigma(k) =: (sigma_1(k), sigma_2(k)).  Definieren  c_k := a_{sigma_1(k)} cdot b_{sigma_2(k)}.  Dann heißt  sum c_k  die zu  sigma  gehörende **Produktreihe**.

Satz.. Seien  sum a_k, \; sum b_k  absolut konvergent. Dann ist für jedes bijektive  sigma : NN to NN^2  die zugehörige Produktreihe konvergent. Sie konvergieren *alle* gegen  (sum a_k)(sum b_k).  

Def.. Seien  sum a_k, \; sum b_k  Reihen und  c_n := a_0b_n + a_1b_{n-1} + ... + a_nb_0 = sum_{k=0}^n a_kb_{n-k}.  Dann heißt die Reihe  sum c_k  das **Cauchy-Produkt** der beiden Reihen.

Folgerung.. Sind  sum a_k  und  sum b_k  absolut konvergent, so konvergiert ihr Cauchy-Produkt absolut gegen  (sum a_k)(sum b_k).  

**Doppelreihensatz**..
Sei eine Doppelreihe  (i, j) in NN^2 mapsto a_{ij} in CC  gegeben. Zu jeder Bijektion  sigma : NN to NN^2  konvergiere  sum_{k=0}^infty a_{sigma(k)}  absolut  (a_{(i,j)} := a_{ij}).  Dann gilt: (a) Für alle  i  konvergiert  sum_{j=0}^infty  absolut.. (b) Mit  a_i := sum_{j=0}^infty a_{ij}  konvergiert  sum_{i=0}^infty a_i  absolut.. (c)  sum_{i=0}^infty (sum_{j=0}^infty a_{ij}) := sum_{i=0}^infty a_i = sum_{k=0}^infty a_{sigma(k)}.  

Bmk.. Die obige Vorraussetzung "Für ein bijektives  sigma : NN to NN times NN  ist  sum_{k=0}^infty a_{sigma(k)}  absolut konvergent" ist äquivalent zu: Für alle  m, n in NN  ist  sum_{i=0}^m sum_{j=0}^n |a_{ij}| < C.  

Bmk.. Die obige Aussage gilt auch für  i  und  j  vertauscht  (widetilde{a_{ij}} := a_{ji}).  

# Dez 11. Wurzel- und Quotientenkriterium, Potenzreihen

[**Wurzelkriterium**](http://www.proofwiki.org/wiki/Nth_Root_Test)..
(a) Sei  q in (0,1) subset RR.  Für  sum_{k=0}^infty a_k  gelte  sqrt[n]{|a_n|} ≤ q  für fast alle  n.  Dann konvergiert  sum a_k  absolut.. (b) Falls hingegen  sqrt[n]{|a_n|} ≥ 1  für unendlich viele  n in NN,  dann divergiert diese Reihe.

[**Quotientenkriterium**](http://www.proofwiki.org/wiki/Ratio_Test)..
(a) Sei  q in (0, 1).  Sei außerdem  a_n neq 0  für fast alle  n in NN,  sowie  left|frac {a_{n+1}} {a_n}right| ≤ q  für fast alle  n.  Dann konvergiert  sum a_k  absolut. (b)  a neq 0  für fast alle  n  und  left|frac {a_{n+1}} {a_n}right| ≥ 1  für fast alle  n,  dann ist  sum a_k  divergent.

Bmk.. Aus Voraussetzung des QK folgt Voraussetzung des WK. (Voraussetzung des QK ist stärker als Voraussetzung des WK, das heißt die Aussage des WK ist stärker als die des QK.)

Def.. Eine Reihe der Form  P(z) = sum_{k=0}^infty a_k z^k  mit  a_k in CC  und (Parameter)  z in CC  heißt **Potenzreihe**.

Satz.. Sei  z_0 in CC  und  sum_{k=0}^infty a_k z_0^k  konvergent. Dann konvergiert  sum_{k=0}^infty a_k z^k  absolut für alle  z in CC  mit  |z| < |z_0|.  

Def.. Der **Konvergenzradius** einer Potenzreihe  P(z) = sum_{k=0}^infty a_k z^k  ist definiert als  R := sup \{r ≥ 0 : P(r) \text{ konvergiert}\}. \; K_R(0) := \{z in CC : |z| < R\}  heißt **Konvergenzkreis**.  (R in [0, infty] := [0, infty) cup \{infty\}.)  

Satz.. Sei  P(z) = sum_{n=0}^infty a_n z^n  und  R in [0, infty]  ihr Konvergenzradius.. (i)  P(z)  konvergiert dann absolut für alle  z in CC  mit  |z| < R..  (ii)  P(z)  divergiert dann für alle  z in CC  mit  |z| > R.  

**Berechnung des Konvergenzradius**.. Sei  R  Konvergenzradius der Reihe  sum a_k z^k.  (a)  R=frac 1 L  falls  L := limn sup sqrt[n]{|a_n|} in [0, infty] \; (frac 1 0 := infty, frac 1 infty := 0  HIER!). (b) Sei  left|frac {a_{n+1}} {a_n}right|  konvergent oder konvergierend gegen  infty.  Dann ist  R= frac 1 q,  wobei  q := limn left|frac {a_{n+1}} {a_n}right|.  

# Dez 13. Identitätssatz, Stetigkeit

Satz.. Seien  P(z) = sum a_k z^k  und  Q(z) = sum b_k z^k  zwei Reihen mit Konvergenzradius  R_1  bzw.  R_2.  Dann hat die Potenzreihe  S(z):=sum_{n=0}^infty (sum_{k=0}^n a_k b_{n-k})z^n  den Konvergenzradius  R = min (R_1, R_2).  

**Identitätssatz**.. Seien  P(z)=sum a_k z^k  und  Q(z)=b_k z^k  zwei Potenzreihen mit *positiven* Konvergenzradien und sei  P(z_n) = Q(z_n)  für eine Nullfolge paarweise verschiedener  z_n in CC.  Dann ist  P=Q,  das heißt  a_k = b_k  für alle  k.  

Lemma.. Sei  P(z) = sum a_k z^k  mit  a_k neq 0  für mindestens ein  k  eine Reihe mit Konvergenzradius  R in (0, infty].  Dann gibt es ein  eps > 0,  so dass für jedes  z in CC, \; |z| < R \; (z in K_R(0))  mit  z neq 0  gilt:  P(z) = sum_{k=0}^infty a_k z^k neq 0,  falls  |z| < eps.  

Def.. Eine Funktion  f:D to CC \; (D sse CC)  heißt **stetig in**  z_0 in D  falls: Für alle  eps > 0  existiert ein  delta > 0,  so dass für jedes  z in D  mit  |z-z_0|<delta  gilt:  |f(z)-f(z_0)| < eps.  Eine Funktion, die in allen  z in D  stetig ist, heißt **stetig**.

# Dez 20. Lipschitz-stetig, Folgenkriterium

Def..  D sse CC. \; f:D to CC  heißt **Lipschitz-stetig** falls es ein  L >= 0  gibt für das gilt:  |f(x)-f(y)| <= L cdot |x-y|  für alle  x,y in D.  

Satz.. Jede Lipschitz-stetige Funktion ist stetig.

Satz..  E sse D sse CC, \; z_0 in E, \; f:D to CC  ist stetig in  z_0.  Dann ist auch  f|_E : E to CC  stetig in  z_0.  

**Folgenkriterium der Stetigkeit**..  D sse CC, \; z_0 in D.  Eine Funktion  f: D to CC  ist genau dann stetig in  z_0,  wenn *für jede* Folge  (z_n) sse CC  mit  limn z_n = z_0  gilt, dass  limn f(z_n) = f(z_0).  

Satz.. (i)  D sse CC.  Seien  f,g : D to CC  stetig in  z_0 in D.  Dann sind  f+g, f cdot g : D to CC  stetig in  z_0..  (ii) Sei  E:=\{z in D : g(z) neq 0\}.  Dann gibt es für jedes  z_0 in E  ein  r>0  mit  g|_{K_r(z_0) cap D} neq 0  überall (das heißt  K_r(z_0) cap D sse E).  Weiterhin gilt  frac{f|_E}{g|_E} : E to CC  ist stetig in  z_0.  

# Jan 8. Gleichmäßige Konvergenz

Satz..  D sse CC.  Seien  f:D to CC, g:E to CC  stetige Funktionen mit  f(D) sse E.  Dann ist  g circ f : D to CC  ebenfalls stetig.

Satz..  f:D to CC  stetig. Dann sind  overline f, |f|, Re f  und  Im f  ebenfalls stetig.

Def..  D sse RR, f : D to RR  heißt **(streng) monoton wachsend**, falls für alle  x, y in D: x < y => f(x) ≤ f(y) \; (f(x) < f(y)).  **Monoton fallend** analog.

Satz.. Sei  I sse RR  ein Intervall und  f:I to RR  streng monoton wachsend. Definieren  E:=f(I) = \{f(x) : x in I\}  und  g:E to I sse RR  mit  g(y) := x  für  f(x) = y. \; g  heißt **Umkehrfunktion**. Sie ist wohldefiniert und stetig.

Bsp..  n in NN.. g(x) := sqrt[n]{x}  ist stetig.

Folgerung..  f(x) = x^s  für  s in QQ_+  ist stetig.

Def.. Sei  D sse CC  und  f_n : D to CC  eine Folge,  (f_n),  von Funktionen  f:D to CC. \; (f_n)  **konvergiert punktweise** gegen  f  falls für *jedes*  z in D  gilt:  limn f_n(z) = f(z). \; f  heißt **Grenzwert** oder **Grenzfunktion**. Schreibweise:  limn f_n = f  punktweise.

Def.. Sei  D sse CC  und  f:D to CC  Funktion.  ||f||_D := sup \{|f(x)|:x in D\} in [0, infty]  ist die **Supremumsnorm**.  f  heißt **beschränkt**, falls  ||f||_D < infty.  

Bmk.. Seien  f, g : D to CC  beschränkt.. (1)  ||f||_D = 0 <=> f == 0..  (2)  c in CC : ||cf||_D = |c| cdot ||f||_D.  (3)  ||f+g||_D ≤ ||f||_D + ||g||_D.  

Def..  D sse CC, \; f_n, f : D to CC  Funktionen,  n in NN.. (f_n)  **konvergiert gleichmäßig** gegen  f  falls  limn ||f_n-f||_D = 0.  Schreibweise:  limn f_n = f  gleichmäßig.

Bmk..  (f_n)  konvergiere gleichmäßig gegen  f.  Dann konvergiert  (f_n)  auch punktweise.

Satz..  D sse CC, \; f_n, f : D to CC, n in NN.. (f_n)  konvergiere gleichmäßig gegen  f  und alle  f_n  seien stetig. Dann ist  f  auch stetig.

# Jan 10. Funktionenreihen, Zwischenwertsatz

Def.. Sei  (f_n)_{n in NN}  eine Folge von Funktionen  f_n : D sse CC to CC.  Die Funktionenreihe  sum_{n=0}^infty f_n  heißt **absolut** konvergent, falls für jedes  z in D  die Reihe  sum_{n=0}^infty f_n(z)  absolut konvergiert.

Def..  sum_{n=0}^infty f_n  heißt **gleichmäßig** konvergent, falls die Folge der Partialsummen  s_n = sum_{k=0}^n f_k : D to CC  gleichmäßig konvergiert.

**Weierstraßkriterium für die Konvergenz einer Funktionenreihe**.. Sei  sum_{n=0}^infty f_n  eine Funktionenreihe wie oben. Gilt  sum_{n=0}^infty ||f_n||_D < infty,  dann ist  sum_{n=0}^infty f_n  absolut und gleichmäßig konvergent.

Bmk.. Die Umkehrung gilt nicht.

Satz.. Sei  P(z) = sum_{k=0}^infty a_k z^k  eine Potenzreihe mit Konvergenzradius  R > 0..  (1) Für  0<r<R  ist  P(z)|_{K_r(0)}  absolut und gleichmäßig konvergent.. (2)  P:K_R(0) to CC  ist stetig.

Bsp.. (i)  z mapsto sum_{k=0}^infty z^k  ist stetig auf  K_1(0)..  (ii)  exp(z) = sum_{k=0}^infty frac{1}{k!} z^k  definiert eine stetige Funktion  CC to CC.  

**Zwischenwertsatz**.. Sei  f : [a,b] to RR  eine stetige Funktion. Dann existiert für jedes  y  echt zwischen  f(a)  und  f(b)  ein  c in (a,b)  mit  y = f(c).  

Satz.. Ist  P(x) = a_n x^n + ... + a_1 x + a_0  ein reelles Polynom vom Grad  n in NN, \; a_n neq 0, \; n  ungerade. Dann hat  P  eine Nullstelle in  RR.  

Satz.. (i) Für  z, w in CC  gilt  exp(z+w) = exp(z)exp(w)..  (ii)  exp|_RR : RR to RR_+  ist streng monoton wachsend, stetig und bijektiv.. (iii) Die Umkehrfunktion  ln = (exp|_RR)^{-1}  ist eine streng monoton wachsende, stetige und bijektive Funktion  RR_+ to RR..  (iv) Es gilt  ln(1) = 0  und  ln(xy) = ln(x) + ln(y)  für  x,y in RR_+.  

# Jan 15. Offene Menge

Def..  exp(z) := sum_{k=0}^infty frac{z^k}{k!}.  

Satz..  x, y in CC.. exp(x+y) = exp(x) cdot exp(y).  

Folgerung.. (1)  exp(1) = sum_{k=0}^infty frac{1}{k!} = e (= limn (1+frac 1 n)^n)..  (2) Für  x in QQ  gilt  exp(x) = e^x.  Setzen für  x in RR: \; e^x := exp(x)..  (3)  a > 0, x in RR. \; a^x := e^{x cdot ln a}.  Das passt zu der alten Definition:  x in QQ => a^x = sqrt[n]{m}.  Außerdem:  x in RR mapsto a^x in RR  stetig.

Def.. (1) Eine Teilmenge  U sse RR  heißt **offen** (offene Menge), falls es für jedes  x in U  ein  ε > 0  gibt, so dass  (x-ε, x+ε) sse U..  (2)  U sse CC  heißt offen, falls für jedes  x in U  ein  ε > 0  existiert, so dass  K(x; ε) sse U..  (3)  A sse RR  (bzw.  A sse CC)  heißt **abgeschlossen**, wenn  RR setminus A  (bzw.  CC setminus A)  offen ist.

Bsp.. (1)  RR subset CC  abgeschlossen, aber nicht offen. (2)  a,b in RR, a<b. \; (a,b) subset RR  offen, aber nicht in  CC. \; [a,b] subset RR  abgeschlossen, auch abgeschlossen in  CC.  

Satz.. (1) Jede offene Menge in  RR  (in  CC)  ist *abzählbare* Vereinigung von offenen Intervallen (offenen Kreisscheiben).. (2)  A sse RR  abgeschlossen, dann auch  A sse CC  abgeschlossen.. (3)  A sse CC  abgeschlossen genau dann, wenn für jede Folge  (x_n) sse A  gilt:  (limn x_n = x) => (x in A).  

Satz.. Sei  f : D to RR, \; f  stetig,  D sse CC  sei abgeschlossen und beschränkt. Dann nimmt  f  ihr Minimum und ihr Maximum auf  D  an: Es gibt ein  x_{min}, x_{max} in D,  so dass  f(x_{min}) = inf \{f(x) : x in D\}, \; f(x_{max}) = sup \{f(x) : x in D\}.  Insbesondere ist  f  beschränkt. Man spricht dann von Minimum/Maximum.  max \{f(x) : x in D\} = sup \{f(x) : x in D\}.  

Def.. Eine Funktion  f : D to CC, D sse CC  heißt **gleichmäßig stetig**, falls es für jedes  ε > 0  ein  ∂ > 0  gibt, so dass für beliebige  x, x_0 in D  gilt:  (|x-x_0|) < ∂) => (|f(x) - f(x_0)| < ε).  

Bmk.. Gleichmäßig stetig  =>  stetig (überall).

Bsp..  f(x) = frac 1 x, \; 0 < a < b. \; f|_{[a,b]} to RR  ist gleichmäßig stetig..  f: (0, infty) to RR  ist stetig, aber nicht gleichmäßig stetig.

# Jan 17. Links- und rechtsseitiger Grenzwert, Differenzierbarkeit

Satz.. Sei  C sse CC  beschränkt und abgeschlossen, und  f:D to CC.  Dann ist  f  stetig genau dann, wenn  f  gleichmäßig stetig ist.

Bmk.. Dieser Satz und der vorherige gelten, weil  D  "kompakt" ist: Jede Folge  (x_n) subset D  besitzt Teilfolge, die gegen Element in  D  konvergiert.

Bsp..  f:[0,∞) to RR, \; f(x) := sqrt x. \; f|_{[0,N]}  ist gleichmäßig stetig (Satz) und ist sogar gleichmäßig stetig auf  [0,∞)  (explizites Nachrechnen).  f  ist aber nicht Lipschitz-stetig.

Def.. Sei  f:D to CC  eine Funktion und  a in CC,  so dass es eine Folge  (x_n) subset D  gibt, mit  limn x_n = a..  (1) Für *jede* Folge  (x_n) subset D  mit  limn x_n = a  gelte  limn f(x_n) = c.  Dann heißt  lim_{x to a} f(x) = c  der **Grenzwert von _f_ in _a_**.. (2) Sei  D subset RR  und für jede Folge  (x_n) subset D  mit  x_n > a  und  limn x_n = a  gelte  limn f(x_n) = c.  Dann heißt  lim_{x down a} f(x) = c  der **rechtsseitige Grenzwert von _f_ in _a_**.. (3) Es gelte dasselbe wie in (2), aber  x_n < a.  Dann heißt  lim_{x up a} f(x) = c  der **linksseitige Grenzwert von _f_ in _a_**.. (4) Für jede Folge  (x_n) subset D  mit  limn x_n = ±∞  gelte  limn f(x_n) = c.  Wir schreiben dann  lim_{x to ±∞} f(x) = c..  (5) Sei  a in RR cup \{+∞, -∞\}  und für jede Folge  (x_n) subset D  mit  limn x_n = a  gelte  limn f(x_n) = ±∞.  Wir schreiben dann  lim_{x to a} f(x) = ±∞.  Entsprechend  lim_{x up a} f(x) = ±∞  und  lim_{x down a} f(x) = ±∞.  

Bmk.. (1)  f:D to CC, \; a in D.  Dann  f  stetig in  a <=> lim_{x to a} f(x) = f(a)..  (2)  D sse RR, \; a in D.  Dann  f  stetig in  a <=> lim_{x down a} f(x) = lim_{x up a} f(x) = f(a).  

Bmk.. Rechenregeln für Grenzwerte von Folgen implizieren entsprechende Regeln für Grenzwerte von Funktionen:  lim_{x to a} (f cdot g)(x) = lim_{x to a} f(x) cdot lim_{x to a} g(x)  usw. Auch Cauchyfolgenkonvergenz und Konvergenz monotoner, beschränkter Folgen.

Def..  f:D to CC, \; D sse RR  Funktion.  x in D  sei **nicht isoliert in _D_**, das heißt es existiert  (x_n) subset D setminus \{x\}  mit  limn x_n = x.  Dann heißt  f  **differenzierbar in _x_** falls der Grenzwert  lim_{ξ to x} frac{f(ξ)-f(x)}{ξ-x}  existiert.

Bmk..  frac{f(ξ)-f(x)}{ξ-x} = a  ist der Anstieg der Geraden durch die Punkte  (x, f(x))  und  (ξ,f(ξ)).  

Bmk..  f'(x)  wird interpretiert als Anstieg der Tangenten an den Graphen von  f. \; f'(x)  heißt **Ableitung von _f_ in _x_**.

# Jan 22. Ableitungsregeln

Bsp..  c in CC, f: RR to CC..  (1)  f(x) = c => f'(x)=0..  (2)  f(x) = cx => f'(x) = c..  (3)  f:RR setminus \{0\} to RR, f(x) = frac 1 x => f'(x) = - frac{1}{x^2}..  (4)  exp'(x) = exp(x)..  (5)  f(x) = x^2 => f'(x) = 2x.  Allgemein:  n in NN, f(x) = x^n => f'(x) = n x^{n-1}..  (6)  f(x) = |x|  nicht differenzierbar in  x=0.  

Def.. Sei  f:D to CC  Funktion,  x in D.  Dann heißt  f  von rechts (links) differenzierbar, falls  lim_{ξ down x} frac{f(ξ)-f(x)}{ξ-x}  existiert (bzw.  lim_{ξ up x} frac{f(ξ)-f(x)}{ξ-x}  existiert).

Satz.. Sei  f: D to CC  Funktion,  x in D.  Dann ist  f  in  x  differenzierbar genau dann, wenn für alle  ξ in D  gilt:  f(ξ) = f(x) + c cdot (ξ-x) + phi(ξ)  für ein  c in D  und  phi: D to CC  mit  lim_{ξ to x} frac{phi(ξ)}{ξ-x} = 0.  

Folgerung.. Ist  f:D to CC  in  x  differenzierbar, so ist  f  in  x  stetig. Ist  f  in allen  x in D  differenzierbar, so ist  f: D to CC  stetige Funktion.

**Rechenregeln**..  f,g: D to CC  Funktionen,  λ in CC, x in D, f  und  g  in  x  differenzierbar. Dann sind  (f+g), (λ f), (f cdot g) : D to CC  differenzierbar in  x.  Ist  g(y) neq 0  für alle  y in D,  dann ist auch  (frac{f}{g}):D to CC  differenzierbar. Es gelten folgende Gesetze..  (λ f)'(x) = λ f'(x).. (f+g)'(x) = f'(x) + g'(x).. (f cdot g)'(x) = f'(x)g(x) + f(x)g'(x).. (frac f g)'(x) = frac{f'(x)g(x)-f(x)g'(x)}{(g(x))^2}.  

**Ableitung der Umkehrfunktion**..  I=[a,b] subset RR  sei abgeschlossenes Intervall. Sei  f:I to RR  streng monoton (wachsend oder fallend).  f  sei stetig. Dann ist  f(I) subset RR  wieder abgeschlossenes Intervall  J.  Sei  g:J to I  die Umkehrfunktion.. Ist  f  in  x  differenzierbar, so ist  g  in  y=f(x)  differenzierbar (und umgekehrt) und es gilt  g'(x) = frac{1}{f'(x)} = frac{1}{f'(g(y))}.  

# Jan 24. Kettenregel, Satz von Rolle

**Kettenregel**..  I, J subset RR, \; g : I to J, \; f: J to RR.  Sei  g  in  x_0  differenzierbar und  f  in  g(x_0)  differenzierbar. Dann ist  f circ g  in  x_0  differenzierbar und es gilt  (f circ g)'(x_0) = f'(g(x_0)) cdot g'(x_0).  

Def..  I,J subset RR..  Jede Funktion  f: I to CC  ist **null mal differenzierbar**. Ihre nullte Ableitung,  f^{(0)},  ist  f  selbst:  f^{(0)} = f.. k in NN.  Eine Funktion,  f,  heißt **_k_ mal differenzierbar** in  x_0 in J,  falls  f  auf  J \; (k-1)  mal differenzierbar ist und  f^{(k-1)} : J to CC  in  x_0  differenzierbar ist.  f^{(k)} := (f^{(k-1)})'(x_0).  

Def.. Sei  f: (a,b) to RR  Funktion. Dann nimmt  f  in  x_0 in (a,b)  ihr **lokales Minimum** bzw. **Maximum** an, falls für ein  ε > 0  und für alle  x in (x_0-ε, x_0+ε)  gilt:  f(x_0) ≤ f(x)  bzw.  f(x_0) ≥ f(x).  Gilt  (f(x)=f(x_0)) <=> (x=x_0)  oder  x not in (x_0-ε, x_0+ε),  dann nennen wir das Minimum/Maximum **strikt**. (Extremum ist Minimum oder Maximum.)

Satz.. Hat  f:(a,b) to RR  in  x_0  ein lokales Extremum und ist dort differenzierbar, so ist  f'(x_0) = 0.  

**Satz von Rolle**.. Sei  f:[a,b] to RR  stetig und  f: (a,b) to RR  differenzierbar. Ist  f(a)=f(b),  dann existiert ein  x in (a,b)  mit  f'(x)=0.  

Satz..  f:[a,b] to RR  stetig,  f  differenzierbar auf  (a,b).  Dann existiert  x in (a,b),  so dass  f'(x) = frac{f(b)-f(a)}{b-a}.  

Folgerung.. (1) Sei  f:[a,b] to RR  wie vorher und sei  m ≤ f'(x) ≤ M  für geeignete  m,M in RR  und *alle*  x in (a,b).  Dann  m ≤ frac{f(b)-f(a)}{b-a} ≤ M => m(b-a) ≤ f(b)-f(a) ≤ M(b-a)..  (2) Ist insbesondere  f'(x)=0  für alle  x in (a,b).  Dann  f  ist konstant. (Es gilt  frac{f(x)-f(b)}{b-a} = 0  für alle  x in (a,b).)  

Satz..  c in RR  und  f:RR to RR  differenzierbar mit  f'(x) = c cdot f(x)  für alle  x.  Dann ist  f(x) = A cdot e^{cx}  für  A = f(0).  
