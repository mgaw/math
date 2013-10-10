Titel: Lina 2
Layout: cm small


*Def*.. Ein Schema der Form ... heißt **Matrix** reeller Zahlen mit  m  Zeilen und  n  Spalten, kurz:  m times n  -Matrix,  i  ist Zeilenindex,  j  Spaltenindex, Spaltenvektoren, Zeilenvektoren. Menge aller reellen  m times n  -Matrizen:  RR^{m times n}.  

*Def*.. Matrix **quadratisch**, falls  m = n.  

*Def*.. Quadratische Matrix. Sind alle  a_{i j}  mit  i != j  gleich Null, so heißt diese Matrix **Diagonalmatrix**:  mat{a_{1 1} & & 0 \\ & ddots & \\ 0 & & a_{n n}}  

*Def*.. Matrix **symmetrisch**, falls  A = A^T.  

*Def*.. **Zeilenrang**, **Spaltenrang**.

*Folg*.. Der Spaltenrang einer Matrix ist gleich der Dimension des von den Spaltenvektoren erzeugten linearen Unterraums  spn(a_{s 1}, ..., a_{s n}).  


*Satz*.. Vektoren sind linear unabhängig  <==>  Lineare Hülle hat "volle" Dimension  <==>  Linearkombinations-Vektorgleichung ist eindeutig lösbar  <==>  Linearkombinations-Vektorgleichung hat nur die triviale Lösung  <==>  Bei Gauß-Verfahrens-Matrix  mat{... & | & 0 \\ ... & | & 0}  verschwindet *keine* Zeile  <==>  Matrix ist regulär, d.h. hat vollen Rang  <==>  Kern der Abbildung ist  \{varnothing\} <==>  Abbildung ist invertierbar, d.h. ist bijektiv  <==>  Determinante ist *nicht* Null  <==>  Matrix ist invertierbar.


*Satz*.. Zeilenrang = Spaltenrang.

*Def*.. Eine quadratische  n times n  -Matrix heißt **regulär**, falls  rg A = n.  

*Satz*..  (A B) v = A (B v).. lam (A B) = (lam A) B = A (lam B) = (A B) lam.  

*Satz*..  (A B)^T = B^T A^T.  


*Bmk*.. Kann nur multiplizieren, wenn Spalten links = Zeilen rechts. Also  A in RR^{l times m} cdot B in RR^{m times n}  geht.

*Satz*.. Matrizenmultiplikation ist *nicht* nullteilerfrei.

*Satz*.. Das Produkt regulärer Matrizen (voller Rang) ist wieder reguläre Matrix, also insbesondere nullteilerfrei.




*Def*.. Elementarmatrix  S_i(lam) :=  "passende" Einheitsmatrix mit  a_{i i} = lam.  

*Satz*.. Multiplikation mit  S_i(lam)  von links entspricht Multiplikation der *i*-ten Zeile mit  lam.  Multiplikation mit  S_i(lam)  von rechts entspricht Multiplikation *i*-ter Spalte mit  lam.  

*Def*.. Elementarmatrix  Q_i^j :=  "passende" Einheitsmatrix mit  a_{i j} = 1.  

*Satz*.. Multiplikation mit  Q_i^j  von links entspricht Addition von *j*-ter Zeile zu *i*-ter Zeile. Multiplikation mit  Q_i^j  von rechts entspricht Addition von *i*-ter Spalte zu *j*-ter Spalte.

*Def*.. Elementarmatrix  Q_i^j(lam) :=  Einheitsmatrix mit  a_{i j} = lam.  

*Def*.. Elementarmatrix  P_i^j :=  Einheitsmatrix mit  a_{i j} = 1, \; a_{j i} = 1.  

*Bmk*.. Generell: Multiplikation mit Elementarmatrizen von links sind Zeilenumformungen, von rechts sind Spaltenumformungen.

*Satz*.. Alle Elementarmatrizen sind regulär.

