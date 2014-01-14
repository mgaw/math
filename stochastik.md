Layout: std palatino

*Def*.. Sei  X : A to B  und  k in B.  Dann steht der Ausdruck  glqq X = k grqq  abkürzend für die Menge  \{om in A mid X(om) = k\}.  Analog für  glqq\! ≤ \!grqq  etc.

Bmk..  Om xrightarrow{enspace X enspace} RR xrightarrow{p_X, F_x} [0, 1].  

# Oct. 23

*Zählweisen*.. Mit Wiederholung, mit Reihenfolge:  n^r..  Mit Wiederholung, *ohne* Reihenfolge:  binom{n+r-1}{r}..  *Ohne* Wiederholung, mit Reihenfolge:  frac{n!}{(n-r)!}..  Ohne Wiederholung, *ohne* Reihenfolge:  binom n r.  

*Def*.. Eine Folge von Ereignissen  (E_n)  heißt **paarweise disjunkt**, falls für alle  i neq j  gilt:  E_i schnitt E_j = leer.  

*Def*.. Sei  A  eine nicht-leere Menge. Dann heißt  B sse Pp(A)  eine  sigma  -**Algebra auf**  A,  falls gilt:: (i) Die *Grundmenge ist enthalten*, das heißt:  A in B, quad  (ii)  B  ist *abgeschlossen gegenüber Komplementbildung*, das heißt für alle  M in B  gilt:  M^C in B quad  und (iii)  B  ist *abgeschlossen gegenüber Vereinigung*, das heißt für jede Folge  (M_n)  mit  M_n in B  gilt:  left(Verein_{n in N} M_n right) in B.  

*Def*.. Sei  Om  nicht-leer und  Ff  eine  sigma  -Algebra auf  Om.  Eine Funktion  PP : Ff to [0, 1]  heißt **Wahrscheinlichkeitsmaß auf**  Om,  falls gilt:: (i)  PP  ist *normiert*, das heißt:  PP(Om) = 1 quad  und (ii)  PP  ist  sigma  -*additiv*, das heißt für jede Folge paarweise disjunkter Ereignisse  (E_n)  gilt:  PP(Verein_{n in NN} E_n) = sum_{n in NN} PP(E_n).  

*Endliche Additivität*..  PP(leer) = 0.. PP  ist endlich additiv, das heißt für beliebige paarweise disjunkte  E_1, ..., E_n in Ff  gilt:  PP(Verein_{i = 1}^n E_i) = sum_{i = 1}^n PP (E_i).  

Prop.. Sei  E in Ff.  Dann  PP(E^C) = 1 - PP(E).  

Prop.. Für  E, F in Ff  mit  E sse F  gilt:  PP(E) ≤ PP(F).  

Prop.. Seien  E, F in Ff.  Dann gilt:  PP(E verin F) = PP(E) + PP(F) - PP(E schnitt F).  

# Nov. 11

%Def.. Sei  (Omega, Ff, PP)  ein Wkt.sraum. Eine **Zufallsvariable** (ZV) ist eine messbare Abbildung  X : (Omega, Ff) to (RR^n, Bb(RR^n)).  (Damit gilt  X^{-1}(A) in Ff,, forall A in Bb(RR^n)).  

%Bmk.. Für diskrete Grundräume  Omega = \{omega_i\}  wählen wir  Ff = Pp(Omega),  und Messbarkeit ist automatisch erfüllt. Für  Omega aus RR^n  wählen wir  Ff = Bb(RR^n),  und  X  ist Prinzip ?? in Analysis I  (f to X.. f(x) to X(omega)).  

*Def*.. Sei  (Omega, Ff, PP)  ein W'keitsraum. Eine Abbildung  X : Om to RR  heißt **Zufallsvariable**.

Bmk.. Für Zufallsvariablen  X  gilt  X^-1(k) in Ff  für alle  k in RR.  

*Def*.. Eine Zufallsvariable  X  heißt **diskret**, falls  X(Om)  endlich oder abzählbar unendlich.

