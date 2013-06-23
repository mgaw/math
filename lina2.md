Titel: Lina 2
Layout: cm toc
Format: html

# Montag 8. April (1)

Def.. Ein Schema der Form ... heißt **Matrix** reeller Zahlen mit  m  Zeilen und  n  Spalten, kurz:  m times n  -Matrix,  i  ist Zeilenindex,  j  Spaltenindex, Spaltenvektoren, Zeilenvektoren. Menge aller reellen  m times n  -Matrizen:  RR^{m times n}.  

Def.. Matrix **quadratisch**, falls  m = n.  

Def.. Quadratische Matrix. Sind alle  a_{i j}  mit  i != j  gleich Null, so heißt diese Matrix **Diagonalmatrix**:  mat{a_{1 1} & & 0 \\ & ddots & \\ 0 & & a_{n n}}  

Def.. Matrix **symmetrisch**, falls  A = A^T.  

Def.. **Zeilenrang**, **Spaltenrang**.

Folgerung.. Der Spaltenraum einer Matrix ist gleich der Dimension des von den Spaltenvektoren erzeugten linearen Unterraums  span(a_{s 1}, ..., a_{s n}).  

# Mittwoch 10. April (2)

Satz.. Vektoren sind linear unabhängig  <==>  Lineare Hülle hat "volle" Dimension  <==>  Linearkombinations-Vektorgleichung ist eindeutig lösbar  <==>  Linearkombinations-Vektorgleichung hat nur die triviale Lösung  <==>  Bei Gauß-Verfahrens-Matrix  mat{... & | & 0 \\ ... & | & 0}  verschwindet *keine* Zeile  <==>  Matrix hat vollen Rang  <==>  Kern der Abbildung ist  \{varnothing\} <==>  Abbildung ist invertierbar  <==>  Determinante ist nicht Null.

(Umformungen ändern den Z/S-Rang nicht.)

# Montag 15. April (3)

Satz.. Zeilenrang = Spaltenrang.

Def.. Eine quadratische  n times n  -Matrix heißt regulär, falls  rg A = n.  

wo? Satz..  (A B) v = A (B v).. lam (A B) = (lam A) B = A (lam B) = (A B) lam.  

wo? Satz..  (A B)^T = B^T A^T.  

# Mittwoch 17. April (4)

Bmk.. Kann nur multiplizieren, wenn Spalten links = Zeilen rechts. Also  A in RR^{l times m} cdot B in RR^{m times n}  geht.

Satz.. Matrizenmultiplikation ist *nicht* nullteilerfrei.

Satz.. Das Produkt regulärer Matrizen (voller Rang) ist wieder reguläre Matrix, also insbesondere nullteilerfrei.

# Montag 22. April (5)

?

# Mittwoch 24. April (6)

Def.. Elementarmatrix  S_i(lam) :=  "passende" Einheitsmatrix mit  a_{i i} = lam.  

Satz.. Multiplikation mit  S_i(lam)  von links entspricht Multiplikation der *i*-ten Zeile mit  lam.  Multiplikation mit  S_i(lam)  von rechts entspricht Multiplikation *i*-ter Spalte mit  lam.  

Def.. Elementarmatrix  Q_i^j :=  "passende" Einheitsmatrix mit  a_{i j} = 1.  

Satz.. Multiplikation mit  Q_i^j  von links entspricht Addition von *j*-ter Zeile zu *i*-ter Zeile. Multiplikation mit  Q_i^j  von rechts entspricht Addition von *i*-ter Spalte zu *j*-ter Spalte.

Def.. Elementarmatrix  Q_i^j(lam) :=  Einheitsmatrix mit  a_{i j} = lam.  

Def.. Elementarmatrix  P_i^j :=  Einheitsmatrix mit  a_{i j} = 1, \; a_{j i} = 1.  

