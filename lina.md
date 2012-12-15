Titel: Lineare Algebra I*
Vorlage: math

# Nov 8. Linksnebenklasse

Def. Sei  (G, cdot)  eine Gruppe und  H ≤ G.  Die Teilmenge von  PP(G),  die aus Elementen der Form  gH  besteht wird als  (G/H)_l  bezeichnet. Sie heißt Menge der **Linksnebenklassen** von  H.  

Lemma.  forall x, y in G : xH=yH <=> x^{-1}y in H.  

Satz. Die Relation  ~_l  mit  x~_ly <=> xH=yH  ist eine Äquivalenzrelation. Die Linksnebenklassen von  H  sind also Äquivalenzklassen, das heißt  overline x = xH.  

Bmk.  G  wirkt auf  (G/H)_l  durch Multiplikation von links, das heißt für  g, x in G : g(xH) = (gx)H in (G/H)_l.  

Satz. Multiplikation von links mit einem bestimmten Element  g in GG  definiert einen Gruppenhomomorphismus  L_g : (G/H)_l to (G/H)_l  mit  L_g(xH) := (gx)H.  

# Nov 13. Normalteiler, Faktorgruppe

Bsp. Sei  G  Gruppe,  H ≤ G.  Dann ist  (G/H)_l := \{gH : g in G\} sse P(G)  die Menge der
Linksnebenklassen von  H  in  G.  Haben Äquivalenzrelation auf *G*:
  x sim_l y :<=> x^{-1}y in H.  Dann ist  overline x = \{y in G : x sim_l y\} = \{y in G : x^{-1}y
= h in H\} = \{y in G : y = xh, h in H\} = xH.  

Def. Eine Untergruppe  H  einer Gruppe  G  heißt **Normalteiler**, wenn  forall h in H, g in G:
g^{-1}hg in H.  Dann schreibt man  H unlhd G.  

Bmk. Für abelsche Gruppen gilt, dass jede Untergruppe ein Normalteiler ist.

Satz. Sei  H unlhd G,  dann kann man die Verknüpfung  (G/H)_l times (G/H)_l to (G/H)_l  mit  (xH,
yH) mapsto xyH  definieren.

Bmk. Sei  H ≤ G.  Dann ist  H unlhd G <=> gH=Hg, \; forall g in G.  Die Linksnebenklassen sind also
die Rechtsnebenklassen sind die Nebenklassen.

Satz. Ist  H unlhd G,  dann ist  ((G/H), cdot)  eine Gruppe. Man nennt sie **Faktorgruppe**.

Def. Sei  H ≤ G.  Dann heißt  [G:H] := |(G/H)_l|  der **Index** von  H  in  G.  

Satz von Lagrange. Sei  G  endliche Gruppe,  H ≤ G.  Dann  |G| = |H| cdot [G:H].  

Kor. Die Ordnung einer Untergruppe teilt die Ordnung der Gruppe:  |H|\;|\;|G|.  

# Nov 15. Kleiner Satz von Fermat

Satz von Lagrange anders.  G  endliche Gruppe,  H ≤ G.  Dann gibt es eine Bijektion  (G/H)_l times 
H to G.  

Bmk. Die Anzahl der Links- und Rechtsnebenklassen ist gleich, d.h.  [G:H] = |(G/H)_l| = |(G/H)_r|.  

Kor. Ist  G  endliche Gruppe,  n = |G|, x in G.  Dann  ord (x) \; | \; |G|,  d.h.  x^n = e, \; forall x in G.  

Bsp.  overline a in ZZ/nZZ, \; 0 ≤ a ≤ n-1.  Dann  ord(overline x) = n <=> ggT(a,n) = 1.  

Kleiner Satz von Fermat. Sei  p  Primzahl und  a in ZZ  mit  p not | \; a.  Dann gilt  a^{p-1}
equiv 1 mod p.  Außerdem gilt für alle  a in ZZ : a^p equiv a mod p.  

# Nov 20. Isomorphiesatz

Prop. Seien  a, b in ZZ, \; d = \text{ggT}(a, b).  Dann gibt es  x, y \in ZZ,  so dass  d=xa+yb.  

Bmk. Der  ggT(a, b)  ist die kleinste natürliche Zahl, die als lineare Kombination von a und b
darstellbar ist.

Lemma. Sei  f:G \to G'  Gruppenmorphismus. Dann ist  N:=ker(f) unlhd G.  