*Def*.. Sei  X  eine diskrete Zufallsvariable auf  (Om, Ff, PP).  Die Funktion  k in RR mapsto PP(X = k)  heißt **Massenfunktion von _X_**.. Wir nennen wie  quine{p_X}.  

%> Bsp.. Wir haben eine Urne mit 20 nummerierten Kugeln. Wir ziehen 3x ohne Zurücklegen. Wir suchen die Wkt, dass wir eine Kugel mit Nr.  >= 17  ziehen. Haben also Laplace-Experiment mit  Om = \{1, ..., 20\}^3.  Wählen die Zufallsvariable  X  mit  X(om) = max om.  Suchen also die Wkt  PP\{X(om) >= 17\} = p_X(17) + ... + p_X(20).  Berechnen zuerst  p_X(20).  Die Gegenwkt ist  frac{19}{20} cdot frac{18}{19} cdot frac{17}{18} = frac{17}{20}.  Also  p_X(20) = 1 - frac{17}{20} = frac{3}{20}.  Ein alternativer Rechenweg stellt fest, dass dieses Ereignis aus  binom{19}{2}  günstigen Realisierungen besteht, bei  binom{20}{3}  möglichen Realisierungen. Also  p_X(20) = frac{binom{19}{2}}{binom{20}{3}} = frac{3}{20}.  Analog gilt für  i in \{17, 18, 19\},  dass  p_X(i) = frac{binom{i - 1}{2}}{binom{20}{3}}.  

%> Bsp.. Wir werfen eine Münze so lange, bis "Kopf" erscheint, maximal jedoch _n_-mal. "Kopf" erscheint mit Wkt  p in (0, 1).  Sei  X(om)  die Anzahl der Würfe. Wir suchen  p_X(m)  für  m = 1, ..., n.  Da wir für das Ereignis  \{X(om) = m\}  zuerst  m - 1  Mal "Zahl" geworfen (Wkt.  1 - p)  haben müssen, und daraufhin "Kopf" (Wkt  p),  gilt  p_X(m) = (1 - p)^{m - 1}.  Allerdings nicht für den Fall  m = n,  denn dort brauchen als letzten Wurf nicht unbedingt "Kopf". Also  p_X(n) = (1 - p)^{n - 1}..  Es gilt dann  PP(bigcup_{i = 1}^n \{X(om) = i\}) = sum_{i = 1}^n PP\{X(om) = i\} = 1.  

%> Bsp.. Es gibt  N  unterscheidbare Coupons. Wir sammeln diese (unabhängig). Sei  T(om)  die Anzahl der Coupons, die wir gesammelt haben, bis wir ein vollständiges Set von  N  verschiedenen Coupons haben. Wir suchen  PP\{T(om) = n\}  für  n = N, N + 1, ...  . Es ist einfacher  PP \{T(om) > n\}  zu berechnen. (Es gilt dann  PP\{T(om) = n\} = PP\{T(om) > n - 1\} - PP\{T(om) > n\}.)  Es sei  A_j  das Ereignis, dass sich kein *j*-Coupon unter den ersten  n  Versuchen befindet. Dann gilt  PP\{T(om) > n\} = PP(bigcup_{j = 1}^N A_j) = ... = N(frac{N - 1}{N})^n - binom N 2 (frac{N - 2}{N})^n + ... + (-1)^N binom{N}{N - 1}(frac{N - (N - 1)}{N})^n + 0.  

*Def*.. Sei  X  eine diskrete Zufallsvariable auf  (Om, Ff, PP).  Die Zahl  EE(X) := sum_{x in X(Om)} x cdot p_X(x)  heißt **Erwartungswert von _X_**, falls diese Reihe absolut konvergiert, das heißt  sum_{x in X(Om)} |x| cdot p_X(x) < infty.  

