Titel: Analysis I*
Vorlage: math

# Nov 13. Konvergenz

Def. Eine **Folge**  (a_n)_{n in NN}  ist Abbildung  a : NN to CC. a_n in CC  mit  a_n := a(n).  Eine Folge  (a_n)_{n in NN}  heißt **konvergent**, falls es eine komplexe Zahl  a in CC  gibt mit folgender Eigenschaft: Für jedes  eps > 0  gibt es ein  N in NN  mit: für jedes  n > N  gilt:  |a_n - a| < eps. \; a  heißt dann **Grenzwert** der Folge. Man sagt:  (a_n)  konvergiert gegen  a  oder:  limn a_n = a.  

# Nov 15. Grenzwerte

Bmk.  eps > 0. \; \triangle(a, eps) := \{z in CC : |z-a| < eps \}  "Epsilon-Scheibe".  (a_n)_{n in NN}  konvergiert gegen  a in CC,  gdw.  exists N in NN : forall n > N  gilt  a_n in \triangle(a, eps).  

Satz.  (a_n)_{n in NN}  konvergiert gegen  a in CC  gdw.  (a_n - a)_{n in NN}  eine **Nullfolge** ist, d.h. gegen  0 in CC  konvergiert. (1)  s in QQ_+  gilt  limn 1/n^s = 0.  (2) Für  a > 0  gilt  limn sqrt[n]{a} = 1, \; (n ≥ 1).  (3)  limn sqrt[n]{n} = 1, \; (n≥1).  (4)  z in CC, |z| < 1 : limn z^n = 0.  (5)  z in CC, s in Q_+, |z| > 1 : limn n^s/z^n > 0.  

Satz. Der Limes ist eindeutig bestimmt, wenn er existiert. Beweis Forster S. 34.

# Nov 15. Abzählbarkeit (Übung)

Satz. Ist  M  unendlich und es gibt *surjektive* Abildung  g: NN to M,  dann ist  M  abzählbar.

Satz. Ist  M  abzählbar, und ist  N sse M  unendlich, dann ist auch  N  abzählbar.

Satz. Eine unendliche Vereinigung abzählbar unendlicher Mengen ist abzählbar.

Satz. Eine disjunkte abzählbar unendliche Vereinigung nichtleerer endlicher Mengen ist abzählbar.

# Nov 20. Rechenregeln für Grenzwerte

Def. Sei  (a_n)_{n in NN}  eine Folge. (1) Sie heißt **divergent**, wenn sie nicht konvergiert. (2) Falls für eine reelle Folge gilt: Für jedes  C>0  gibt es ein  N in NN,  so dass für alle  n in NN, n ≥ N  gilt:  a_n > C,  dann schreibt man  limn a_n = + infty.  Analog  limn a_n = - infty.  

Satz. Eine reelle Folge  (a_n)_{n in NN}  konvergiert gegen  + infty,  gdw. die Folge  (1/a_n)_{n in NN}  ab einem gewissen Folgenglied definiert ist und positiv ist und  limn 1/a_n = 0.  

Satz. Seien  (a_n)_{n in NN}, (b_n)_{n in NN}  konvergente Folgen,  a, b  deren Grenzwerte. (1) Dann sind  (a_n+b_n)_{n in NN}, (a_n cdot b_n)_{n in NN}  ebenfalls konvergent,  (a+b)  bzw.  (a cdot b)  ihre zugehörigen Grenzwerte. (2) Ist  b neq 0,  so gibt es  N_0 in NN,  s.d.  b_n neq 0  falls  n ≥ N_0  und  limn 1/b_n = 1/b = 1/limn b_n.  (3) Dann sind auch  (|a_n|), (Re a_n), (Im a_n), (overline a_n)  konvergent und es gelten  limn |a_n| = |a|, limn (Re a_n) = Re a,  usw. Beweis Forster S. 34--36.

Satz.  (a_n)_{n in NN}, (b_n)_{n in NN}  reelle, konvergente Folgen. Es sei  a_n ≤ b_n  für  n ≥ N  mit  N in NN.  Dann folgt  limn a_n ≤ limn b_n.  Beweis Forster S. 37.

Folgerung. (1) Gilt für konvergente Folge  (a_n)_{n in NN},  dass  a_n in [c, d],  falls  n ≥ N.  Dann ist  limn a_n in [c, d].  (2) Ist  (c_n)  eine weitere beliebige Folge und  a_n ≤ c_n ≤ b_n  für  n ≥ N  und  limn a_n = limn b_n = a = b.  Dann ist  (c_n)  konvergent und  limn c_n = a.  

# Nov 22. Monotonie

Satz.  a_n ≤ c_n ≤ b_n, \; limn a_n = limn b_n = a.  Dann ist  (c_n)  eine konvergente Folge und  limn c_n = a.  

