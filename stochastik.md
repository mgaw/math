Layout: math

# Nov. 11

Def.. Sei  (Omega, Ff, PP)  ein Wktsraum. Eine **Zufallsvariable** (ZV) ist eine messbare Abbildung  X : (Omega, Ff) to (RR^n, Bb(RR^n)).  (Damit gilt  X^{-1}(A) in Ff,, forall A in Bb(RR^n)).  

Bmk.. Für diskrete Grundräume  Omega = \{omega_i\}  wählen wir  Ff = Pp(Omega),  und Messbarkeit ist automatisch erfüllt. Für  Omega aus RR^n  wählen wir  Ff = Bb(RR^n),  und  X  ist Prinzip ?? in Analysis I  (f to X.. f(x) to X(omega)).  

Def.. Eine Zufallsvariable  X  heißt **diskret**, falls  X(Om) = \{x : X(om) = x text{ für ein } om in Om\} = \{x_i\}_{i = 1, ..., n}  mit  n in NN verein \{infty\}.  

Def.. Sei  X  eine ZV auf  (Om, Ff, PP)  und  k in RR.  Dann definieren wir die Menge  [X = k] := \{om in Om : X(om) = k\} in Ff.  

Def.. Sei  X  eine diskrete ZV. Dann heißt  p_X : X(Om) to [0, 1]  mit  x mapsto PP[X = x]  **Massenfunktion** bzw. **Wktverteilung von _X_** (unter dem Maß  PP).  

> Bsp.. Wir haben eine Urne mit 20 nummerierten Kugeln. Wir ziehen 3x ohne Zurücklegen. Wir suchen die Wkt, dass wir eine Kugel mit Nr.  >= 17  ziehen. Haben also Laplace-Experiment mit  Om = \{1, ..., 20\}^3.  Wählen die Zufallsvariable  X  mit  X(om) = max om.  Suchen also die Wkt  PP[X >= 17] = PP[X = 17] + ... + PP[X = 20].  Berechnen zuerst  PP[X = 20].  Die Gegenwkt ist  frac{19}{20} cdot frac{18}{19} cdot frac{17}{18} = frac{17}{20}.  Also  PP[X = 20] = 1 - frac{17}{20} = frac{3}{20}.  Ein alternativer Rechenweg stellt fest, dass dieses Ereignis aus  binom{19}{2}  günstigen Realisierungen besteht, bei  binom{20}{3}  möglichen Realisierungen. Also  PP[X = 20] = frac{binom{19}{2}}{binom{20}{3}} = frac{3}{20}.  Analog gilt für  i in \{17, 18, 19\},  dass  PP[X=i] = frac{binom{i - 1}{2}}{binom{20}{3}}.  

> Bsp.. Wir werfen eine Münze so lange, bis "Kopf" erscheint, maximal jedoch _n_-mal. "Kopf" erscheint mit Wkt  p in (0, 1).  Sei  X(om)  die Anzahl der Würfe. Wir suchen  PP[X = m]  für  m = 1, ..., n.  Da wir für das Ereignis  [X = m]  zuerst  m - 1  Mal "Zahl" geworfen (Wkt  1 - p)  haben müssen, und daraufhin "Kopf" (Wkt  p),  gilt  PP[X = m] = (1 - p)^{m - 1}.  Allerdings nicht für den Fall  m = n,  denn dort brauchen als letzten Wurf nicht unbedingt "Kopf". Also  PP[X = n] = (1 - p)^{n - 1}..  Es gilt dann  PP(bigcup_{i = 1}^n [X = i]) = sum_{i = 1}^n PP[X = i] = 1.  

> Bsp.. Es gibt  N  unterscheidbare Coupons. Wir sammeln diese (unabhängig). Sei  T(om)  die Anzahl der Coupons, die wir gesammelt haben, bis wir ein vollständiges Set von  N  verschiedenen Coupons haben. Wir suchen  PP[T = n]  für  n = N, N + 1, ...  . Es ist einfacher  PP[T > n]  zu berechnen. (Es gilt dann  PP[T = n] = PP[T > n - 1] - PP[T > n].)  Es sei  A_j  das Ereignis, dass sich kein *j*-Coupon unter den ersten  n  Versuchen befindet. Dann gilt  PP[T > n] = PP(bigcup_{j = 1}^N A_j) = ... = N(frac{N - 1}{N})^n - binom N 2 (frac{N - 2}{N})^n + ... + (-1)^N binom{N}{N - 1}(frac{N - (N - 1)}{N})^n + 0.  

Def.. Sei  X  eine diskrete Zufallsvariable auf  (Om, Ff, PP).  Dann heißt  EE(X) = sum_{x in X(Om)} x cdot p_X(x)  der **Erwartungswert** von *X*, falls diese Reihe absolut konvergiert, das heißt  sum_{x in X(Om)} |x| cdot p_X(x) < infty.  

> Bsp.. Sei  A aus Om.  Wir definieren als Zufallsvariable die Indikatorfunktion  I_A : Om to \{0, 1\}  mit  I_A(om) = 1,  falls  om in A  und  I_A(om) = 0,  sonst. Dann gilt  P_{I_A}(0) = PP(A^C) = 1 - PP(A)  und  P_{I_A}(1) = PP(A).  Also nach Definition  EE I_A = 0 cdot (1 - PP(A)) + 1 cdot PP(A) = PP(A).  