%> Bsp.. Sei  A aus Om.  Wir definieren als Zufallsvariable die Indikatorfunktion  I_A : Om to \{0, 1\}  mit  I_A(om) = 1,  falls  om in A  und  I_A(om) = 0,  sonst. Dann gilt  p_{I_A}(0) = PP(A^C) = 1 - PP(A)  und  p_{I_A}(1) = PP(A).  Also nach Definition  EE I_A = 0 cdot (1 - PP(A)) + 1 cdot PP(A) = PP(A).  

# Nov. 20

*Def*.. Sei  X  eine Zufallsvariable auf  (Om, Ff, PP).  Die Funktion  k in RR mapsto PP(X <= k)  heißt **Verteilungsfunktion von _X_**  (F_X).  

*Eigenschaften*.. Die Verteilungsfunktion einer Zufallsvariable  X  ist monoton wachsend und rechtsseitig stetig mit  lim_{x to infty} F_X(x) = 1  und  lim_{x to -infty} F_X(x) = 0.  

% Folgen von Zufallsvariablen, die Indikatorfunktionen sind

%Def.. Sei  n in NN  und  p in (0, 1).  Eine Zufallsvariable  X  heißt  (n, p)  -**binominalverteilt**, falls für jedes  k in NN  gilt::  PP(X = k) = binom n k p^k (1-p)^{n-k}..  Schreiben dann  quine{X ~ B(n, p)}.  
*Def*.. Sei  n in NN  und  p in (0, 1).  Eine Zufallsvariable  X  mit der Massenfunktion  k in RR mapsto binom n k p^k (1-p)^{n-k}  heißt  (n, p)  -**binominalverteilt**  (X ~ B(n, p)).  

%Def.. Eine Zufallsvariable  X  heißt **binomialverteilt** gdw. es gibt  n  und  p  mit  X ~ B(n, p).  

%Bmk..  X ~ B(n, p) \; <=> \; F_X(x) = sum_{k=0}^x binom n k p^k (1-p)^{n-k}.  

*Erwartungswert und Varianz*.. Für  X ~ B(n, p)  gilt  EE(X) = n  und  Var(X) = n p (1-p).  