Bmk.. Generell: Multiplikation mit Elementarmatrizen von links sind Zeilenumformungen, von rechts sind Spaltenumformungen.

Satz.. Alle Elementarmatrizen sind regulär.

Satz.. Jede reguläre Matrix lässt sich als Produkt von Elementarmatrizen darstellen.

Satz.. Alle vier Elementarmatrizen sind invertierbar und ihre Inversen sind Produkte von Elementarmatrizen.

# Montag 29. April (7)

Satz..  (RR^{n times m}, +, cdot)  ist Vektorraum.

Inverse Matrizen.

Satz.. Eindeutigkeit der Inversen.

Satz.. Matrix genau dann invertierbar, wenn sie regulär ist.

Satz.. Die Menge der regulären quadratischen Matrizen ist eine Gruppe.

Satz.. Elementarmatrizen sind invertierbar. Die Inverse ist selber wieder Elementarmatrix.

Satz.. Eine Matrix ist invertierbar genau dann, wenn sie sich als Produkt von Elementarmatrizen darstellen lässt.

**Dimensionssatz**..  V  und  W  VR,  f: V to W  lin. Abb. und  dim(V) < infty.  Dann gilt:  dim V = dim Im f + dim Ker f.  

Def.. VR  V  heißt **isomorph** zu VR  W,  falls es eine bijektive lineare Abbildung  f : V -> W  gibt.

Def.. Sei  V  endlich-dimensionaler VR. Dann heißt  V^* := \{T : V to RR : T text{ ist linear}\}  **Dualraum von _V_**.

Satz..  V^*  ist Unterraum von  \{f : V to RR\}  und  dim V^* = dim V.  

Def.. Der von den Zeilen einer Matrix aufgespannte VR heißt **Zeilenraum**. Analog **Spaltenraum**. Die Lösungsmenge des LGS  A x = 0  heißt **Nullraum**.

Satz.. Zeilenumformungen ändern nicht den Zeilenrang, aber möglicherweise den Spaltenrang.

# Montag 6. Mai (8)

Def..  f : V to W  linear, falls Additivität und Homogenität.

Bsp..  f : RR^2 to RR^2, \; mat{x \\ y} mapsto mat{a x + b y \\ c x + d y}  ist linear für alle  a, b, c, d in RR.. f  injektiv  <==> ... = ... => ... = ... <==>  [LGS] eindeutig lösbar  <==> mat{a & b \\ c & d}  ist regulär..  f  surjektiv  <==> forall ... exists ... <==>  [LGS] lösbar  <==> mat{a & b \\ c & d}  ist regulär (?).

Def.. Lineare Abbildung heißt **Monomorphismus**, falls injektiv. **Epimorphismus**, falls surjektiv. **Isomorphismus**, falls bijektiv. **Automorphismus**, falls bijektiv und  f : V to V.  

Satz.. VR  V, \; W  und  f : V to W  linear.. (i) Lineare Abbildungen respektieren Linearkombinationen:  f(sum_{i = 1}^k lam_i u_i) = sum_{i = 1}^k lam_i f(u_i)..  (ii) Sind  u_i, ..., u_k  linear abhängig, so sind auch  f(u_1), ..., f(u_k)  linear abhängig.. (iii)  U ≤ V \;=>\; f(U) ≤ W..  (iv)  f(span(u_1, ..., u_k)) = span(f(u_1), ..., f(u_k)).  

# Mittwoch 8. Mai (9)

**Hauptsatz über lin. Abb**.. Seien  V, W  VR,  B = \{b_1, ..., b_n\}  eine Basis von  V  sowie  w_1, ..., w_n  beliebige Vektoren von  W.  Dann existiert *genau eine* lineare Abbildung  f : V to W  mit  f(b_i) = w_i  für  i = 1, ..., n.  

# Montag 13. Mai (10)

Matrizielle Darstellung lin. Abb.

Def..  A^f_{B C} cdot [v]_B = [f(v)]_C.  

