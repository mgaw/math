Titel: Lineare Algebra I*
Layout: parskip toc cm

# Nov 8. Linksnebenklasse

Def.. Sei  (G, cdot)  eine Gruppe und  H ≤ G.  Die Teilmenge von  PP(G),  die aus Elementen der Form  g H  besteht wird als  (G/H)_l  bezeichnet. Sie heißt Menge der **Linksnebenklassen** von  H.  

Lemma..  forall x, y in G : x H=y H <=> x^{-1}y in H.  

Satz.. Die Relation  sim_l  mit  x sim_l y <=> x H = y H  ist eine Äquivalenzrelation. Die Linksnebenklassen von  H  sind also Äquivalenzklassen, das heißt  overline x = x H.  

Bmk..  G  wirkt auf  (G/H)_l  durch Multiplikation von links, das heißt für  g, x in G : g(x H) = (g x)H in (G/H)_l.  

Satz.. Multiplikation von links mit einem bestimmten Element  g in G  definiert einen Gruppenhomomorphismus  L_g : (G/H)_l to (G/H)_l  mit  L_g(x H) := (g x)H.  

# Nov 13. Normalteiler, Faktorgruppe

Bsp.. Sei  G  Gruppe,  H ≤ G.  Dann ist  (G/H)_l := \{g H : g in G\} sse P(G)  die Menge der
Linksnebenklassen von  H  in  G.  Haben Äquivalenzrelation auf *G*:
  x sim_l y :<=> x^{-1}y in H.  Dann ist  overline x = \{y in G : x sim_l y\} = \{y in G : x^{-1}y
= h in H\} = \{y in G : y = x h, h in H\} = x H.  

Def.. Eine Untergruppe  H  einer Gruppe  G  heißt **Normalteiler**, wenn  forall h in H, g in G:
g^{-1}h g in H.  Dann schreibt man  H unlhd G.  

Bmk.. Für abelsche Gruppen gilt, dass jede Untergruppe ein Normalteiler ist.

Satz.. Sei  H unlhd G,  dann kann man die Verknüpfung  (G/H)_l times (G/H)_l to (G/H)_l  mit  (x H,
y H) mapsto x y H  definieren.

Bmk.. Sei  H ≤ G.  Dann ist  H unlhd G <=> g H = H g, \; forall g in G.  Die Linksnebenklassen sind also
die Rechtsnebenklassen sind die Nebenklassen.

Satz.. Ist  H unlhd G,  dann ist  ((G/H), cdot)  eine Gruppe. Man nennt sie **Faktorgruppe**.

Def.. Sei  H ≤ G.  Dann heißt  [G:H] := |(G/H)_l|  der **Index** von  H  in  G.  

**Satz von Lagrange**.. Sei  G  endliche Gruppe,  H ≤ G.  Dann  |G| = |H| cdot [G:H].  

Kor.. Die Ordnung einer Untergruppe teilt die Ordnung der Gruppe:  |H|\;|\;|G|.  

# Nov 15. Kleiner Satz von Fermat

**Satz von Lagrange anders**..  G  endliche Gruppe,  H ≤ G.  Dann gibt es eine Bijektion  (G/H)_l times 
H to G.  

Bmk.. Die Anzahl der Links- und Rechtsnebenklassen ist gleich, d.h.  [G:H] = |(G/H)_l| = |(G/H)_r|.  

Kor.. Ist  G  endliche Gruppe,  n = |G|, x in G.  Dann  ord (x) \; | \; |G|,  d.h.  x^n = e, \; forall x in G.  

Bsp..  overline a in ZZ/n ZZ, \; 0 ≤ a ≤ n-1.  Dann  ord(overline x) = n <=> ggT(a,n) = 1.  

**Kleiner Satz von Fermat**.. Sei  p  Primzahl und  a in ZZ  mit  p not | \; a.  Dann gilt  a^{p-1}
equiv 1 mod p.  Außerdem gilt für alle  a in ZZ : a^p equiv a mod p.  

# Nov 20. Isomorphiesatz

Prop.. Seien  a, b in ZZ, \; d = \text{ggT}(a, b).  Dann gibt es  x, y \in ZZ,  so dass  d = x a + y b.  

Bmk.. Der  ggT(a, b)  ist die kleinste natürliche Zahl, die als lineare Kombination von a und b
darstellbar ist.

Lemma.. Sei  f:G \to G'  Gruppenmorphismus. Dann ist  N:=ker(f) unlhd G.  