*Erfolg-Misserfolg-Versuchsreihen sind binomialverteilt*.. Sei  X  die Zufallsvariable, die die Anzahl der Erfolge (Eintritt mit W'keit  p)  in einer Versuchsreihe der Länge  n  misst, das heißt  Om = set{0, 1}^n  und  X(om) = sum om.  Dann gilt  X ~ B(n, p).  

*Bild von Binomial-ZV*.. Für binomialverteilte Zufallsvariablen  X  gilt  X(Om) aus NN.  

*Verlauf der Binomial-Massenfunktion*.. Für  X sim B(n, p)  ist die Massenfunktion  p_X  monoton wachsend auf  [0, (n + 1)p]  und monoton fallend auf  [(n + 1)p, infty).  

% Binomialverteilungen mit großem n und kleinem p
*Def*.. Sei  lam > 0.  Eine Zufallsvariable  X  mit der Massenfunktion  k mapsto exp(-lam) frac{lam^k}{k!}  heißt **Poisson-verteilt** mit Parameter  lam..  Schreiben dann  quine{X sim pi(lam)}.  

% Stimmt das? Genauer: Kann ich das wirklich in die Bemerkung verschieben, oder muss das in die Definition rein?
*Bild von Poission-ZV*..  X ~ pi(lam) => X(Om) sse ZZ^+.  

# Nov. 25

% eine Binomialverteilung ist die Massenfunktion einer binomialverteilten ZV.
*Approximation einer Binomialverteilung durch eine Poissonverteilung*.. Für  n p_n overset{n to infty}{longrightarrow} lam  gilt  binom n k p_n^k (1-p_n)^{n-k} overset{n to infty}{longrightarrow} exp(-lam) frac{lam^k}{k!}  (*n* muss also groß sein).

*Erwartungswert und Varianz*.. Für  X sim pi(lam)  gilt  EE(X) = Var(X) = lam.  

*Def*.. Sei  n in NN  und  X_n sim B(n, p).  Dann definieren wir  X_n^* := frac{X_n - n p}{sqrt{n p (1-p)}}.  

*Def*..  phi(x) := frac{1}{sqrt{2 pi}} exp(-frac{x^2}{2})  für  x in RR.  

**Satz von deMoivre/Laplace**.. Sei  p = frac 1 2.  Sei  X_n sim B(n, p)  für alle  n in NN.  Dann gilt für  a, b in RR  mit  a < b:: {lim_{n to infty}} PP(a <= X_n^*(om) <= b) = int_a^b phi(x) d x.  

Bmk.. (i)  int_{-infty}^infty phi(x) = 1..  (ii) Theorem gilt auch für  p in (0, 1).  

*Def*.. Für Folgen  (a_n)  und  (b_n)  schreiben wir  quine{a_n sim b_n},  falls  lim_{n to infty} frac{a_n}{b_n} = 1.  

**Stirling-Formel**..  n! sim sqrt{2 pi n}(frac n e)^n.  

# Nov. 27

(Beweis der Stirling-Formel.)

# Dez. 2

# Dez. 4

# Dez. 9

*Def*.. Sei  mu in RR  und  sigma > 0.  Eine Zufallsvariable  X  mit der Dichtefunktion  x mapsto frac{1}{sqrt{2 pi sigma^2}} exp (-frac{(x - mu)^2}{2 sigma^2})  heißt **normalverteilt** mit Parametern  (mu, sigma)..  Schreiben dann  quine{X sim Nn(mu, sigma)}..  

*Def*.. Eine Zufallsvariable  X  mit  X ~ Nn(0, 1)  heißt **standardnormalverteilt**. Ihre Dichtefunktion  x mapsto frac{1}{sqrt{2 pi}} exp(-frac{x^2}{2})  nennen wir  text{„}phi text{“}  und ihre Verteilungsfunktion  z mapsto int_minfty^z frac{1}{sqrt{2 pi}} exp(-frac{x^2}{2})  nennen wir  text{„}Phi text{“}.  

*Erwartungswert und Varianz*.. Für  X sim Nn(mu, sigma)  gilt  EE(X) = mu  und  Var(X) = sigma^2.  

*Linearität*.. Sei  alpha > 0  und  beta in RR..  Wenn  X ~ Nn(mu, sigma),  dann  (alpha X + beta) ~ Nn(alpha mu + beta, alpha sigma).  

% Das hier ist irgendwie Quatsch. Nochmal prüfen.
*Normierte Binomial-Zufallsgröße*.. Für jedes  X ~ B(n, p)  gibt es ein  Z ~ Nn(0, 1)  mit  limn PP(a <= frac{X - n p}{sqrt{n p (1-p)}} <= b) = PP(a <= Z <= b).  
% „Die Binomialverteilung lässt sich durch die Standardnormalverteilung approximieren“?

*Approximation einer Binomialverteilung durch die Standardnormalverteilung*.. Für  X ~ B(n, p)  gilt  PP(X = k) approx Phi(frac{i - onehalf - n p}{sqrt{n p (1-p)}}) - Phi(frac{i + onehalf - n p}{sqrt{n p (1-p)}}).  
% = PP(i - onehalf < X < i + onehalf)

# Dez. 11

(Zwischenklausur.)

# Dez. 16

%Prop.. Für  X ~ B(n, p)  gilt  limn PP(frac{X_n - n p}{sqrt{n p (1-p)}}) = 1 - Phi(a).  
Prop.. Für  B(n, p)  -verteilte Zufallsvariablen  X  gilt  limn PP(frac{X_n - n p}{sqrt{n p (1-p)}} >= a) = 1 - Phi(a).  
%Prop.. Für  (n, p)  -binomialverteilte Zufallsvariablen  X  gilt  limn PP(frac{X_n - n p}{sqrt{n p (1-p)}}) = 1 - Phi(a).  

%> Bsp: Berliner für ein Alkoholverbot.

*Def*.. Sei  lam > 0.  Eine absolutstetige ZV  X  mit der Dichtefunktion  x mapsto lam exp(-lam x)  für  x >= 0,  sonst  x mapsto 0,  heißt **exponentialverteilt** mit Parameter  lam..  Schreiben dann  quine{X ~ E(lam)}.  

*Bild von Exponential-ZV*..  X ~ E(lam) => X(Om) sse [0, infty).  

*Erwartungswert und Varianz*.. Für  X sim E(lam)  gilt::  EE(X) = frac 1 lam  und  Var(X) = frac{1}{lam^2}.  

% „Erinnerung: Eine ZV  X ~ G(p)  ist gedächtnislos.“ Was ist G(p)?

*Gedächtnislosigkeit*.. Für  X ~ E(lam)  und  s, t > 0  gilt::  PP(X > s+t | X > t) = PP(X > s).  
% Beweis: Bayes, Def.  X ~ E(lam), Potenzrechnung.

Lemma.. Sei ZV  Y >= 0.  Dann gilt  EE(Y) = int_0^infty PP(Y > y) d y.  
% (Vgl. Satz von Fubini.)

# Dez. 18

(Mehrdimensionale Integration.)

# Jan. 6

% Confused stuff...

*Def*.. Seien  X, Y  Zufallsvariablen auf   (Om, Ff, PP).  Die Funktion  (a, b) mapsto PP(X <= a, Y <= b)  heißt die **gemeinsame Verteilungsfunktion** von  X  und  Y.  

*Def*.. Seien  X, Y  Zufallsvariablen mit der gemeinsamen Verteilungsfunktion  F.  Dann heißen die Funktion  F_X : RR to [0, 1]  mit  F_X(a) := F(a, infty) := limn F(a, n)  und analog  F_Y  ihre **Randverteilungen**.

Bmk..  PP(a_1 < X <= a_2, b_1 < Y <= b_2) = F(a_2, b_2) - F(a_1, b_2) - F(a_2, b_1) + F(a_1, b_1).  

% Man muss diese Funktionskennzeichnungsterme wohl erlauben.
*Def*.. Seien  X, Y  diskrete Zufallsvariablen. Die Funktion  (x, y) mapsto PP(X = x, Y = y)  heißt **gemeinsame Massenfunktion** (*p*).
%*Def*.. Die **gemeinsame Massenfunktion** zweier diskreter Zufallsvariablen  X, Y  ist die Funktion  p(x, y) = PP(X = y, Y = y).  

*Def*.. Sei  p  die gemeinsame Massenfunktion von  X  und  Y.  Die Funktion  displaystyle x mapsto sum_{y : p(x, y) > 0} p(x, y)  heißt *X*-**Randverteilung**  (p_X).  Analog  p_Y.  
%*Def*.. Die **Randverteilungen** der gemeinsamen Massenfunktion von  X  und  Y  sind die Funktionen  p_X(x) = sum_{y : p(x, y) > 0} p(x, y)  und analog  p_Y.  

%# Jan. 6 Übung

%(Integration)

# Jan. 8

*Def*.. Seien  X, Y  Zufallsvariablen auf  (Om, Ff, PP).  Sie heißen **gemeinsam absolut-stetig verteilt mit Dichte**  f: RR^2 to RR_+,  falls  PP((X, Y) in C) = int_C (x, y) d(x, y)  für jedes  C sse RR^2.  

*Def*.. Für  C = (-infty, a] times (-infty, b]  setzen wir  PP(X <= a, Y <= b) = F(a, b) = int_minfty^a int_minfty^b f(x, y) d y\ d x.  

Prop.. Ist  f  stetig, so gilt  f(x, y) = frac{partial^2}{partial x partial y} F(x, y).  

*Def*.. Die **Randverteilung** von  X  ist  F_X(x) = PP(X <= x, Y <= infty) = int_minfty^x (int_RR f(t, y) d y) d t.  

Prop.. Falls  f  stetig:  F_X' = f_X.  

*Def*.. Zwei ZV sind **unabhängig**.