*Satz*.. Jede reguläre Matrix lässt sich als Produkt von Elementarmatrizen darstellen.

*Satz*.. Alle vier Elementarmatrizen sind invertierbar und ihre Inversen sind Produkte von Elementarmatrizen.


*Satz*..  (RR^{n times m}, +, cdot)  ist Vektorraum.

Inverse Matrizen.

*Satz*.. Eindeutigkeit der Inversen.

*Satz*.. Matrix genau dann invertierbar, wenn sie regulär ist.

*Satz*.. Die Menge der regulären quadratischen Matrizen ist eine Gruppe.

*Satz*.. Elementarmatrizen sind invertierbar. Die Inverse ist selber wieder Elementarmatrix.

*Satz*.. Eine Matrix ist invertierbar genau dann, wenn sie sich als Produkt von Elementarmatrizen darstellen lässt.

**Dimensionssatz**..  V  und  W  VR,  f: V to W  lin. Abb. und  dim(V) < infty.  Dann gilt:  dim V = dim Im f + dim Ker f.  

*Def*.. VR  V  heißt **isomorph** zu VR  W,  falls es eine bijektive lineare Abbildung  f : V -> W  gibt.

*Def*.. Sei  V  endlich-dimensionaler VR. Dann heißt  V^* := \{T : V to RR : T text{ ist linear}\}  **Dualraum von _V_**.

*Satz*..  V^*  ist Unterraum von  \{f : V to RR\}  und  dim V^* = dim V.  

*Def*.. Der von den Zeilen einer Matrix aufgespannte VR heißt **Zeilenraum**. Analog **Spaltenraum**. Die Lösungsmenge des LGS  A x = 0  heißt **Nullraum**.

*Satz*.. Zeilenumformungen ändern nicht den Zeilenrang, aber möglicherweise den Spaltenrang.


*Def*..  f : V to W  linear, falls Additivität und Homogenität.

*Bsp*..  f : RR^2 to RR^2, \; mat{x \\ y} mapsto mat{a x + b y \\ c x + d y}  ist linear für alle  a, b, c, d in RR.. f  injektiv  <==> ... = ... => ... = ... <==>  [LGS] eindeutig lösbar  <==> mat{a & b \\ c & d}  ist regulär..  f  surjektiv  <==> forall ... exists ... <==>  [LGS] lösbar  <==> mat{a & b \\ c & d}  ist regulär (?).

*Def*.. Lineare Abbildung heißt **Monomorphismus**, falls injektiv. **Epimorphismus**, falls surjektiv. **Isomorphismus**, falls bijektiv. **Automorphismus**, falls bijektiv und  f : V to V.  

*Satz*.. VR  V, \; W  und  f : V to W  linear.. (i) Lineare Abbildungen respektieren Linearkombinationen:  f(sum_{i = 1}^k lam_i u_i) = sum_{i = 1}^k lam_i f(u_i)..  (ii) Sind  u_i, ..., u_k  linear abhängig, so sind auch  f(u_1), ..., f(u_k)  linear abhängig.. (iii)  U ≤ V \;=>\; f(U) ≤ W..  (iv)  f(spn(u_1, ..., u_k)) = spn(f(u_1), ..., f(u_k)).  


**Hauptsatz über lin. Abb**.. Seien  V, W  VR,  B = \{b_1, ..., b_n\}  eine Basis von  V  sowie  w_1, ..., w_n  beliebige Vektoren von  W.  Dann existiert *genau eine* lineare Abbildung  f : V to W  mit  f(b_i) = w_i  für  1 <= i <= n.  


Matrizielle Darstellung lin. Abb.

*Def*.. Sei  V  VR,  v in V,, B = \{b_1, ..., b_n\}  Basis von  V.  Die **Koordinaten von _v_ bzgl. _B_** ist der Spaltenvektor  [v]_B = mat{lam_1 \\ vdots \\ lam_n},  so dass gilt  lam_1 b_1 + ... + lam_n b_n = v.  