Def..  sgn(sigma) = (-1)^{\#\{(i,j) \;:\; i<j \text{ und } sigma(i) > sigma(j)\}}.  

Lemma..  \forall sigma \in S_n : sgn(sigma) = (Produkt) \frac{sigma(j) - sigma(i)}{j-i}.  

Def..  sigma in S_n  heißt **gerade**, falls  sgn(sigma) = 1. \; sigma  heißt **ungerade**, falls  sgn(sigma) = -1.  

Def..  ker(sgn) = A_n = \{ sigma in S_n : sgn(sigma) = 1 \}  heißt die **alternierende Gruppe**.

Bmk..  A_n unlhd S_n.    |A_n| = \frac{n!}{2}.  

**Isomorphiesatz**.. Sei  phi : G to G'  Gruppenmorphismus, damit  ker(phi) unlhd G.  Dann gibt es einen kanonischen Isomorphismus von Gruppen  overline φ : G/ker(φ) simto φ(G).  
  (φ(G) ≤ G'  Untergruppe.)  phi = overline phi circ pi. \; pi  ist die Projektion, die ein Element aus  G  auf seine Nebenklasse abbildet. Eigentlich nur:  overline φ : G/ker(φ) to G'  ist injektiv. Aber wenn  phi(G)=G'  dann surjektiv und damit auch bijektiv.

Bmk.. Falls  φ  surjektiv ist, d.h.  φ(G) = G',  dann bildet  overline φ  nach  G'  ab.

# Nov 20 (Übung)

Satz..  G  Gruppe,  overline x cdot overline y := overline {x cdot y}. quad (G/H, cdot)  ist Gruppe,
gdw.  H unlhd G.  

Prop..  G  Gruppe,  overline x cdot overline y := overline {x cdot y}, H unlhd G. quad π : (G, cdot)
 to (G/H, cdot), \; x mapsto overline x  ist Gruppenhomomorphismus.

# Nov 22. Ring, Körper

Def.. Eine Menge  R  zusammen mit zwei Verknüpfungen  +: R times R to R  und  cdot : R times R to R  
heißt **Ring**, wenn (i)  (R, +)  ist abelsche Gruppe mit neutralem Element  0 in RR,  (ii) "
  cdot  " ist assoziativ und (iii) es gilt Distributivität.

Def.. Ein Ring heißt **kommutativ**, wenn  a cdot b = b cdot a, \; forall a, b in R.  

Def..  0 in R  heißt das **Nullelement**.

Def.. Ein Element  1 in R  heißt **Einselement**, wenn  1 cdot a = a cdot 1 = a, \; forall a in R.  
Ein Ring mit Einselement heißt **Ring mit Eins**.

Prop.. Sei  R  ein Ring,  0 in R  das Nullelement. Dann gilt (i)
  0 cdot a = a cdot 0 = 0, \; forall a in R  und (ii) falls  R  Ring mit Eins ist, dann
  (-1) cdot a = -a,  wobei  -a in R : a + (-a) = 0.  

Def..  (R, +, cdot), (R', oplus, odot)  Ringe. Eine Abbildung  phi : R to R'  heißt **Morphismus von
Ringen**, wenn  forall a, b in R  (i)  phi(a+b) = phi(a) oplus phi(b)  und (ii)
  phi(a cdot b) = phi(a) odot phi(b).  

Satz.. (i) gdw.  phi : (R, +) to (R', oplus)  ist Morphismus von abelschen Gruppen.
(ii) gdw.  phi : (R, cdot) to (R', odot)  ist Monoidmorphismus.

Def..  phi  ist **Isomorphismus**, wenn  phi  ist bijektiver Morphismus.

Def.. Ein Ring mit Eins  (K, +, cdot)  heißt **Körper**, gdw.  (K^* = K setminus \{0\}, cdot)  ist abelsche Gruppe.

# Nov 27. Komplexe Zahlen

Satz..  (CC := RR^2, +, cdot)  bildet einen Körper.

Bmk.. Wir können  RR  als Untermenge von  CC  betrachten wie folgt.  phi : RR to CC  mit  phi(a) := (a, 0).  Dann ist  phi  ein Ringhomomorphismus.

Satz.. Seien  x, y in CC.  Dann folgt: (1)  overline{x+y} = overline x + overline y,  (ii)  overline{x cdot y} = overline x cdot overline y  und (iii)  x in RR <=> x = overline x.  Aus (i) und (ii) folgt, dass  x mapsto overline x  Ringhomomorphismus ist.

# Nov 29. Polynomkörper

Def..  x in CC.  Dann  |x|:=sqrt{x cdot overline x}.  

Satz..  x, y in CC. \;|x + y| ≤ |x| + |y|. \;|x cdot y| = |x| cdot |y|. \; x = |x| cdot cos phi + i|x| sin phi = |x|(cos phi + i sin phi) = |x|e^{i phi} = |x|e^{i cdot \arg(x)}.  Bisher gilt  e^{i phi} := cos phi + i sin phi.  

Def.. Sei  R  ein Ring. Ein Element  x in R^*  heißt **Nullteiler**, falls es ein  y in R*  gibt, so dass  x cdot y = 0_R  ist. Ein Ring ohne Nullteiler heißt **nullteilerfrei**.

Satz.. Jeder Körper ist nullteilerfrei.

Def.. Ein kommutativer, nullteilerfreier Ring mit 1 heißt **Integritätsbereich**.

Bmk.. Jeder Körper ist Integritätsbereich.

Lemma.. Ein Integritätsbereich mit endlich vielen Elementen ist ein Körper.

Bmk.. Sei  k  Primzahl. Dann ist  ZZ/p ZZ  Körper und wird mit  FF_2  bezeichnet.

Def.. Sei  R  ein Ring mit 1. Dann heißt  char(R) := 0  falls  n cdot 1_R neq 0_R  für alle  n in NN_{>0}  und  char(R) := min \{n in NN_{>0} : n cdot 1_R = 0_R\}  die **Charakteristik** von  R.  

Satz.. Sei  K  Körper. Dann ist  char(K)  entweder 0 oder eine Primzahl.

Bmk.. Ist  K  ein endlicher Körper, so ist  char(K) = p > 0  und es ist  |K|=p^n, \; n in NN_{>0}  und es gibt einen injektiven Ringhomomorphismus  FF_k to K.  

Def.. Der Körper  FF_p  heißt **Primkörper** der Charakteristik  p.  

Def.. Sei  K  Körper. Ein **Polynom** mit Koeffizienten in  K  in der Unbestimmten  t  ist ein Ausdruck der Form  f = f(t) = a_0 + a_1 t + a_2 t^2 + ... + a_n t^n  mit  a_0, ..., a_n in K, \; n in NN. \; K[t]  ist die Menge aller solchen Polynome.  f=0  heißt **Nullpolynom**.  deg(f) := max \{n in NN : a_n neq 0\}  heißt **Grad** von  f.  Das Polynom heißt **normiert**, falls  a_n = 1,  wobei  n = deg f.  

Bmk.. Man kann für  t  ein  x in K  einsetzen, dann ist  f(x) in K.  Ein Polynom induziert also eine Abbildung  tilde f : K to K, \; x mapsto f(x).  

Bmk..  f mapsto tilde f  ist nicht injektiv, da  tilde f  Nullabbildung sein kann, obwohl  f  nicht Nullpolynom ist.

Satz..  (K[t])  ist mit den folgenden Operationen  +  und  cdot  ein Ring. Sei  f(t) = sum^m_{i=0} a_i t^i, \; g(t) = sum^n_{i=0}.  Dann  (f+g)(t) := sum^{max (m, n)}_{i=0} c_k t^k, \; c_k = a_k+b_k  und  (f cdot g)(t) := sum^{m+n}_{i=0}d_k t^k, \; d_k = sum_{i+j=k}a_i b_j.  

Bmk.. Für den Grad der Polynome gilt  deg(f+g) ≤ max (deg f, deg g)  und  deg(f cdot g) = deg f + deg g,  wobei  -infty + n := -infty  und  max (-infty, n) := n.  

Satz.. Seien  f, g in K[t]  mit  g neq 0.  Dann existieren eindeutig bestimmte  q, r in K[t],  so dass  f = q g + r  ist und  deg(r) < deg(g).  

# Dez 4. Polynomteiler, Vielfachheit von Nullstellen

**Division mit Rest**.. Sei  K  Körper,  f,g in K[t]  Polynome. Dann existieren  q(t), r(t)  eindeutig bestimmt in  f=g q + r  mit  deg(r) < deg(g).  

Def.. Sei  f in K[t]. \; lam in K  heißt **Nullstelle**, falls  f(lam) = 0.  

Kor..  lam in K  Nullstelle von  f <=> (t-lam) | f :<=> exists q in K[t]  mit  f=(t-lam)q.  

Satz.. Sei  K  Körper,  f in K[t], \; f neq 0, \; deg(f) = n.  Dann besitzt  f  höchstens  n  Nullstellen.

Def..  f in K[t], \; f neq 0, \; lam in K  Nullstelle. Die **Vielfachheit** von  lam,  ausgedrückt durch  mu(f, lam),  ist die größte natürliche Zahl  r  mit  (t-lam)^r | f.  

Bmk..  mu(f, lam) ≥ 1  heißt, dass  lam  Nullstelle ist.

Kor..  f in K[t]  Polynom,  lam_1, ..., lam_s  die verschiedenen Nullstelllen von  f,  das heißt  r_i = mu(f, lam) ≥ 1.  Dann gibt es ein  g in K[t]  mit  f=(t-lam_1)^{r_1} cdot (t-lam_2)^{r_2} cdot ... cdot (t-lam_s)^{r_s} cdot g.  Anders ausgedrückt: Produkt von i=1 bis s  (t-lam_i)^{r_i} | f.  

Satz..  sin(alpha+beta) = sin alpha cos beta + sin beta cos alpha.  

Satz.. Sei  w = r e^{i theta} in CC.  Dann besitzt das Polynom  z^n-w in CC[z] \; n  verschiedene Nullstellen, das heißt es existieren  n  verschiedene komplexe Zahlen  z_1, ..., z_n  mit  z_i^n = w.  Schreiben  sqrt[n] w := \{z_1, z_2, ..., z_n\}.  

# Dez 4. Ideal (Übung)

Satz.. Ein Homomorphismus  phi  zwischen Ringen mit trivialem Kern  ker(phi) = varnothing  ist injektiv.

Def.. Sei  (X, +, cdot)  ein Ring. Eine Menge  I sse X  heißt **rechtes (linkes) Ideal**, falls (i)  (I, +)  ist Untergruppe und (ii)  X cdot I sse I \; (I cdot X sse I).  

# Dez 6. Fundamentalsatz der Algebra, Vektorraum

Satz..  z = r e^{i theta} in CC. \; z^n = w <=> z = sqrt[n] w = \{sqrt[n]r (cos frac{theta + 2k pi} n + i sin frac{theta + 2k pi} n) : k in \{0, 1, ..., n-1\} \}.  

Folgerung.. Für  n=2  gilt  sqrt w = \{sqrt r (cos frac theta 2 + i sin frac theta 2), \; -sqrt r (cos frac theta 2 + i sin frac theta 2)\}  (wegen  cos (x + pi) = -cos x).  

Satz.. Sei  a z^2 + b z + c=0, \; a neq 0.  Dann  z=-frac{b +- sqrt{b^2 - 4a c}}{2a}.  

Prop.. Ist  f in RR[t]  ein *reelles* Polynom und  lam in CC  eine Nullstelle von  f.  Dann ist  overline lam in CC  eine Nullstelle von  f.  Es gilt sogar  mu(f, lam) = mu(f, overline lam).  

**Fundamentalsatz der Algebra**.. Jedes Polynom  f in CC[t]  mit  deg(f) > 0  hat mindestens eine Nullstelle.

Kor.. Jedes Polynom  f in CC[t]  zerfällt in Linearfaktoren, das heißt es gibt  lam_1, ..., lam_n in CC  mit  f(t) = a(t-lam_1)(t-lam_2)...(t-lam_n).  

Prop.. Sei  K  unendlicher Körper. Dann ist die Abbildung  K[t] to Abb(K, K)  injektiv.

Def.. Sei  K  ein Körper. Eine Menge  V  mit einer inneren Verknüpfung  +:V times V to V  und einer äußeren Verknüpfung  cdot : K times V to V  heißt **K-Vektorraum**, wenn gilt: (1)  (V, +)  ist abelsche Gruppe mit neutralem Element  0 in V.  (2) Verträglichkeiten für  lam, mu in K, \; v, w in V,  nämlich (i)  (lam + mu)v = lam v + mu v,  (ii)  lam(v+w) = lam v + lam w,  (iii)  lam(mu v) = (lam mu) v  und (iv)  1v = v.  

# Dez 11. Untervektorraum, lineare Unabhängigkeit

**Rechenregeln**.. a)  0_K cdot v = 0 in V.  b)  lam cdot 0 = 0.  c)  lam cdot v = 0 \;=>\; lam = 0  oder  v = 0.  d)  (-1) cdot v = -v,  das additiv Inverse zu  v.  

Def.. Sei  V  ein K-Vektorraum. Eine Teilmenge  W sse V  heißt **Untervektorraum** (man
schreibt  W ≤ V),  falls gilt: (UV1)  W neq varnothing.  (UV2)  v, w in W \;=>\; v+w in W.  (UV3)  v in W, lam in K \;=>\; lam cdot v in W.  (Nichtleer und abgeschlossen gegenüber  +  und  cdot.)  

Bmk.. Wegen (UV2) und (UV3) erhalten wir induzierte Operationen  +_W : W times W to W  und  cdot_W : K times W to W.  

Satz.. Sei  W  ein UVR. Dann ist  (W, +_W, cdot_W)  ein Vektorraum.

Lemma.. Sei  V  ein VR und  (W_i)_{i in I}  eine Familie von UVR von V. Dann ist auch  W := bigcap_{i in I} W_i  ein UVR.

Lemma.. Sei  V  ein K-Vektorraum und  W_1, W_2 ≤ V.  Dann gilt:  W_1 cup W_2 ≤ V \;<=>\; W_1 sse W_2  oder  W_2 sse W_1.  

Def.. Sei  v_1, ..., v_r in V:  Ein beliebiger Vektor  v in V  heißt **Linearkombination** von  v_1, ... v_r,  falls es  lam_1, ..., lam_r in K  gibt, so dass  v = lam_1 v_1 + ... + lam_r v_r.  

Def.. Sei  M sse V  eine Teilmenge. Die Menge aller Linearkombinationen von *endlich vielen* Vektoren aus  M  heißt **Lineare Hülle** (oder **Spann**) von  M.  Man schreibt  langle M rangle  oder  span_K(M).  

Satz.. Sei  V  ein Vektorraum und  M sse V  eine Teilmenge. Dann ist  langle M rangle  der kleinste UVR von  V,  der  M  enthält, das heißt (a)  langle M rangle  ist ein UVR und (b) Ist  W ≤ V  ein UVR mit  M sse W,  so gilt  langle M rangle sse W.  

Def.. Sei  V  ein Vekorraum. Eine endliche Familie  (v_1, ..., v_k)  von Vektoren in  V  heißt **linear unabhängig**, wenn für alle  lam_1, ..., lam_r in K  gilt:  (lam_1v_1 + ... + lam_r v_r = 0) \;=>\; (lam_1 = ... = lam_r = 0),  das heißt der Nullvektor lässt sich nur auf *eine* (triviale) Art als Linearkombination der  v_i  schreiben. Eine unendliche Familie  (v_i)_{i in I}  heißt linear unabhängig, wenn jede endliche Teilfamilie linear unabhängig ist. Eine Familie, die nicht linear unabhängig ist, heißt **linear abhängig**.

Lemma.. (a)  \{v\}  ist genau dann linear unabhängig, wenn  v = 0.  (b) Jede Familie, die den Nullvektor enthält, ist linear abhängig. (c) Eine Familie, die einen Vektor doppelt enthält, ist linear abhängig. (d) Zwei oder mehr Vektoren  v_1, ..., v_r  sind genau dann linear abhängig, wenn einer davon im Spann der anderen liegt.

# Dez 11. Maximales Ideal, Primideal (Übung)

Prop.. Seien  p, q in NN^*.  Dann  p ZZ + q ZZ = ggT(p,q)ZZ.  

Theorem.. Seien  p, q in NN^*  und  d = ggT(p,q).  Dann existieren  s, t in ZZ  so, dass  s p + t q = d.  

Def.. Zwei Ideale  A, B  eines Ringes  R  heißen **fremd**, falls  A+B=R.  

Kor..  p ZZ  und  q ZZ  sind genau dann fremde Ideale, wenn  ggT(p, q) = 1.  

Def.. Sei  (X, +, cdot)  ein kommutativer Ring. Ein Ideal  I sse X  heißt **Primideal**, falls  x y in I => x in I  oder  y in I. \; I  heißt **maximal**, falls  J  Ideal von  X  und  I sse J sse X \;=>\; J = I  oder  J = X.  

Satz..  p ZZ  ist genau dann Primideal von  ZZ,  wenn  p  Primzahl ist.

Satz.. Sei  I sse ZZ, x in X setminus I.  Dann gilt  J := displaystyle bigcap_{tilde J \text{ Ideal, } I cup \{x\} sse tilde J} = \{i+k x : i in I, k in ZZ\} =: H.  

Satz.. Sei  I  ein maximales Ideal von  ZZ.  Dann ist  I  Primideal.

# Dez 18. Basis

Def.. Sei  V  ein *K*-Vektorraum. Eine Familie  B = (e_i)_{i in I} sse V  heißt **Basis**, falls gilt: (1)  B  ist linear unabhängig und (2)  B  ist ein Erzeugendensystem von  V,  das heißt  span(B) = V.  

Satz.. Für eine Teilmenge  B=(e_i)_{i in I} sse V  sind die folgenden Bedingungen äquivalent: (1)  B  ist Basis. (2)  B  ist ein *minimales* Erzeugendensystem von  V,  das heißt:  A sse B  ist Erz.sys.  => A=B.  (3)  B  ist eine *maximale* linear unabhängige Teilmenge von  V,  das heißt:  B ssne B' sse V => B'  ist linear unabhängig.

**Austauschlemma**.. Sei  V  *K*-Vektorraum,  B = \{e_1, ..., e_r\}  Basis von  V  und  v=lam_1e_1 + ... + lam_r e_r in V.  Ist  lam_k neq 0 \;(1 ≤ k ≤ r),  dann ist  B':=\{e_1, ..., e_{k-1}, v, e_{k+1}, ..., e_r\}  wieder Basis von  V.  

# Dez 20. Dimension

**Austauschsatz**.. Sei  V  *K*-Vektorraum,  B = \{e_1, ... e_r\}  Basis und  \{v_1, ..., v_n\}  eine linear unabhängige Familie. Dann gilt: (1)  n <= r.  (2) Es gibt Indizes  i_{n+1}, ..., i_r in \{1, ..., r\},  so dass  \{v_1, ..., v_n, e_{i_{n+1}}, ..., e_{i_r}\}  auch eine Basis von  V  ist. (Bew. mit Induktion nach  n  und Austauschlemma.)

Kor.. Hat ein *K*-Vektorraum  V  eine endliche Basis, so ist jede Basis von  V  endlich.

Kor.. Zwei endliche Basen eines *K*-Vektorraumes haben die gleiche Länge.

Def.. Sei  V  *K*-Vektorraum. Dann  dim_K V := infty,  falls  V  keine endliche Basis besitzt.  dim_K V := r,  falls  V  eine Basis der Länge  r  besitzt.

Satz.. Ist  V  endlich erzeugt, dann gibt es eine endliche Basis von  V.  

Prop.. Ist  V  nicht endlich erzeugt, so gibt es eine unendliche linear unabhängige Familie von Vektoren.

# Jan 8. Dimensionssatz

Def..  V  Vektorraum,  W_i <= V.  Dann  W_1 + W_2 + ... + W_n := \{w_1 + w_2 + ... + w_n : w_i in W_i\}.  

Prop..  W_1 + W_2 + ... + W_n = span(W_1 cup W_2 cup ... cup W_n).  

Prop..  dim(W_1 + ... + W_n) <= dim(W_1) + ... + dim(W_n).  

**Dimensionssatz**.. Sind  U_1  und  U_2  Untervektorräume eines endlichdimensionalen *K*-Vektorraums  V,  so gilt:  dim_K(U_1 + U_2) + dim_K(U_1 cap U_2) = dim_K(U_1) + dim_K(U_2)..  

Satz.. Seien  U_1, U_2 <= V  Teilräume,  U := U_1 + U_2.  Dann sind die folgenden äquivalent.. (1) Ist  u_1 + u_2 = 0, \; u_1 in U_1, \; u_2 in U_2,  dann  u_1 = u_2 = 0..  (2) Für alle  u in U  ist die Darstellung  u = u_1 + u_2, \; u in U  eideutig.. (3)  U_1 cap U_2 = \{0\}..  In diesem Fall heißt die Summe  U_1 + U_2  **direkte Summe**. Man schreibt  U_1 oplus U_2.  

Def.. Seien  V, W  zwei *K*-Vektorräume.  f:V to W  heißt **linear**, falls folgendes gilt.. (1)  f(v+v') = f(v) + f(v'), \; v, v' in V..  (2)  f(lam v) = lam f(v), \; lam in K, \; v in V..  Ist  V=W,  dann ist  f:V to W  **Endomorphismus**.

Prop.. Sei  f:V to W  *K*-lineare Abbildung.. (1)  f(lam_1 v_1 + ... + lam_n v_n) = lam_1 f(v_1) + ... + lam_n f(v_n) \; forall v_1, ..., v_n in V, \; lam_1, ..., lam_n in K..  (2) Ist die Familie  \{v_i\}_{i in I}  in  V  linear abhängig, so ist  \{f(v_i)\}_{i in I}  linear abhängig in  W..  (3)  f(V) <= W..  (4)  dim f(V) <= dim W.  

Def..  Hom_K(V, W) := \{f:V to W : f \text{ ist }K\text{-lineare Abbildung}\}.  

Satz..  Hom_K(V,W) <= Abb(V, W).  

Def..  f in Hom_K(V,W). \; ker(f) := f^{-1}(0).  

Satz..  f  injektiv  <=> ker(f) = \{0\}.  

Def..  m,n in NN, \; K  Körper.  A=(...)  ist  m times n\text{-Matrix}  mit Einträgen aus  K.  Matrix ist eine Abbildung  A:\{1..m\} times \{1..n\} to K.  

# Jan 10. Koordinaten eines Vektors, Matrix einer Abbildung

Def..  M(m,n:K) := \{A = (a_{ij})_{smatrix{ 1 ≤ i ≤ m \\ 1 ≤ j ≤ n}} : a_{ij} in K\}.  Das sind Matrizen mit **_m_ Zeilen** und **_n_ Spalten**.  a_{ij}  ist der Eintrag der **_i_-ten Zeile** und der **_j_-ten Spalte**. Zuerst Zeile, dann Spalte. Das macht Sinn, wenn man Vektoren mit Einträgen  v_i in K  als Spaltenvektoren, also einspaltige Matrizen betrachtet. Dann wird das  j,  also die Spaltenangabe weggelassen, da diese immer gleich 1 ist.

Def..  M(n:K) := M(n,n:K).  

Def..  I_n := mat{1&&0 \\& ddots& \\ 0&&1 } = (∂_{ij})_{smatrix{ 1 ≤ i ≤ n \\ 1 ≤ j ≤ n}}, \; ∂_{ij} := 1,  für  i=j, \; ∂_{ij} := 0,  sonst.  I_n  ist die **_n_-reihige Einheitsmatrix**.

Bmk..  M(m,n:K)  ist ein *K*-Vektorraum isomorph zu  K^{mn}.  

Def.. Sei  A in M(m,n:K), \; A = (a_{ij})_{smatrix{ 1 ≤ i ≤ m \\ 1 ≤ j ≤ n}}.  Die **transponierte Matrix** ist  ^t A = (a_{ji})_{smatrix{ 1 ≤ j ≤ n \\ 1 ≤ i ≤ m }} in M(n,m:K).  

Bmk..  ^t I_n = I_n.  

Def.. Eine Matrix  A in M(m,n:K)  heißt **symmetrisch**, falls  A =    ^t A.  

Def.. Sei  V  ein *K*-Vektorraum und  B=(v_1,...,v_n)  eine Basis. Sei der Isomorphismus von Vektorräumen  Phi_B : K^n simto V  gegeben durch  Phi_B(λ_1, ..., λ_n) := λ_1v_1 + ... + λ_n v_n.  Sei  v=sum_{i=1}^n λ_i v_i..  Dann heißen  [v]_B :=    ^t(Phi_B^{-1}(v)) = mat{λ_1 \\ vdots \\ λ_n}  die **Koordinaten von _v_ bzgl. _B_**.

Def.. Sei  A = mat{a_{11} & cdots & a_{1n} \\ vdots & & vdots \\ a_{m1} & cdots & a_{mn}}  und  v=mat{v_1 \\ vdots \\ v_n} in K^n.  Definieren den Operator  cdot : M(m,n:K) times K^n to K^m  mit  A cdot v = mat{a_{11} & cdots & a_{1n} \\ vdots & & vdots \\ a_{m1} & cdots & a_{mn}} mat{v_1 \\ vdots \\ v_n} := mat{a_{11}v_1 + a_{12}v_2 + ... + a_{1n}v_n \\ vdots \\ a_{m1}v_1 + a_{m2}v_2 + ... + a_{mn}v_n}.  

Satz..  A (v+w) = A v + A w.. (A+B) = A v + B v.  

Def.. Sei  A in M(m,n:K).  Definieren  phi_A : K^n to K^m  mit  phi_A(v) := A v.  

Satz..  phi_A  ist eine *K*-lineare Abbildung. Die Spalten der Matrix stellen dabei die Bilder der Elemente  (0,...,1,...,0)  der kanonischen Basis von  K^n  dar.

Def.. Sei  f:V to W  eine *K*-lineare Abbildung,  B=(v_1, ..., v_n)  Basis von  V  und  C=(w_1,...,w_m)  Basis von  W.  Einträge  a_{ij}  seien gegeben durch  f(v_j) = a_{1j}w_1 + ... + a_{mj}w_m, 1 ≤ j ≤ n.  Definieren  M_B^C(f) := (a_{ij})_{smatrix{ 1 ≤ i ≤ m \\ 1 ≤ j ≤ n}}.  

Satz..  V, W, B, C, f  wie oben. Dann gilt für alle  v in V: [f(v)]_C = M_B^C(f) cdot [v]_B.  

Satz.. (...?) Dann  Phi_B = M = Phi_{B'}  

# Jan 15. Matrixmultiplikation, Faktorraum

Def..  A = (a_{ij})_{smatrix{ 1 ≤ i ≤ m \\ 1 ≤ j ≤ n}}, \; B = (b_{jl})_{smatrix{ 1 ≤ j ≤ n \\ 1 ≤ l ≤ r}}.. A B := (c_{il})_{smatrix{ 1 ≤ i ≤ m \\ 1 ≤ l ≤ r}}  mit  c_{il}:= sum_{j=1}^n a_{ij}b_{jl}  ("*i*-te Zeile von *A* mal *j*-te Spalte von *B*").

Satz..  phi_A circ phi_B = phi_{A B}  

**Rechenregeln**.. (1)  A(B+B') = A B+A B', \; (A+A')B = A B + A'B..  (2)  I_n A = A, \; A I_n = A..  (3)  ^t(A B) =    ^t B cdot    ^t A.  

Satz.. Sei  \{u_1, ..., u_r\}  eine Basis von  Ker(f).  Wählt man  v_1, ..., v_s in V,  so dass  \{f(v_1), ..., f(v_s)\}  eine Basis von  Bild(f)  bilden, dann ist  B=\{u_1, ..., u_r, v_1, ..., v_s\}  eine Basis von  V.  

Satz..  f:V to W, \; dim_K V, dim_K W < ∞..  Dann  dim_K V = dim_K Ker(f) + dim_K Bild(f).  

Def..  rang(f) := dim_K Bild(f).  

Kor.. Seien  V  und  W  endlich-dimensionale *K*-Vektorräume mit  dim_K(V)=dim_K(W).  Dann für eine lineare Abbildung  f:V to W  die Folgenden äquivalent.. (1)  f  injektiv.. (2)  f  surjektiv.. (3)  f  bijektiv.

Def.. Sei  V  ein *K*-Vektorraum,  U ≤ V  Unterraum. **Faktorraum**  V/U := \{x+U : x in V\}.  

Bmk..  x+U = y+U <=> x-y in U.  

Satz..  V/U  ist *K*-Vektorraum.

# Jan 17. Isomorphiesatz

**Isomorphiesatz**.. Sei  f:V to W  eine *K*-lineare Abbildung von *K*-Vektorräumen. Dann gibt es einen kanonischen Isomorphismus von *K*-Vektorräumen  tilde f:V/{Ker(f)} simto f(V) ≤ W  mit  tilde f(x+Ker(f)) := f(x), \; x in V.  

(Bmk..  dim_K V/U = dim_K V - dim_K U.)  

Def.. Eine Matrix  A in M(n,n:K)  heißt **invertierbar**, wenn es eine Matrix  B in M(n,n:K)  gibt mit  A B = B A = I_n.  

Lemma.. Sei  A=(a_{ij})_{1 ≤ i,j ≤ n} in M(n,n:K).  Ist  A  invertierbar, dann ist die lineare Abbildung  Phi_A:K^n to K^n  mit  Phi_A(x) = A x  ein Isomorphismus.

Prop.. Seien  A, B in M(n:K)  mit  B A = I_n,  dann ist  A B = I_n  und  B  mit dieser Eigenschaft eindeutig.

Bsp..  A = mat{a&b\\c&d} in M(2:K).  Sei  a d - b c = 0.  Dann  A^{-1} = frac{1}{a d-b c}mat{d&-b\\-c&a}.  



Satz.. Seien  V,W,U  Vektorräume,  f:V to W  und  g:W to U  lineare Abbildungen,  B,C,D  Basen von  V,W  bzw.  U.  Dann  M_C^D(g) cdot M_B^C(f) = M_B^D(g circ f).  

# Jan 22. Basiswechselmatrix

Def.. Sei  V  *K*-Vektorraum,  B  und  B'  Basen von  V.  Dann heißt  M_{B'}^B(Id_V)  die **Basiswechselmatrix von _B_ nach _B'_**.

Prop.. Die Matrix  T=M_{B'}^B(Id) in M(n:K)  ist invertierbar und es ist  T^{-1} = M_B^{B'}(Id).  

Satz.. Sei  f:V to W  eine lineare Abbildung,  B, B'  Basen von  V  und  C, C'  Basen von  W.  Seien  T=M_{B'}^B(Id_V)  Basiswechselmatrix von  B  nach  B'  und  S=M_{C'}^C(Id_W)  Basiswechselmatrix von  C  nach  C'.  Dann gilt:  M_{B'}^{C'}(f) = S^{-1}M_B^C(f)T.  

Def.. Sei  A = mat{a_{11} & ... & a_{1n} \\ vdots & & vdots \\ a_{m1} & ... & a_{mn}} in M(m,n:K).  Seien  v_j:=mat{a_{1j} \\ vdots \\ a_{mj}}, \; a ≤ j ≤ n  die Spaltenvektoren dieser Matrix. Definieren  Rang(A) := dim_K langle v_1, ..., v_n rangle.  

Satz.. Sei  f: V to W  lineare Abbildung,  B  Basis von  V  und  C  Basis von  W.  Dann  Rang(M_B^C(f)) = dim_K Bild(f).  

Kor.. Sei  A in M(n:K).  Dann ist  A  invertierbar genau dann, wenn  Rang(A) = n.  

Prop..  A in M(m,n:K), \; B in M(n,r:K).  Dann  Rang(A B) ≤ min (Rang(A), Rang(B)).  

# Jan 24. Lineare Gleichungssysteme

Def..  A in M(m,n:K), \; b = mat{b_1 \\ vdots \\ b_m} in K^m, \; x = mat{x_1 \\ vdots \\ x_n} in K^n.. Lös(A,b) := \{x in K^n : A x=b \} = Phi_A^{-1}(b)  ist die Lösungsmenge des Systems aus den Gleichungen  a_{i1}x_1 + ... + a_{in}x_n = b_i, \; 1 ≤ i ≤ m.  

Prop.. Gegeben ein lineares System  A x=b.  Sei  r=Rang(A)..  (1)  Lös(A,0) ≤ K^n  ist Unterraum mit Dimension  n-r..  (2)  Lös(A, b)  ist entweder leer oder ein affiner Raum der Dimension  n-r,  das heißt ist  v in Lös(A,b),  dann  Lös(A,b) = v+Lös(A,0) sse K^n.  

Notation.. Die erweiterte Koeffizientenmatrix  (A|b) := mat{a_{11} & ... & a_{1n} & | & b_1 \\ vdots & & vdots & | & vdots \\ a_{m1} & ... & a_{mn} & | & b_m} in M(m,n+1:K).  

**Lösbarkeitskriterien**.. Sei  A in M(m,n:K), \; b in K^m.  Äquivalent sind dann folgende.. (1) Das System  A x = b  ist lösbar.. (2)  b in Bild(Phi_A)..  (3)  Rang(A) = Rang(A|b).  

Def..  A in M(m,n:K)  ist in **Zeilenstufenform**, wenn sie von der folgenden Form ist: (...).

Def..  A in M(m,n:K).  Eine **elementare Zeilenumformung** ist eine der folgenden Vorgänge.. (1) Vertauschung zweier Zeilen.. (2) Multiplikation einer Zeile mit einem Skalar.. (3) Addition des  λ\text{-fachen}  einer Zeile zu einer anderen Zeile.

Bmk..  Lös(A|b) = Lös(tilde A | tilde b)  (die mit elementaren Zeilenumformungen umgeformte Matrix).

Satz.. Sei  A in M(m,n:K), \; Rang(A) = n.  Dann ist  A x=b  eindeutig lösbar.

# Jan 29. Spaltenrang ist Zeilenrang, Ermittlung der Inversen

Satz.. Für jede  A in M(m, n:K)  gilt:  \text{Spaltenrang}(A) = \text{Zeilenrang}(A) = Rang(A).  

Bmk..  dim_K V = n, \; dim_K W = m.  Ist  phi: V to W  eine lineare Abbildung und  r = rang(phi),  dann gibt es Basen  B  von  V  und  C  von  W  mit  M_B^C(phi) = mat{I_r & 0 \\ 0 & 0} in M(m,n:K).  

Satz..  mat{A & I_n}  mit Gauß umformen ergibt  mat{I_n & A^{-1}}.  

# Jan 31. Determinante

Def..  A in M(2, 2: K).  Dann  det A = det mat{a & b \\ c & d} = vm{a & b \\ c & d} := a d - b c.  

Satz.. Parallelogramm aufgespannt von  v = (a_1, a_2)  und  w = (b_1, b_2).  Dann Fläche  = det mat{a_1 & a_2 \\ b_1 & b_2}.  

Satz.. Seien  v = (a, b) in RR^2  und  w = (c, d) in RR^2  Zeilenvektoren von  A,  schreiben  A = mat{v \\ w}..  (1)  det mat{lam v \\ w} = lam det mat{v \\ w} = det mat{v \\ lam w}..  (2)  det mat{v \\ w} = det mat{v \\ w + lam v}..  (3)  det mat{v \\ w} = 0 <=> v, w  linear unabhängig.. (4)  det mat{e_1 \\ e_2} = det mat{1 & 0 \\ 0 & 1} = 1.  

Def.. Sei  K  Körper. Eine Abbildung  det : M(n, n: K) to K  heißt **Determinante** falls: (1)  det  ist linear in jeder Zeile:  a_i = a_i' + a_i'' => det mat{vdots \\ a_i \\ vdots} = det mat{vdots \\ a_i' \\ \small vdots} + det mat{vdots \\ a_i'' \\ vdots}  und  a_i = lam a_i' => det mat{vdots \\ a_i \\ vdots} = lam det mat{vdots \\ a_i' \\ vdots}..  (2)  det  ist **alternierend**, das heißt hat  A  zwei gleichen Zeilen, so ist  det A = 0..  (3)  det  ist **normiert**, das heißt  det I_n = 1.  

Satz.. Eine Abbildung  det : M(n, n : K)  hat die folgenden weiteren Eigenschaften.. (4)  det(lam A) = lam^n det(A)..  (5) Ist eine Zeile von  A  gleich Null, so ist  det A = 0..  (6) Entsteht  B  aus  A  durch (genau eine) Zeilenvertauschung, so ist  det B = - det A..  (7) Ist  lam in K  und entsteht  B  aus  A  durch Addition der  lam\text{-fachen}  *j*-ten Zeile zur *i*-ten Zeile  (i neq j),  so ist  det B = det A..  (8) Ist  A  eine obere Dreiecksmatrix,  A = mat{lam_1 & & * \\ & ddots & \\ 0 & & lam_n},  so ist  det A = lam_1 cdot ... cdot lam_n..  (9) Sei  n ≥ 2  und  A in M(m, n : K)  von der Gestalt  A = mat{A_1 & C \\ 0 & A_2},  wobei  A_1, A_2  quadratisch. Dann gilt  det A = det(A_1) cdot det(A_2)..  (10)  det A = 0 <=> Rang(A) < n <=>  Zeilenvektoren sind linear abhängig.

# Feb 5. Permutationen

Def..  S_n := \{sigma : \{1, ..., n\} to \{1, ..., n\} : sigma \text{ bijektive Abbildung} \}  heißt Menge der **Permutationen**.

Bmk.. (1)  (S_n, circ)  ist Gruppe.. (2)  |S_n| = n!..  (3) Für  n ≥ 3  ist  S_n  nicht abelsch.

Def.. Eine Permutation  tau in S_n  heißt **Transposition** falls  τ  zwei Elemente aus  \{1, ..., n\}  vertauscht und alle anderen fest lässt.

Lemma.. Zu jedem  σ in S_n  gibt es Transpositionen  τ_1, ..., τ_k  in  S_n  mit  σ = τ_1 circ ... circ τ_k \; (n ≥ 2).  

Bmk.. Die Zerlegung einer Permutation ist nicht eindeutig.

Def.. Ist  sigma in S_n,  so nennt man jedes Paar  i, j in \{1, ..., n\}  mit  i < j  aber  σ(i) > σ(j)  einen **Fehlstand** von  σ.  Das **Signum** von  σ  ist definiert durch  sgn(σ) := 1,  falls  σ  gerade Anzahl von Fehlständen hat,  sgn(σ) := 0,  sonst.

Lemma.. Für jedes  σ in S_n  gilt:  sgn(σ) = prod_{i < j} frac{σ(j) - σ(i)}{j - i} in \{±1\}.  

Satz.. Die Abbildung  sgn : S_n to \{-1, +1\}  ist ein Gruppenhomomorphismus.

Kor.. (1) Für jede Transposition  τ in S_n  gilt  sgn(τ) = -1..  (2) Ist  σ in S_n  und  σ = τ_1 circ ... circ τ_k  mit  τ_1, ..., τ_k in S_n  Transpositionen, dann  sgn(σ) = (-1)^k.  

Kor..  det E_σ = det mat{e_{σ(1)} \\ vdots \\ e_{σ(n)}} = sgn(σ).  

Def..  A_n := Ker(sgn) = \{σ in S_n : sgn(σ) = 1\}  heißt die **alternierende Gruppe**.

Bmk..  τ in S_n, \; sgn(τ) = -1.  Dann  S_n = A_n overset . cup τ cdot A_n  (disjunkte Vereinigung).  (τ cdot A_n  ist die Linksnebenklasse  \{τ circ σ : σ in A_n\}.)  Insbesondere  |A_n| = frac{n!}{2}.  

Theorem.. Ist  K  ein Körper und  n ≥ 1,  so gibt es genau eine Determinante  det : M(n, n : K) to K  und für  A = (a_{ij})  lautet sie  det A := sum_{σ in S_n} sgn(σ) a_{1σ(1)} cdot ... cdot a_{nσ(n)}.  

# Feb 7

Satz.. Sei  A in M(n, n : K).  Es gilt  det A = det A^t.  

Folgerung.. Die Axiome für die Determinante lassen sich auch mit Spaltenvektoren formulieren.

Def.. Sei  V  ein *K*-Vektorraum, dann heiße  Phi : V times ... times V_(m-\text{mal}) to K  eine **_m_-fache Linearform**, wenn für alle  i in \{q, ..., m\}  gilt:  Phi(v_1, ..., lam v_i' + v_i'', ..., v_m) = lam Phi(v_1, ..., v_i', ..., v_m) + Phi(v_1, ..., v_i'', ..., v_m).  

Bmk.. Ist  dim V = n,  dann ist  det  *n*-fache Linearform. (?)
