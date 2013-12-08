Layout: math

Def.. Sei  X : A to B  und  k in B.  Dann steht der Ausdruck  mlq X = k mrq  abkürzend für die Menge  \{om in A mid X(om) = k\}.  Analog für  mlq\! ≤ \!mrq.  

# Oct. 23

Satz.. Mit Wiederholung, mit Reihenfolge:  n^r..  Mit Wiederholung, *ohne* Reihenfolge:  binom{n+r-1}{r}..  *Ohne* Wiederholung, mit Reihenfolge:  frac{n!}{(n-r)!}..  Ohne Wiederholung, *ohne* Reihenfolge:  binom n r.  

Def.. Eine Folge von Ereignissen  (E_n)  heißt **paarweise disjunkt**, falls für alle  i neq j  gilt:  E_i schnitt E_j = leer.  

Def.. Sei  A  eine nicht-leere Menge. Dann heißt  B sse Pp(A)  eine  sigma  -**Algebra auf**  A,  falls gilt:: (i) Die *Grundmenge ist enthalten*, das heißt:  A in B, quad  (ii)  B  ist *abgeschlossen gegenüber Komplementbildung*, das heißt für alle  M in B  gilt:  M^C in B quad  und (iii)  B  ist *abgeschlossen gegenüber Vereinigung*, das heißt für jede Folge  (M_n)  mit  M_n in B  gilt:  left(Verein_{n in N} M_n right) in B.  

Def.. Sei  Om  nicht-leer und  Ff  eine  sigma  -Algebra auf  Om.  Eine Funktion  PP : Ff to [0, 1]  heißt **Wahrscheinlichkeitsmaß auf**  Om,  falls gilt:: (i)  PP  ist *normiert*, das heißt:  PP(Om) = 1 quad  und (ii)  PP  ist  sigma  -*additiv*, das heißt für jede Folge paarweise disjunkter Ereignisse  (E_n)  gilt:  PP(Verein_{n in NN} E_n) = sum_{n in NN} PP(E_n).  

Prop..  PP(leer) = 0.. PP  ist endlich additiv, das heißt für beliebige paarweise disjunkte  E_1, ..., E_n in Ff  gilt:  PP(Verein_{i = 1}^n E_i) = sum_{i = 1}^n PP (E_i).  

Prop.. Sei  E in Ff.  Dann  PP(E^C) = 1 - PP(E).  

Prop.. Für  E, F in Ff  mit  E sse F  gilt:  PP(E) ≤ PP(F).  

Prop.. Seien  E, F in Ff.  Dann gilt:  PP(E verin F) = PP(E) + PP(F) - PP(E schnitt F).  

# Nov. 11

%Def.. Sei  (Omega, Ff, PP)  ein Wkt.sraum. Eine **Zufallsvariable** (ZV) ist eine messbare Abbildung  X : (Omega, Ff) to (RR^n, Bb(RR^n)).  (Damit gilt  X^{-1}(A) in Ff,, forall A in Bb(RR^n)).  

%Bmk.. Für diskrete Grundräume  Omega = \{omega_i\}  wählen wir  Ff = Pp(Omega),  und Messbarkeit ist automatisch erfüllt. Für  Omega aus RR^n  wählen wir  Ff = Bb(RR^n),  und  X  ist Prinzip ?? in Analysis I  (f to X.. f(x) to X(omega)).  

Def.. Sei  (Omega, Ff, PP)  ein W'keitsraum. Eine **Zufallsvariable** ist eine Abbildung  X : Om to RR..  

Bmk.. Für Zufallsvariablen  X  gilt  X^{-1}(k) in Ff  für alle  k in RR.  

Def.. Eine Zufallsvariable  X  heißt **diskret**, falls  X(Om)  endlich oder abzählbar unendlich.

Def.. Sei  X  eine diskrete Zufallsvariable auf  (Om, Ff, PP).  Dann heißt  p_X : RR to [0, 1]  mit  p_X(k) := PP(X^-1(k))  die **Massenfunktion von _X_**.

> Bsp.. Wir haben eine Urne mit 20 nummerierten Kugeln. Wir ziehen 3x ohne Zurücklegen. Wir suchen die Wkt, dass wir eine Kugel mit Nr.  >= 17  ziehen. Haben also Laplace-Experiment mit  Om = \{1, ..., 20\}^3.  Wählen die Zufallsvariable  X  mit  X(om) = max om.  Suchen also die Wkt  PP\{X(om) >= 17\} = p_X(17) + ... + p_X(20).  Berechnen zuerst  p_X(20).  Die Gegenwkt ist  frac{19}{20} cdot frac{18}{19} cdot frac{17}{18} = frac{17}{20}.  Also  p_X(20) = 1 - frac{17}{20} = frac{3}{20}.  Ein alternativer Rechenweg stellt fest, dass dieses Ereignis aus  binom{19}{2}  günstigen Realisierungen besteht, bei  binom{20}{3}  möglichen Realisierungen. Also  p_X(20) = frac{binom{19}{2}}{binom{20}{3}} = frac{3}{20}.  Analog gilt für  i in \{17, 18, 19\},  dass  p_X(i) = frac{binom{i - 1}{2}}{binom{20}{3}}.  

> Bsp.. Wir werfen eine Münze so lange, bis "Kopf" erscheint, maximal jedoch _n_-mal. "Kopf" erscheint mit Wkt  p in (0, 1).  Sei  X(om)  die Anzahl der Würfe. Wir suchen  p_X(m)  für  m = 1, ..., n.  Da wir für das Ereignis  \{X(om) = m\}  zuerst  m - 1  Mal "Zahl" geworfen (Wkt.  1 - p)  haben müssen, und daraufhin "Kopf" (Wkt  p),  gilt  p_X(m) = (1 - p)^{m - 1}.  Allerdings nicht für den Fall  m = n,  denn dort brauchen als letzten Wurf nicht unbedingt "Kopf". Also  p_X(n) = (1 - p)^{n - 1}..  Es gilt dann  PP(bigcup_{i = 1}^n \{X(om) = i\}) = sum_{i = 1}^n PP\{X(om) = i\} = 1.  