# Mittwoch 15. Mai (11)

Satz.. Nacheinandersausführung linearer Abbildungen ist wieder linear.

(Pfingsmontag)

# Mittwoch 22. Mai (12)

Satz.. Die Menge der Isomorphismen  f : V -> V  ist eine Gruppe bzgl. Nacheinanderausführung.. Die Menge der regulären  n times n  -Matrizen ist eine Gruppe bzgl. Maultiplikation.. Diese beiden Gruppen sind isomoprh (bzgl. einer festgelegten Basis von  V).  

Def..  V  Vektorraum,  B, B'  Basen von  V,, v in V.  **Transformationsmatrix** ist die Matrix  T_B^{B'},  so dass  T_B^{B'} cdot [v]_B = [v]_{B'}.  

**Berechnung von**  T_B^{B'}..  Es seien  B = (b_1, ..., b_n)  und  B' = (b_1', ..., b_n')  zwei Basen von VR  V..  Die Elemente von  B'  als Linearkombination bzgl.  B  schreiben:  b_j' = sum_{i = 1}^n t_{i j} b_i..  Das schreibe ich in die Spalten der Matrix:  T_B^{B'} := (t_{i j})_{1 ≤ i, j ≤ n}.  (In den Spalten von  T_B^{B'}  stehen die Basisvektoren von  B'  bzgl. der Basisvektoren von  B.)  

Satz..  T_B^{B'} = A_{B B}^f  mit  f : V to V,, f(b_i) = b_i',, i = 1..n.  

Satz..  T_B^{B'} = A_{B' B}^{Id}.  (?)

Bsp..  T_B^{B'} = mat{frac{1}{sqrt 2} \;& -frac{1}{sqrt 2} \\ frac{1}{sqrt 2} & frac{1}{sqrt 2}}  ist die Drehmatrix um 45 Grad.

**Basistransformationsformel**..  A^f_{B' B'} = T^B_{B'} cdot A^f_{B B} cdot T^{B'}_B.  (?)

Satz..  (t_B^{B'})^{-1} = T_{B'}^B.  


# Montag 27. Mai (13)

# Mittwoch 29. Mai (15)

Def.. Zwei Matrizen  A  und  B  heißen **ähnlich**, falls es eine Matrix  S  gibt, so dass  A = S^{-1} A S.  Schreiben  A sim B.  

Satz.. Die Ähnlichkeit von Matrizen ist Äquivalenzrelation.

Satz.. Zwei Matrizen sind genau dann ähnlich, wenn sie bzgl. bestimmter Basen dieselbe lin. Abb. beschreiben.

Bmk.. Alle Matrizen gleichen Ranges sind zueinander ähnlich.

Determinante (?) ist Spezialfall der Cramerschen Regel.

Satz.. Es gibt genau eine Abbildung mit D1, D2, D3.

Def.. Diese Abbildung (falls sie existiert), heißt **Determinante**(nfunktion).

Satz.. Ist  det  eine Determinantenfunktion, dann gilt: (i), (ii).

Satz.. Matrix  A  regulär gdw.  det A != 0.  

Satz..  A  Matrix.  det A = det A^T.  

# Montag 3. Juni (16)

# Mittwoch 5. Juni (17)

Def..   K  Körper,  V  *K*-Vektorraum,  f : V to V  lineare Abbildung.  lam in K  heißt **Eigenwert von _f_**, falls es  v in V, \; v != 0  gibt, so dass  f(v) = lam v..  Diese  v  heißen **Eigenwerte zu**  lam.  

%. \; \{v in V : f(v) = lam v \} = ker(f - lam Id)  heißt **Eigenraum zu**  lam.  

% (Identifizieren  f  mit Matrix zu einer Basis  B.  Ziel: Basis finden, so dass die Matrix der Abbildung diagonal ist.)

Lemma.. Sei  A  die Matrix von  f : V to V  bzgl. einer Basis  (v_1, ..., v_n)  von  V,  dann hat  A  Diagonalgestalt, d.h.  A = mat{lam_1 & & 0 \\ & ddots & \\ 0 & & lam_n},  wenn  v_i  Eigenvektor zum Eigenwert  lam_i  ist  (i = 1, ..., n).  

% Satz..  V  endlichdimensional,  A  eine zu  f  gehörige Matrix.  f(v) = lam v <=> A x = lam x <=> A x = lam E x <=> (A - lam E)x = 0.  

Lemma.. Ein Vektor  v in V \ \{0\}  ist genau dann Eigenvektor von  f : V to V  zum Eigenwert  lam in KK,  wenn  v in ker(f - lam Id).  

Def.. Ist  lam  ein Eigenwert von  f,  dann heißt der Untervektorraum  E_lam := ker(f - lam Id)  von  V  der **Eigenraum** von  f  zum Eigenwert  lam,  und  beta_lam := dim E_lam  heißt **geometrische Vielfachheit von**  lam.  

% Def..   det(A - lam E)  heißt das **charakteristische Polynom von _f_**.

% Satz.. Die Nullstellen des charakteristischen Polynoms sind die Eigenwerte von  f.  

% >  (A - lam E)x = 0  ist lösbar  (x != 0)  genau dann, wenn  det(A - lam E) = 0.  

% Def.. Die *n*-fachheit einer Nullstelle  lam  im charakteristischen Polynom heißt die **algebraische Vielfachheit** dieses Eigenwertes.

% Def.. Eine quadratische Matrix  A  heißt **diagonalisierbar**, falls es eine Diagonalmatrix gibt, die zu  A  ähnlich ist.

% Satz.. Eine *n*-dimensionale Matrix  A  ist genau dann diagonalisierbar, wenn es  n  linear unabhängige Eigenvektoren von  A  gibt (eine Basis aus Eigenvektoren).

Lemma.. Seien  v_1, ..., v_r  Eigenvektoren zu Eigenwerten  lam_1, ..., lam_r  von  f  und gelte  lam_i != lam_j  für  i != j,  dann ist  (v_1, ..., v_r)  linear unabhängig.

Folgerung..  f : V to V  Endomorphismus mit  dim V = n  über  KK,, lam_1, ..., lam_r  seien die EW und  n_1, ..., n_r  seien die geom. Vielfachheiten, d.h.  n_i = dim E_{lam_i}.  Sei jeweils  (v_1^{(i)}, ..., v_{n_i}^{(i)})  Basis von  E_{lam_i}..  Dann ist auch  (v_1^{(1)}..v_{n_1}^{(1)}, ..., v_1^{(r)}..v_{n_r}^{(r)})  linear unabhängig (d.h. Menge von EV zu versch. EW sind lin. unabh.).. Insbesondere ist  n_1 + ... + n_r ≤ n quad  und  quad f  diagonalisierbar  <=> n_1 + ... + n_r = n.  

Satz..  lam  ist EW zu  f  genau dann, wenn  det(f - lam Id) = 0.  

Def..  f  Endomorphismus.  A  Matrix von  f  zu beliebiger Basis. Dann  det f := det A.  (Determinante ist unabhängig von Basis.)

# Montag 10. Juni (18)

Def.. Wird  f  bzgl. einer Basis von  V  durch die Matrix  A  beschrieben, so ist  P_f(lam) = P_A(lam) = det(f - lam Id_V)  das **charakteristische Polynom** von  f.  

Satz.. Das charakteristische Polynom eines Endomorphismus  f  ist unabhängig von der Wahl der Basis, bzgl. der  f  durch eine Matrix  A  beschrieben wird.

Satz.. Es gibt Koeffizienten  a_0, ..., a_{n - 1},  so dass  P_f(lam) = (-1)^n lam^n + a_{n-1} lam^{n-1} + ... + a_1 lam + a_0..  Die Eigenwerte einer linearen Abbildung bzw. einer Matrix sind die Nullstellen des charakteristischen Polynoms.

# Mittwoch 12. Juni (19)

Def.. Sei  f in L(V, V)  und  lam_0  sei ein EW von  f,  d.h.  lam_0  ist Nullstelle des char. Polynoms  P_f(lam) = det(f - lam Id)..  Dann ist  (lam - lam_0)  ein Teiler von  P_f(lam).  Der maximale ganzzahlige Exponent  alpha_{lam_0}  mit  (lam - lam_0)^{alpha_{lam_0}} | P_f(lam)  heißt **algebraische Vielfachheit** des EW  lam_0.  

Satz.. Die geometrische Vielfachheit eines EW ist  ≤  der algebraischen Vielfachheit.

Def.. Ein Endomorphismus  f in L(V, V)  heißt **diagonalisierbar**, falls  V  eine Basis besitzt, die vollständig aus EV von  f  besteht.

Def.. Eine Matrix  A in RR^{n times n}  heißt **diagonalisierbar**, falls eine *invertierbare* Matrix  S in RR^{n times n}  existiert, so dass  S{^-1} A S  eine Diagonalmatrix ist.

Satz.. Eigenvektoren zu versch. EW sind lin. unabhängig.

Satz..  f in L(V, V)  ist diagonalisierbar gdw. für jeden EW die algebraische und geometrische Vielfachheit übereinstimmen. Insbesondere ist jeder Endomorphismus mit  n = dim V  paarweise verschiedenen EW diagonalisierbar.

Def.. Eine **positiv definite symmetrische Bilinearform** (verallgemeinertes Skalarprodukt) auf einem reellen VR ist eine Abbildung  B : V times V to RR  mit:: (B1)  B(u + v, w) = B(u, w) + B(v, w)  (Additivität) und  B(lam u, v) = lam B(u, v)  (Homogenität) (Linearität im ersten Argument).. (B2)  B(u, v) = B(v, u)  (Symmetrie).. (B3)  B(u, v) ≥ 0  sowie  B(u, u) = 0 <=> u = 0  (positiv definit).

Bmk.. Wegen der Symmetrie gilt auch die Linearität im zweiten Argument.

Def.. Ein VR  V  mit einer pos. def. symm. BLF  B  heißt **euklidischer VR**  (V, B).  Ein affiner Punktraum mit pos. def. symm. BLF heißt **euklidischer Punktraum**  (A, V, B).  

Satz.. Für die positiv definite BLF eines Vektors  x  mit einer Linearkombination aus Vektoren  x = sum_{i = 1}^k lam_i v_i  gilt  B(x, sum_{i = 1}^k lam_i v_i) = sum_{i = 1}^k lam_i B(x, v_i).  

Def.. Wir nennen positiv definite BLF in Zukunft **Skalarprodukte** und schreiben dafür  a cdot b  oder  langle a, b rangle.  

Satz..  V  sei euklidischer VR mit Skalarprodukt  `cdot´  und  B = \{b_1, ..., b_n\}  eine Basis von V. Wenn alle Skalarprodukte  b_i cdot b_j \;(i, j = 1..n)  der Basisvektoren gegeben sind, so ist das Skalarprodukt zweier beliebiger Vektoren von  V  eindeutig bestimmt.

Def.. Es sei  u in V  (eukl. VR mit SP). Dann heißt  |u| := sqrt{u cdot u}  der **Betrag** von  u.  Sind  P  und  Q  zwei Elemente eines affinen Raumes, so nennt man den Betrag des Vektors  ora{P Q}  ihren **Abstand**.

**Cauchy-Schwarz-Ungleichung**.. Für beliebige Vektoren  u, v  eines eukl. VR gilt, dass  |u cdot v| ≤ |u| cdot |v|.  Gleichheit gilt gdw.  u  und  v  lin. abhängig.

# Montag 17. Juni (20)

% Wir benutzen Transformationsmatrizen, um das Skalarprodukt zu berechnen.  =>  Gramsche Matrix eines SP bzgl.  B  bzw.  B'.  

% Dimensionssatz und Eigenraum.

**Dreiecksungleichung**.. Für beliebige Vektoren  u, v  eines eukl. VR gilt  |u + v| ≤ |u| + |v|.  

Def.. Zwei vom Nullvektor verschiedene Vektoren  u, v  eines euklidischen VR heißen **orthogonal** genau dann, wenn  u v = 0.  

% Bsp.. Beweis Satz des Pythagoras: ...

Def.. Es seien  u, v  zwei versch. Vektoren eines eukl. VR. Als **Winkelmaß** dieser Vektoren bezeichnet man die Zahl  phi  mit  cos phi = frac{u cdot v}{|u| cdot |v|}  (mit  -pi < phi < pi).  

% (Diese Definition wird durch die Cauchy-Schwarz-Ungleichung gerechtfertigt.)

% Bsp.. Beweis Kosinussatz: In jedem bel. Dreieck gilt  a^2 = b^2 + c^2 - 2 b c cos alpha.  

Def.. Es sei  (V, .)  ein eukl. VR. Eine Basis  B = \{b_1, ..., b_n\}  von  V  heißt **Orthonormalbasis**, falls:: (i) Alle Basisvektoren sind Einheitsvektoren, d.h.  |b_1| = ... = |b_n| = 1..  (ii) Alle Basisvektoren sind paarweise orthogonal zueinander, d.h.  b_i b_j = 0  für  i neq j, \; i, j = 1..n.  

Def.. Ein Koordinatensystem  K = \{0, b_1, ..., b_n\}  eines affinen Raumes heißt **karthesisches Koordinatensystem**, falls  \{b_1, ..., b_n\}  eine ON-Basis ist.

# Mittwoch 19. Juni (21)

**Gram-Schmidtsche Orthonormalisierungsverfahren** ...

Def.. Seien  V, W  eukl. VR. Eine lin. Abb.  f : V to W  heißt **orthogonale Abbildung**, falls für alle  u, v in V  gilt, dass  f(u) f(v) = u v.  

Satz.. Jede orthogonale Abbildung ist injektiv, eine orthogonale Abbildung  f : V to V  ist ein Isomorphismus.

Bezeichnungen..  O(V)  ist die Menge aller orthogonalen Abb.  V to V.. O(n)  ist die Menge aller orthogonalen Abb. in  RR^n  bzgl. des Standardskalarprodukts.. Als **orthogonale Matrizen** bezeichnen wir Matrizen orthogonaler Abb. bzgl. des Standardskalarprodukts.

Satz.. Jede betragstreue lin. Abb., d.h. jede lin. Abb. mit  f : V to W  mit  |f(u)| = |u|  f.a.  u in V,  ist eine orthogonale Abbildung.

Satz.. Sind  V, W  eukl. VR und  B = \{b_1, ..., b_n\}  eine ON-Basis von  V,  so ist eine lineare Abb.  f : V to W  genau dann orthogonal, falls  \{f(b_1), ..., f(b_n)\}  ein ON-System in  W  und damit eine ON-Basis von  Im f.  

Folgerung.. Eine  n times n  -Matrix ist genau orthogonal, wenn die *Spalten* ein ON-System bilden.

Folgerung.. (i) Ist  A  eine orthogonal Matrix, so gilt  A^T cdot A = E_n..  (ii)  A^{-1} = A^T..  (iii)  det A = +- 1.  

Def.. Orthogonale Abbildungen, die durch orthogonale Matrizen mit positiver Determinante (1) beschrieben werden, heißten **ordnungserhaltend**, solche mit  det A = -1  **ungleichsinnig**.