Def.  sgn(sigma) = (-1)^{\#\{(i,j) \;:\; i<j \text{ und } sigma(i) > sigma(j)\}}.  

Lemma.  \forall sigma \in S_n : sgn(sigma) = (Produkt) \frac{sigma(j) - sigma(i)}{j-i}.  

Def.  sigma in S_n  heißt **gerade**, falls  sgn(sigma) = 1. \; sigma heißt **ungerade**, falls  sgn(sigma) = -1. 

Def.  ker(sgn) = A_n = \{ sigma in S_n : sgn(sigma) = 1 \}  heißt die **alternierende Gruppe**.

Bmk.  A_n unlhd S_n.    |A_n| = \frac{n!}{2}.  

Isomorphiesatz. Sei  phi : G to G'  Gruppenmorphismus, damit  ker(phi) unlhd G.  Dann gibt es einen kanonischen Isomorphismus von Gruppen  overline φ : G/ker(φ) \xrightarrow{\simeq} φ(G).  
  (φ(G) ≤ G'  Untergruppe.)  phi = overline phi circ pi. \; pi  ist die Projektion, die ein Element aus  G  auf seine Nebenklasse abbildet. Eigentlich nur:  overline φ : G/ker(φ) to G'  ist injektiv. Aber wenn  phi(G)=G'  dann surjektiv und damit auch bijektiv.

Bmk. Falls  φ  surjektiv ist, d.h.  φ(G) = G',  dann bildet  overline φ  nach  G'  ab.

# Nov 20 (Übung)

Satz.  G  Gruppe,  overline x cdot overline y := overline {x cdot y}. quad (G/H, cdot)  ist Gruppe,
gdw.  H unlhd G.  

Prop.  G  Gruppe,  overline x cdot overline y := overline {x cdot y}, H unlhd G. quad π : (G, cdot)
 to (G/H, cdot), \; x mapsto overline x  ist Gruppenhomomorphismus.

# Nov 22. Ring, Körper

Def. Eine Menge  R  zusammen mit zwei Verknüpfungen  +: R times R to R  und  cdot : R times R to R  
heißt **Ring**, wenn (i)  (R, +)  ist abelsche Gruppe mit neutralem Element  0 in RR,  (ii) "
  cdot  " ist assoziativ und (iii) es gilt Distributivität.

Def. Ein Ring heißt **kommutativ**, wenn  a cdot b = b cdot a, \; forall a, b in R.  

Def.  0 in R  heißt das **Nullelement**.

Def. Ein Element  1 in R  heißt **Einselement**, wenn  1 cdot a = a cdot 1 = a, \; forall a in R.  
Ein Ring mit Einselement heißt **Ring mit Eins**.

Prop. Sei  R  ein Ring,  0 in R  das Nullelement. Dann gilt (i)
  0 cdot a = a cdot 0 = 0, \; forall a in R  und (ii) falls  R  Ring mit Eins ist, dann
  (-1) cdot a = -a,  wobei  -a in R : a + (-a) = 0.  

Def.  (R, +, cdot), (R', oplus, odot)  Ringe. Eine Abbildung  phi : R to R'  heißt **Morphismus von
Ringen**, wenn  forall a, b in R  (i)  phi(a+b) = phi(a) oplus phi(b)  und (ii)
  phi(a cdot b) = phi(a) odot phi(b).  

Satz. (i) gdw.  phi : (R, +) to (R', oplus)  ist Morphismus von abelschen Gruppen.
(ii) gdw.  phi : (R, cdot) to (R', odot)  ist Monoidmorphismus.

Def.  phi  ist **Isomorphismus**, wenn  phi  ist bijektiver Morphismus.

Def. Ein Ring mit Eins  (K, +, cdot)  heißt **Körper**, gdw.  (K^* = K setminus \{0\}, cdot)  ist abelsche Gruppe.

# Nov 27. Komplexe Zahlen

Satz.  (CC := RR^2, +, cdot)  bildet einen Körper.

Bmk. Wir können  RR  als Untermenge von  CC  betrachten wie folgt.  phi : RR to CC  mit  phi(a) := (a, 0).  Dann ist  phi  ein Ringhomomorphismus.

Satz. Seien  x, y in CC.  Dann folgt: (1)  overline{x+y} = overline x + overline y,  (ii)  overline{x cdot y} = overline x cdot overline y  und (iii)  x in RR <=> x = overline x.  Aus (i) und (ii) folgt, dass  x mapsto overline x  Ringhomomorphismus ist.

# Nov 29. Polynomkörper

Def.  x in CC.  Dann  |x|:=sqrt{x cdot overline x}.  

Satz.  x, y in CC. \;|x + y| ≤ |x| + |y|. \;|x cdot y| = |x| cdot |y|. \; x = |x| cdot cos phi + i|x| sin phi = |x|(cos phi + i sin phi) = |x|e^{i phi} = |x|e^{i cdot \arg(x)}.  Bisher gilt  e^{i phi} := cos phi + i sin phi.  

Def. Sei  R  ein Ring. Ein Element  x in R^*  heißt **Nullteiler**, falls es ein  y in R*  gibt, so dass  x cdot y = 0_R  ist. Ein Ring ohne Nullteiler heißt **nullteilerfrei**.

Satz. Jeder Körper ist nullteilerfrei.

Def. Ein kommutativer, nullteilerfreier Ring mit 1 heißt **Integritätsbereich**.

Bmk. Jeder Körper ist Integritätsbereich.

Lemma. Ein Integritätsbereich mit endlich vielen Elementen ist ein Körper.

Bmk. Sei  k  Primzahl. Dann ist  ZZ/pZZ  Körper und wird mit  FF_2  bezeichnet.

Def. Sei  R  ein Ring mit 1. Dann heißt  char(R) := 0  falls  n cdot 1_R neq 0_R  für alle  n in NN_{>0}  und  char(R) := min \{n in NN_{>0} : n cdot 1_R = 0_R\}  die **Charakteristik** von  R.  

Satz. Sei  K  Körper. Dann ist  char(K)  entweder 0 oder eine Primzahl.

Bmk. Ist  K  ein endlicher Körper, so ist  char(K) = p > 0  und es ist  |K|=p^n, \; n in NN_{>0}  und es gibt einen injektiven Ringhomomorphismus  FF_k to K.  

Def. Der Körper  FF_p  heißt **Primkörper** der Charakteristik  p.  

Def. Sei  K  Körper. Ein **Polynom** mit Koeffizienten in  K  in der Unbestimmten  t  ist ein Ausdruck der Form  f = f(t) = a_0 + a_1 t + a_2 t^2 + ... + a_n t^n  mit  a_0, ..., a_n in K, \; n in NN. \; K[t]  ist die Menge aller solchen Polynome.  f=0  heißt **Nullpolynom**.  deg(f) := max \{n in NN : a_n neq 0\}  heißt **Grad** von  f.  Das Polynom heißt **normiert**, falls  a_n = 1,  wobei  n = deg f.  

Bmk. Man kann für  t  ein  x in K  einsetzen, dann ist  f(x) in K.  Ein Polynom induziert also eine Abbildung  tilde f : K to K, \; x mapsto f(x).  

Bmk.  f mapsto tilde f  ist nicht injektiv, da  tilde f  Nullabbildung sein kann, obwohl  f  nicht Nullpolynom ist.

Satz.  (K[t])  ist mit den folgenden Operationen  +  und  cdot  ein Ring. Sei  f(t) = sum^m_{i=0} a_i t^i, \; g(t) = sum^n_{i=0}.  Dann  (f+g)(t) := sum^{max (m, n)}_{i=0} c_k t^k, \; c_k = a_k+b_k  und  (f cdot g)(t) := sum^{m+n}_{i=0}d_k t^k, \; d_k = sum_{i+j=k}a_i b_j.  

Bmk. Für den Grad der Polynome gilt  deg(f+g) ≤ max (deg f, deg g)  und  deg(f cdot g) = deg f + deg g,  wobei  -infty + n := -infty  und  max (-infty, n) := n.  

Satz. Seien  f, g in K[t]  mit  g neq 0.  Dann existieren eindeutig bestimmte  q, r in K[t],  so dass  f=qg+r  ist und  deg(r) < deg(g).  

# Dez 4. Polynomteiler, Vielfachheit von Nullstellen

Satz (Division mit Rest). Sei  K  Körper,  f,g in K[t]  Polynome. Dann existieren  q(t), r(t)  eindeutig bestimmt in  f=gq+r  mit  deg(r) < deg(g).  

Def. Sei  f in K[t]. \; lam in K  heißt **Nullstelle**, falls  f(lam) = 0.  

Kor.  lam in K  Nullstelle von  f <=> (t-lam) | f :<=> exists q in K[t]  mit  f=(t-lam)q.  

Satz. Sei  K  Körper,  f in K[t], \; f neq 0, \; deg(f) = n.  Dann besitzt  f  höchstens  n  Nullstellen.

Def.  f in K[t], \; f neq 0, \; lam in K  Nullstelle. Die **Vielfachheit** von  lam,  ausgedrückt durch  mü(f, lam),  ist die größte natürliche Zahl  r  mit  (t-lam)^r | f.  

Bmk.  mü(f, lam) ≥ 1  heißt, dass  lam  Nullstelle ist.

Kor.  f in K[t]  Polynom,  lam_1, ..., lam_s  die verschiedenen Nullstelllen von  f,  das heißt  r_i = mü(f, lam) ≥ 1.  Dann gibt es ein  g in K[t]  mit  f=(t-lam_1)^{r_1} cdot (t-lam_2)^{r_2} cdot ... cdot (t-lam_s)^{r_s} cdot g.  Anders ausgedrückt: Produkt von i=1 bis s  (t-lam_i)^{r_i} | f.  

Satz.  sin(alpha+beta) = sin alpha cos beta + sin beta cos alpha.  

Satz. Sei  w=re^{i theta} in CC.  Dann besitzt das Polynom  z^n-w in CC[z] \; n  verschiedene Nullstellen, das heißt es existieren  n  verschiedene komplexe Zahlen  z_1, ..., z_n  mit  z_i^n = w.  Schreiben  sqrt[n] w := \{z_1, z_2, ..., z_n\}.  

# Dez 4. Ideal (Übung)

Satz. Ein Homomorphismus  phi  zwischen Ringen mit trivialem Kern  ker(phi) = varnothing  ist injektiv.

Def. Sei  (X, +, cdot)  ein Ring. Eine Menge  I sse X  heißt **rechtes (linkes) Ideal**, falls (i)  (I, +)  ist Untergruppe und (ii)  X cdot I sse I \; (I cdot X sse I).  

# Dez 6. Fundamentalsatz der Algebra, Vektorraum

Satz.  z=re^{i theta} in CC. \; z^n = w <=> z = sqrt[n] w = \{sqrt[n]r (cos frac{theta + 2k pi} n + i sin frac{theta + 2k pi} n) : k in \{0, 1, ..., n-1\} \}.  

Folgerung. Für  n=2  gilt  sqrt w = \{sqrt r (cos frac theta 2 + i sin frac theta 2), \; -sqrt r (cos frac theta 2 + i sin frac theta 2)\}  (wegen  cos (x + pi) = -cos x).  

Satz. Sei  az^2 + bz + c=0, \; a neq 0.  Dann  z=-frac{b +- sqrt{b^2-4ac}}{2a}.  

Prop. Ist  f in RR[t]  ein *reelles* Polynom und  lam in CC  eine Nullstelle von  f.  Dann ist  overline lam in CC  eine Nullstelle von  f.  Es gilt sogar  mü(f, lam) = mü(f, overline lam).  

Satz: Fundamentalsatz der Algebra. Jeder Polynom  f in CC[t]  mit  deg(f) > 0  hat mindestens eine Nullstelle.

Kor. Jedes Polynom  f in CC[t]  zerfällt in Linearfaktoren, das heißt es gibt  lam_1, ..., lam_n in CC  mit  f(t) = a(t-lam_1)(t-lam_2)...(t-lam_n).  

Prop. Sei  K  unendlicher Körper. Dann ist die Abbildung  K[t] to Abb(K, K)  injektiv.

Def. Sei  K  ein Körper. Eine Menge  V  mit einer inneren Verknüpfung  +:V times V to V  und einer äußeren Verknüpfung  cdot : K times V to V  heißt **K-Vektorraum**, wenn gilt: (1)  (V, +)  ist abelsche Gruppe mit neutralem Element  0 in V.  (2) Verträglichkeiten für  lam, mü in K, \; v, w in V,  nämlich (i)  (lam + mü)v = lam v + mü v,  (ii)  lam(v+w) = lam v + lam w,  (iii)  lam(mü v) = (lam mü) v  und (iv)  1v = v.  

# Dez 11. Untervektorraum, lineare Unabhängigkeit

Satz, Rechenregeln. a)  0_K cdot v = 0 in V.  b)  lam cdot 0 = 0.  c)  lam cdot v = 0 \;=>\; lam = 0  oder  v = 0.  d)  (-1) cdot v = -v,  das additiv Inverse zu  v.  

Def. Sei  V  ein K-Vektorraum. Eine Teilmenge  W sse V  heißt **Untervektorraum** (man
schreibt  W ≤ V),  falls gilt: (UV1)  W neq varnothing.  (UV2)  v, w in W \;=>\; v+w in W.  (UV3)  v in W, lam in K \;=>\; lam cdot v in W.  (Nichtleer und abgeschlossen gegenüber  +  und  cdot.)  

Bmk. Wegen (UV2) und (UV3) erhalten wir induzierte Operationen  +_W : W times W to W  und  cdot_W : K times W to W.  

Satz. Sei  W  ein UVR. Dann ist  (W, +_W, cdot_W)  ein Vektorraum.

Lemma. Sei  V  ein VR und  (W_i)_{i in I}  eine Familie von UVR von V. Dann ist auch  W := bigcap_{i in I} W_i  ein UVR.

Lemma. Sei  V  ein K-Vektorraum und  W_1, W_2 ≤ V.  Dann gilt:  W_1 cup W_2 ≤ V \;<=>\; W_1 sse W_2  oder  W_2 sse W_1.  

Def. Sei  v_1, ..., v_r in V:  Ein beliebiger Vektor  v in V  heißt **Linearkombination** von  v_1, ... v_r,  falls es  lam_1, ..., lam_r in K  gibt, so dass  v = lam_1 v_1 + ... + lam_r v_r.  

Def. Sei  M sse V  eine Teilmenge. Die Menge aller Linearkombinationen von *endlich vielen* Vektoren aus  M  heißt **Lineare Hülle** (oder **Spann**) von  M.  Man schreibt  langle M rangle  oder  span_K(M).  

Satz. Sei  V  ein Vektorraum und  M sse V  eine Teilmenge. Dann ist  langle M rangle  der kleinste UVR von  V,  der  M  enthält, das heißt (a)  langle M rangle  ist ein UVR und (b) Ist  W ≤ V  ein UVR mit  M sse W,  so gilt  langle M rangle sse W.  

Def. Sei  V  ein Vekorraum. Eine endliche Familie  (v_1, ..., v_k)  von Vektoren in  V  heißt **linear unabhängig**, wenn für alle  lam_1, ..., lam_r in K  gilt:  (lam_1v_1 + ... + lam_rv_r = 0) \;=>\; (lam_1 = ... = lam_r = 0),  das heißt der Nullvektor lässt sich nur auf *eine* (triviale) Art als Linearkombination der  v_i  schreiben. Eine unendliche Familie  (v_i)_{i in I}  heißt linear unabhängig, wenn jede endliche Teilfamilie linear unabhängig ist. Eine Familie, die nicht linear unabhängig ist, heißt **linear abhängig**.

Lemma. (a)  \{v\}  ist genau dann linear unabhängig, wenn  v = 0.  (b) Jede Familie, die den Nullvektor enthält, ist linear abhängig. (c) Eine Familie, die einen Vektor doppelt enthält, ist linear abhängig. (d) Zwei oder mehr Vektoren  v_1, ..., v_r  sind genau dann linear abhängig, wenn einer davon im Spann der anderen liegt.

# Dez 11. Maximales Ideal, Primideal (Übung)

Prop. Seien  p, q in NN^*.  Dann  pZZ + qZZ = ggT(p,q)ZZ.  

Theorem. Seien  p, q in NN^*  und  d = ggT(p,q).  Dann existieren  s, t in ZZ  so, dass  sp+tq = d.  

Def. Zwei Ideale  A, B  eines Ringes  R  heißen **fremd**, falls  A+B=R.  

Kor.  pZZ  und  qZZ  sind genau dann fremde Ideale, wenn  ggT(p,q)=1.  

Def. Sei  (X, +, cdot)  ein kommutativer Ring. Ein Ideal  I sse X  heißt **Primideal**, falls  xy in I => x in I  oder  y in I. \; I  heißt **maximal**, falls  J  Ideal von  X  und  I sse J sse X \;=>\; J = I  oder  J = X.  

Satz.  pZZ  ist genau dann Primideal von  ZZ,  wenn  p  Primzahl ist.

Satz. Sei  I sse ZZ, x in X setminus I.  Dann gilt  J := displaystyle bigcap_{tilde J \text{ Ideal, } I cup \{x\} sse tilde J} = \{i+kx : i in I, k in ZZ\} =: H.  

Satz. Sei  I  ein maximales Ideal von  ZZ.  Dann ist  I  Primideal.