> Bsp.. Es gibt  N  unterscheidbare Coupons. Wir sammeln diese (unabhängig). Sei  T(om)  die Anzahl der Coupons, die wir gesammelt haben, bis wir ein vollständiges Set von  N  verschiedenen Coupons haben. Wir suchen  PP\{T(om) = n\}  für  n = N, N + 1, ...  . Es ist einfacher  PP \{T(om) > n\}  zu berechnen. (Es gilt dann  PP\{T(om) = n\} = PP\{T(om) > n - 1\} - PP\{T(om) > n\}.)  Es sei  A_j  das Ereignis, dass sich kein *j*-Coupon unter den ersten  n  Versuchen befindet. Dann gilt  PP\{T(om) > n\} = PP(bigcup_{j = 1}^N A_j) = ... = N(frac{N - 1}{N})^n - binom N 2 (frac{N - 2}{N})^n + ... + (-1)^N binom{N}{N - 1}(frac{N - (N - 1)}{N})^n + 0.  

Def.. Sei  X  eine diskrete Zufallsvariable auf  (Om, Ff, PP).  Dann heißt  EE(X) = sum_{x in X(Om)} x cdot p_X(x)  der **Erwartungswert von _X_**, falls diese Reihe absolut konvergiert, das heißt  sum_{x in X(Om)} |x| cdot p_X(x) < infty.  

> Bsp.. Sei  A aus Om.  Wir definieren als Zufallsvariable die Indikatorfunktion  I_A : Om to \{0, 1\}  mit  I_A(om) = 1,  falls  om in A  und  I_A(om) = 0,  sonst. Dann gilt  p_{I_A}(0) = PP(A^C) = 1 - PP(A)  und  p_{I_A}(1) = PP(A).  Also nach Definition  EE I_A = 0 cdot (1 - PP(A)) + 1 cdot PP(A) = PP(A).  

# Nov. 20

Def.. Sei  X  eine Zufallsvariable auf  (Om, Ff, PP).  Dann heißt  F_X : RR to [0, 1]  mit  F_X(k) := PP \{X(om) <= k\}  die **Verteilungsfunktion von _X_**.

Prop.. Es gilt (i)  F  ist monoton wachsend, (ii)  lim_{b to infty} F(b) = 1,  (iii)  lim{b to -infty} = 0  und (iv)  F  ist rechtsseitig stetig.

% Folgen von Zufallsvariablen, die Indikatorfunktionen sind
Def.. Eine Zufallsvariable  X  heißt  (n, p)  -**binominalverteilt**, wenn sie die Anzahl der Erfolge (Eintritt mit W'keit *p*) in einer Versuchsreihe der Länge  n  misst. Also  Om = \{0, 1\}^n  und  X(om) = sum om.  Schreiben dann  X sim B(n, p).  

Bmk.. Für binomialverteilte Zufallsvariablen  X  gilt  X(Om) aus NN.  

Prop.. Sei  X  eine Zufallsvariable mit  X sim B(n, p).  Sei  k in NN.  Dann gilt  PP\{X(om) = k\} = binom n k p^k (1-p)^{n-k}.  Außerdem gilt  EE X = n p  und  Var X = n p (1-p).  

Prop.. Gelte  X sim B(n, p).  Dann ist  p_X  monoton wachsend für  k <= (n + 1)p  und monoton fallend für  k >= (n + 1)p.  

% Binomialverteilungen mit großem n und kleinem p
Def.. Sei  lam > 0.  Eine Zufallsvariable  X  mit Werten in  ZZ^+  und Massenfunktion  p_X(k) = e^{-lam} frac{lam^k}{k!}  heißt **Poisson-verteilt** mit Parameter  lam.  Schreiben  X sim pi(lam).  

# Nov. 25

Prop.. Für  n p_n overset{n to infty}{longrightarrow} lam  gilt  binom n k p_n^k (1-p_n)^{n-k} overset{n to infty}{longrightarrow} e^{-lam} frac{lam^k}{k!}.  Man kann also Binomialverteilungen für große  n  durch die Poisson-Verteilung approximieren.

Lemma.. Sei  X sim pi(lam).  Dann gilt  EE X = Var X = lam.  

Def.. Sei  n in NN  und  X_n sim B(n, p).  Dann definieren wir  X_n^* := frac{X_n - n p}{sqrt{n p (1-p)}}.  

Def..  phi(x) := frac{1}{sqrt{2 pi}} e^{-frac{x^2}{2}}  für  x in RR.  

**Satz von deMoivre/Laplace**.. Sei  p = frac 1 2.  Sei  X_n sim B(n, p)  für alle  n in NN.  Dann gilt für  a, b in RR  mit  a < b,  dass  lim_{n to infty} PP \{a <= X_n^*(om) <= b\} = int_a^b phi(x) d x.  

Bmk.. (i)  int_{-infty}^infty phi(x) = 1..  (ii) Theorem gilt auch für  p in (0, 1).  

Def.. Für Folgen  (a_n)  und  (b_n)  schreiben wir  a_n sim b_n,  falls  lim_{n to infty} frac{a_n}{b_n} = 1.  

**Stirling-Formel**..  n! sim sqrt{2 pi n}(frac n e)^n.  