Def. Eine *reelle* Folge  (a_n)_{n in NN}  heißt **monoton wachsend** falls gilt:  a_{n+1} ≥ a_n  für alle  n in NN,  **monoton fallend**, falls  a_{n+1} ≤ a_n  für  n in NN.  Gilt sogar  a_{n+1} > a_n (a_{n+1} < a_n)  für alle  n in NN,  dann heißt sie **streng monoton wachsend (fallend)**.

Satz. Eine *beschränkte*, monoton wachsende Folge ist konvergent. Mit  A=\{a_n : n in NN\}  gilt:  limn a_n = sup A.  Ist  (a_n)  monoton fallend und beschränkt, so gilt  limn a_n = inf A.  

# Nov 22. Optimale Schranke

Def.  a in A sse RR  heißt **Schranke** von  A,  wenn  a  untere oder obere Schranke von  A  ist.  a  heißt **optimale Schranke**, wenn  a  kleinste obere oder größte untere Schranke von  A  ist.

# Nov 27. Euler-Zahl, Häufungspunkt

Def. Der Grenzwert der Folge  a_n = (1+frac 1 n)^n  heißt **Euler-Zahl** und wird mit  e:= limn (1+frac 1 n)^n  bezeichnet.

Def.  (a_n)_{n in NN}  sei Folge (in  CC).  Dann heißt ein  h in CC  **Häufungspunkt**, falls für beliebiges  eps > 0  die Menge  \{n : a_n in triangle(h, eps)\}  unendlich ist, d.h. in jeder Epsilon-Scheibe von  h  liegen unendlich viele Folgenglieder von  (a_n).  

Def. Für eine Folge  (a_n)_{n in NN}  und eine Folge  (n_k)_{k in NN}  *natürlicher* Zahlen, die streng monoton wächst, bezeichnet man  (a_{n_k})_{k in NN}  als **Teilfolge** von  (a_n).  

Satz (Bolzano-Weierstraß). (1) Ist  (a_n)_{n in NN}  eine beschränkte Folge, so besitzt sie einen Häufungspunkt. (2) Ist  (a_n)_{n in NN}  reell und beschränkt, so gibt es einen kleinsten sowie einen größten Häufungspunkt,  h_*  und  h^*.  Es gilt:  NN setminus \{n : h_* - eps < a_n < h^* + eps\}  ist endlich für jedes  eps > 0.  

Def.  h_*  heißt **Limes inferior** der Folge,  h^*  heißt **Limes superior**.

# Nov 29. Cauchy-Folge, Reihe

Def. Sei  (a_n)  reelle Folge. Dann ist  limn sup a_n := infty  für nach oben unbeschränkte  a_n,  sonst  limn sup a_n := limn (sup \{a_k : k ≥ n\}). \; limn inf a_n  analog.

Def. Eine Folge  (a_n)  heißt **Cauchy-Folge**, falls gilt: Für jedes  eps > 0  gibt es ein  N in N,  so dass für alle  m, n in NN, \; m, n ≥ N  gilt:  |a_n-a_m| < eps.  

Satz: Cauchy-Kriterium. Eine Folge  (a_n)  in  CC  ist konvergent genau dann, wenn sie eine Cauchy-Folge ist.

Bmk. Das Cauchy-Kriterium folgt aus Supremumeigenschaft von  RR,  beide Eigenschaften sind sogar äquivalent.

Def. Sei  (a_n)  Folge in  CC  und  s_n := sum_{k=0}^n a_k.  Die Folge  (s_n)  heißt **Reihe**, die  a_n  **Glieder der Reihe**, die  s_n  **Partialsummen**. Eine Reihe heißt **konvergent**, falls die Folge  (s_n)  konvergiert. Dann wird der Grenzwert mit  sum_{k=0}^infty a_k := limn s_n  bezeichnet. (Achtung: Mit  sum_{k=0}^infty a_k  wird gewöhnlich auch die *Reihe*  (s_n)  bezeichnet.)

Bsp. Für ein  z in CC  heißt  sum_{k=0}^infty z^k  die **geometrische Reihe**. Für  z neq 1  ist  s_n = sum_{k=0}^n = frac{1-z^{n+1}}{1-z}.  Also für  |z| < 1 : sum_{k=0}^infty z^k = frac 1 {1-z}.  

# Dez 4. Konvergenzkriterien

??.  sum^infty_{k=0} a_k,  auch  sum^infty_{k=k_0},  auch  sum^infty_{k=-k_0}, \; k_0 in NN.  

Konvergenzen.

(i). Geometrische Reihe.

(ii).  sum^infty_{k=1} frac 1 {k(k+1)}; \; s_n = sum^n_{k=1} frac 1 {k(k+1)} = 1 - frac 1 {k+1}, \; limn s_n = 1 - limn frac 1 {n+1} = 1.  

(iii).  sum^infty_{k=0} (-1)^k  divergent.  s_n = 1  für  n  ungerade,  s_n = 0  sonst.