*Def*.. Sei  f : V to W,, B  Basis von  V,, C  Basis von  W.  Die **Abbildungsmatrix von _f_ bzgl. _B_ und _C_** ist die Matrix  A^f_{B C},  so dass gilt  A^f_{B C} cdot [v]_B = [f(v)]_C.  


*Satz*.. Nacheinanderausführung linearer Abbildungen ist wieder linear.



*Satz*.. Die Menge der Isomorphismen  f : V -> V  ist eine Gruppe bzgl. Nacheinanderausführung.. Die Menge der regulären  n times n  -Matrizen ist eine Gruppe bzgl. Multiplikation.. Diese beiden Gruppen sind isomorph (bzgl. einer festgelegten Basis von  V).  

*Def*..  V  Vektorraum,  B, B'  Basen von  V,, v in V.  **Transformationsmatrix von _B_ nach _B'_** ist die Matrix  T_{B'}^B,  so dass  T_{B'}^B cdot [v]_B = [v]_{B'}.  

**Berechnung von**  T_{B'}^B..  Es seien  B = (b_1, ..., b_n)  und  B' = (b_1', ..., b_n')  zwei Basen von VR  V..  Die Elemente von  B  als Linearkombination bzgl.  B'  schreiben:  b_j = sum_{i = 1}^n t_{i j} b_i'..  Das schreibe ich in die Spalten der Matrix:  T_{B'}^B := (t_{i j})_{1 ≤ i, j ≤ n}.  (In den Spalten von  T_{B'}^B  stehen die Koordinaten der Elemente von  B  bzgl.  B'.)  

*Satz*..  T_{B'}^B = A_{B B'}^f  mit  f : V to V,, f(b_i) = b_i',, 1 <= i <= n.  

*Satz*..  T_{B'}^B = A_{B B'}^{Id}.  

*Bsp*..  T_{B'}^B = mat{frac{1}{sqrt 2} \;& -frac{1}{sqrt 2} \\ frac{1}{sqrt 2} & frac{1}{sqrt 2}}  ist die Drehmatrix um 45 Grad.


**Basistransformationsformel**..  A^f_{B' B'} = T^B_{B'} cdot A^f_{B B} cdot T^{B'}_B.  (?)

*Satz*..  (T_B^{B'})^{-1} = T_{B'}^B.  





*Def*.. Zwei Matrizen  A  und  B  heißen **ähnlich**, falls es eine Matrix  S  gibt, so dass  A = S^{-1} A S.  Schreiben  A sim B.  

*Satz*.. Die Ähnlichkeit von Matrizen ist Äquivalenzrelation.

*Satz*.. Zwei Matrizen sind genau dann ähnlich, wenn sie bzgl. bestimmter Basen dieselbe lin. Abb. beschreiben.

*Bmk*.. Alle Matrizen gleichen Ranges sind zueinander ähnlich.

*Satz*.. Es gibt genau eine Abbildung mit (D1) linear in jeder Spalte,, (D2) alternierend, d.h. zwei gleiche Spalten  => det A = 0  und (D3) normiert, d.h.  det E_n = 1.  

*Def*.. Diese Abbildung (falls sie existiert), heißt **Determinante**(nfunktion).

Satz.. Eine Determinantenfunktion  det  hat die folgenden weiteren Eigenschaften.. (i)  det(lam A) = lam^n det(A)..  (ii) Ist eine Zeile von  A  gleich Null, so ist  det A = 0..  (iii) Entsteht  B  aus  A  durch (genau eine) Zeilenvertauschung, so ist  det B = - det A..  (iv) Ist  lam in K  und entsteht  B  aus  A  durch Addition der  lam text{-fachen}  *j*-ten Zeile zur *i*-ten Zeile  (i neq j),  so ist  det B = det A..  (v) Ist  A  eine obere Dreiecksmatrix,  A = mat{lam_1 & & * \\ & ddots & \\ 0 & & lam_n},  so ist  det A = lam_1 cdot ... cdot lam_n..  (vi) Sei  n ≥ 2  und  A in M(m, n : K)  von der Gestalt  A = mat{A_1 & C \\ 0 & A_2},  wobei  A_1, A_2  quadratisch. Dann gilt  det A = det(A_1) cdot det(A_2)..  (vii)  det A = 0 <=> Rang(A) < n <=>  Zeilenvektoren sind linear abhängig.

*Satz*.. Matrix  A  regulär gdw.  det A != 0.  

*Satz*..  A  Matrix.  det A = det A^T.  


*Def*..   K  Körper,  V  *K*-Vektorraum,  f : V to V  lineare Abbildung.  lam in K  heißt **Eigenwert von _f_**, falls es  v in V, \; v != 0  gibt, so dass  f(v) = lam v..  Diese  v  heißen **Eigenvektoren zu**  lam.  

%. \; \{v in V : f(v) = lam v \} = ker(f - lam Id)  heißt **Eigenraum zu**  lam.  

% (Identifizieren  f  mit Matrix zu einer Basis  B.  Ziel: Basis finden, so dass die Matrix der Abbildung diagonal ist.)

*Lemma*.. Sei  A  die Matrix von  f : V to V  bzgl. einer Basis  (v_1, ..., v_n)  von  V,  dann hat  A  Diagonalgestalt, d.h.  A = mat{lam_1 & & 0 \\ & ddots & \\ 0 & & lam_n},  wenn  v_i  Eigenvektor zum Eigenwert  lam_i  ist  (1 <= i <= n).  

% Satz..  V  endlichdimensional,  A  eine zu  f  gehörige Matrix.  f(v) = lam v <=> A x = lam x <=> A x = lam E x <=> (A - lam E)x = 0.  

*Lemma*.. Ein Vektor  v in V setminus \{0\}  ist genau dann Eigenvektor von  f : V to V  zum Eigenwert  lam in KK,  wenn  v in ker(f - lam Id).  

*Def*.. Ist  lam  ein Eigenwert von  f,  dann heißt der Untervektorraum  E_lam := ker(f - lam Id)  von  V  der **Eigenraum** von  f  zum Eigenwert  lam,  und  beta_lam := dim E_lam  heißt **geometrische Vielfachheit von**  lam.  

% Def..   det(A - lam E)  heißt das **charakteristische Polynom von _f_**.

% Satz.. Die Nullstellen des charakteristischen Polynoms sind die Eigenwerte von  f.  

% >  (A - lam E)x = 0  ist lösbar  (x != 0)  genau dann, wenn  det(A - lam E) = 0.  

% Def.. Die *n*-fachheit einer Nullstelle  lam  im charakteristischen Polynom heißt die **algebraische Vielfachheit** dieses Eigenwertes.

% Def.. Eine quadratische Matrix  A  heißt **diagonalisierbar**, falls es eine Diagonalmatrix gibt, die zu  A  ähnlich ist.

% Satz.. Eine *n*-dimensionale Matrix  A  ist genau dann diagonalisierbar, wenn es  n  linear unabhängige Eigenvektoren von  A  gibt (eine Basis aus Eigenvektoren).

*Lemma*.. Seien  v_1, ..., v_r  Eigenvektoren zu Eigenwerten  lam_1, ..., lam_r  von  f  und gelte  lam_i != lam_j  für  i != j,  dann ist  (v_1, ..., v_r)  linear unabhängig (EV zu paarweise verschiedenen EW sind lin. unabh.).

*Folg*..  f : V to V  Endomorphismus mit  dim V = n  über  KK,, lam_1, ..., lam_r  seien die EW und  n_1, ..., n_r  seien die geom. Vielfachheiten, d.h.  n_i = dim E_{lam_i}.  Sei jeweils  (v_1^{(i)}, ..., v_{n_i}^{(i)})  Basis von  E_{lam_i}..  Dann ist auch  (v_1^{(1)}..v_{n_1}^{(1)}, ..., v_1^{(r)}..v_{n_r}^{(r)})  linear unabhängig (d.h. Menge von EV zu versch. EW sind lin. unabh.).. Insbesondere ist  n_1 + ... + n_r ≤ n quad  und  quad f  diagonalisierbar  <=> n_1 + ... + n_r = n.  

*Def*..  f  Endomorphismus.  A  Matrix von  f  zu beliebiger Basis. Dann  det f := det A.  (Determinante ist unabhängig von Basis.)

*Satz*..  lam  ist EW zu  f  genau dann, wenn  det(f - lam Id) = 0.  


*Def*.. Wird  f  bzgl. einer Basis von  V  durch die Matrix  A  beschrieben, so ist  P_f(lam) = P_A(lam) = det(f - lam Id_V)  das **charakteristische Polynom** von  f.  

*Satz*.. Das charakteristische Polynom eines Endomorphismus  f  ist unabhängig von der Wahl der Basis, bzgl. der  f  durch eine Matrix  A  beschrieben wird.

*Satz*.. Es gibt Koeffizienten  a_0, ..., a_{n - 1},  so dass  P_f(lam) = (-1)^n lam^n + a_{n-1} lam^{n-1} + ... + a_1 lam + a_0..  Die Eigenwerte einer linearen Abbildung bzw. einer Matrix sind die Nullstellen des charakteristischen Polynoms.

*Def*.. Sei  f in L(V, V)  und  lam_0  sei ein EW von  f,  d.h.  lam_0  ist Nullstelle des char. Polynoms  P_f(lam) = det(f - lam Id)..  Dann ist  (lam - lam_0)  ein Teiler von  P_f(lam).  Der maximale ganzzahlige Exponent  alpha_{lam_0}  mit  (lam - lam_0)^{alpha_{lam_0}} | P_f(lam)  heißt **algebraische Vielfachheit** des EW  lam_0.  

*Satz*.. Die geometrische Vielfachheit eines EW ist  ≤  der algebraischen Vielfachheit.

*Def*.. Ein Endomorphismus  f in L(V, V)  heißt **diagonalisierbar**, falls  V  eine Basis besitzt, die vollständig aus EV von  f  besteht.

*Def*.. Eine Matrix  A in RR^{n times n}  heißt **diagonalisierbar**, falls eine ähnliche Diagonalmatrix  D  existiert, das heißt es gibt eine (invertierbare) Matrix  S in RR^{n times n},  so dass  S^{-1} A S = D.  

*Satz*.. Eine solches Matrix  S  ist gegeben durch eine Basis aus EV. (?)

*Satz*..  f in L(V, V)  ist diagonalisierbar gdw. für jeden EW die algebraische und geometrische Vielfachheit übereinstimmen. Insbesondere ist jeder Endomorphismus mit  n = dim V  paarweise verschiedenen EW diagonalisierbar.

*Def*.. Eine **positiv definite symmetrische Bilinearform** (verallgemeinertes Skalarprodukt) auf einem reellen VR ist eine Abbildung  B : V times V to RR  mit:: (B1)  B(u + v, w) = B(u, w) + B(v, w)  (Additivität) und  B(lam u, v) = lam B(u, v)  (Homogenität) (Linearität im ersten Argument).. (B2)  B(u, v) = B(v, u)  (Symmetrie).. (B3)  B(u, v) ≥ 0  sowie  B(u, u) = 0 <=> u = 0  (positiv definit).

*Bmk*.. Wegen der Symmetrie gilt auch die Linearität im zweiten Argument.

*Def*.. Ein VR  V  mit einer pos. def. symm. BLF  B  heißt **euklidischer VR**  (V, B).  Ein affiner Punktraum mit pos. def. symm. BLF heißt **euklidischer Punktraum**  (A, V, B).  

*Satz*.. Für die positiv definite BLF eines Vektors  x  mit einer Linearkombination aus Vektoren  x = sum_{i = 1}^k lam_i v_i  gilt  B(x, sum_{i = 1}^k lam_i v_i) = sum_{i = 1}^k lam_i B(x, v_i).  

*Def*.. Wir nennen positiv definite BLF in Zukunft **Skalarprodukte** und schreiben dafür  a cdot b  oder  langle a, b rangle.  

*Satz*..  V  sei euklidischer VR mit Skalarprodukt  `cdot´  und  B = \{b_1, ..., b_n\}  eine Basis von V. Wenn alle Skalarprodukte  b_i cdot b_j \;(1 <= i, j <= n)  der Basisvektoren gegeben sind, so ist das Skalarprodukt zweier beliebiger Vektoren von  V  eindeutig bestimmt.

*Def*.. Es sei  u in V  (eukl. VR mit SP). Dann heißt  |u| := sqrt{u cdot u}  der **Betrag** von  u.  Sind  P  und  Q  zwei Elemente eines affinen Raumes, so nennt man den Betrag des Vektors  ora{P Q}  ihren **Abstand**.

**Cauchy-Schwarz-Ungleichung**.. Für beliebige Vektoren  u, v  eines eukl. VR gilt, dass  |u cdot v| ≤ |u| cdot |v|.  Gleichheit gilt gdw.  u  und  v  lin. abhängig.


% Wir benutzen Transformationsmatrizen, um das Skalarprodukt zu berechnen.  =>  Gramsche Matrix eines SP bzgl.  B  bzw.  B'.  

% Dimensionssatz und Eigenraum.

**Dreiecksungleichung**.. Für beliebige Vektoren  u, v  eines eukl. VR gilt  |u + v| ≤ |u| + |v|.  

*Def*.. Zwei vom Nullvektor verschiedene Vektoren  u, v  eines euklidischen VR heißen **orthogonal** genau dann, wenn  u v = 0.  

% Bsp.. Beweis Satz des Pythagoras: ...

*Def*.. Es seien  u, v  zwei versch. Vektoren eines eukl. VR. Als **Winkelmaß** dieser Vektoren bezeichnet man die Zahl  phi  mit  cos phi = frac{u cdot v}{|u| cdot |v|}  (mit  -pi < phi < pi).  

% (Diese Definition wird durch die Cauchy-Schwarz-Ungleichung gerechtfertigt.)

% Bsp.. Beweis Kosinussatz: In jedem bel. Dreieck gilt  a^2 = b^2 + c^2 - 2 b c cos alpha.  

*Def*.. Es sei  (V, cdot)  ein eukl. VR. Eine Basis  B = \{b_1, ..., b_n\}  von  V  heißt **Orthonormalbasis**, falls:: (i) Alle Basisvektoren sind Einheitsvektoren, d.h.  |b_1| = ... = |b_n| = 1..  (ii) Alle Basisvektoren sind paarweise orthogonal zueinander, d.h.  b_i b_j = 0  für  i neq j, \; 1 <= i, j <= n.  

*Def*.. Ein Koordinatensystem  K = \{0, b_1, ..., b_n\}  eines affinen Raumes heißt **karthesisches Koordinatensystem**, falls  \{b_1, ..., b_n\}  eine ON-Basis ist.


*Def*.. Seien  V, W  eukl. VR. Eine lin. Abb.  f : V to W  heißt **orthogonale Abbildung**, falls für alle  u, v in V  gilt, dass  f(u) f(v) = u v.  

*Satz*.. Jede orthogonale Abbildung ist injektiv, eine orthogonale Abbildung  f : V to V  ist ein Isomorphismus.

Bezeichnungen..  O(V)  ist die Menge aller orthogonalen Abb.  V to V.. O(n)  ist die Menge aller orthogonalen Abb. in  RR^n  bzgl. des Standardskalarprodukts.. Als **orthogonale Matrizen** bezeichnen wir Matrizen orthogonaler Abb. bzgl. des Standardskalarprodukts.

*Satz*.. Jede betragstreue lin. Abb., d.h. jede lin. Abb. mit  f : V to W  mit  |f(u)| = |u|  für alle  u in V,  ist eine orthogonale Abbildung.

*Satz*.. Sind  V, W  eukl. VR und  B = \{b_1, ..., b_n\}  eine ON-Basis von  V,  so ist eine lineare Abb.  f : V to W  genau dann orthogonal, falls  \{f(b_1), ..., f(b_n)\}  ein ON-System in  W  und damit eine ON-Basis von  Im f.  

*Folg*.. Eine  n times n  -Matrix ist genau orthogonal, wenn die *Spalten* ein ON-System bilden.

*Folg*.. (i) Ist  A  eine orthogonale Matrix, so gilt  A^T cdot A = E_n..  (ii)  A^{-1} = A^T..  (iii)  det A = +- 1.  

*Def*.. Orthogonale Abbildungen, die durch orthogonale Matrizen mit positiver Determinante (1) beschrieben werden, heißten **ordnungserhaltend**, solche mit  det A = -1  **ungleichsinnig**.


*Def*..  times : RR^3 times RR^3 to RR^3  mit  x times y = (x_2 y_3 - y_2 x_3) e_1 + (x_3 y_1 - y_3 x_1) e_2 + (x_2 y_1 - y_1 x_2) e_3  heißt **Vektorprodukt**  (\{e_1, e_2, e_3\}  Standardbasis. Merken mit: "det"  mat{e_1 & e_2 & e_3 \\ x_1 & x_2 & x_3 \\ y_1 & y_2 & y_3}).  

*Satz*.. (i)  (x + x') times y = x times y + x' times y  und  x times (y + y') = x times y + x times y'  (Distributivität).. (ii)  y times x = -x times y  ("Anti-Kommutativität").. (iii)  x times y = 0 <=> x, y  sind linear unabhängig.

**Zusammenhänge zw. Vektor- und Skalarprdukt**.. Für beliebige  x, y, z in RR^3  gilt:: (i)  (x times y) cdot z = det mat{x_1 & x_2 & x_3 \\ y_1 & y_2 & y_3 \\ z_1 & z_2 & z_3}.  Unmittelbare Folgerungen:  (x times y) cdot y = 0  und  (x times y) · x = 0..  (ii)  |x times y|^2 = |x|^2 · |y|^2 - (x · y)^2.  Folgerung:  |x times y| = |x| · |y| · |sin sa (x, y)|.  

*Folg*.. Der Betrag des Vektorprodukts zweier Vektoren entspricht dem Flächeninhalt des von ihnen aufgespannten Parallelogramms.

*Satz*..  (u times v) · w  ist das Volumen des Spats aufgespannt aus  u, v, w in RR^3.  

*Folg*..  RR^3.. det A_{E_3 E_3}^f = frac{V(f(e_1), f(e_2), f(e_3))}{V(e_2, e_2, e_3)},  wobei  V(x, y, z)  das Volumen des von  x, y, z in RR^3  aufgespannten Spats.

*Def*..  B = \{b_1, ..., b_n\}  Basis von VR  V.. A_{(B)}  mit Einträgen  a_{i j} = b_i cdot b_j  heißt **Gramsche Matrix**.

*Satz*..  A_{(E_n)} = (T_B^{E_n})^T cdot A_{(B)} cdot T_B^{E_n}.  

*Satz*..  x, y in V,, B  Basis..  x cdot y = ([x]_B)^T cdot A_{(B)} cdot [y]_B.  