Satz: [Harmonische Reihe](http://www.proofwiki.org/wiki/Sum_of_Reciprocals_is_Divergent).
  sum_{k=1}^infty frac 1 k = infty.  

Satz.  sum_{k=0}^infty a_k  konvergiert genau dann, wenn für jedes  eps > 0  existiert  N in NN,  so dass für  n > m ≥ N : |sum_{k=m+1}^n a_k| < eps.  

Folgerung. 1) Konvergiert  sum_{k=0}^infty a_k  so ist die Folge ihrer Glieder  (a_k)_{k in NN}  eine Nullfolge. 2) Das Abändern *endlich vieler* Reihenglieder ändert nichts am Konvergenzverhalten der Reihe.

Satz: [Majorantenkriterium](http://www.proofwiki.org/wiki/Comparison_Test).
Sei  |a_n| ≤ b_n  für alle  n in NN.  Wenn  sum_{k=0}^infty b_n  konvergiert, so konvergiert auch  sum_{k=0}^infty a_k.  

Satz. Sei  a_n ≥ 0  für alle  n in NN.  Dann konvergiert  sum_{k=0}^infty a_k  genau dann, wenn ihre Partialsummenfolge beschränkt ist.

Bmk.  \zeta (s) := sum_{k=1}^infty frac 1 {k^s}  hießt Riemannsche Zetafunktion.

Satz: [Leibniz-Kriterium](http://www.proofwiki.com/wiki/Alternating_Series_Test).
Sei  (a_n)  eine monoton fallende Nullfolge, dann konvergiert die alternierende Reihe  sum_{k=0}^infty (-1)^k a_k.  

Bmk.  s_{2n+1} ≤ s ≤ s_{2n}  für  n in NN  beliebig.

# Dez 6. Absolute Konvergenz, Produktreihe

Satz: Riemannscher Umordnungssatz.
Sei  (a_n)_{n in NN}  Nullfolge positiver Zahlen mit  sum_{n=0}^{infty} a_n = infty.  Dann gibt es für jedes  lam in RR cup \{-infty, +infty\}  eine Bijektion  sigma : NN to NN,  so dass  sum_{n=0}^infty (-1)^{sigma(n)}a_{sigma(n)} = lam.  

Def. Eine Reihe  sum a_k  heißt **absolut konvergent**, falls  sum |a_k|  konvergiert.

Bmk. Wenn  sum |a_k|  konvergiert, dann konvergiert auch  sum a_k.  

Satz. Sei  sum a_k  absolut konvergent. Dann ist für jede Bijektion  sigma : NN to NN  die Reihe  sum_{k=0}^infty a_{sigma(k)}  absolut konvergent und  sum a_{sigma(k)} = sum a_k.  

Satz.  sum(a_k+b_k) = sum a_k + sum b_k. quad sum(Re a_k) = Re (sum a_k). quad sum Im a_k = Im sum a_k. quad sum overline{a_k} = overline{sum a_k}.  

Def. Seien  sum a_k, \; sum b_k  zwei Reihen. Weiterhin sei  sigma : NN to NN  bijektiv und  sigma(k) =: (sigma_1(k), sigma_2(k)).  Definieren  c_k := a_{sigma_1(k)} cdot b_{sigma_s(k)}.  Dann heißt  sum_{k=0}^infty c_k  (die zu  sigma  gehörende) **Produktreihe**.

Satz. Seien  sum a_k, \; sum b_k  absolut konvergent. Dann ist für jedes bijektive  sigma : NN to NN^2  die zugehörige Produktreihe konvergent. Sie konvergieren *alle* gegen  (sum_{k=0}^infty a_k)(sum_{k=0}^infty b_k).  

Def. Seien  sum a_k, \; sum b_k  Reihen und  c_n := a_0b_n + a_1b_{n-1} + ... + a_nb_0 = sum_{k=0}^infty a_kb_{n-k}.  Dann heißt  sum_{k=0}^infty c_k  das **Cauchy-Produkt** der beiden Reihen.

Folgerung. Sind  sum a_k  und  sum b_k  absolut konvergent, so konvergiert ihr Cauchy-PRodukt absolut gegen  (sum a_k)(sum b_k).  

Satz: Doppelreihensatz.
Sei  (i, j) in NN^2 mapsto a_{ij} in CC  gegeben. Zu jeder Bijektion  sigma : NN to NN^2  konvergiere  sum a_{sigma(k)}  absolut  (a_{(i,j)} := a_{ij}).  Dann gilt: (a) Für alle  i  konvergiert  sum_{j=0}^infty  absolut. (b) Mit  a_i := sum_{j=0}^infty a_{ij}  kovergiert  sum_{i=0}^infty a_i  absolut. (c)  sum_{i=0}^infty (sum_{j=0}^infty a_{ij}) := sum_{i=0}^infty a_i = sum_{k=0}^infty a_{sigma(k)}.  
