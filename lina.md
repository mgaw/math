Titel: Lineare Algebra I*
Vorlage: math

# Nov 8. Linksnebenklasse

Def. Sei  (G, cdot)  eine Gruppe und  H ≤ G.  Die Teilmenge von  PP(G),  die aus Elementen der Form  gH  besteht wird als  (G/H)  bezeichnet. Sie heißt **Linksnebenklasse** von  H.  

Lemma.  forall x, y in G : xH=yH <=> x^{-1}y in H.  

Satz. Linksnebenklassen von  H  sind Äquivalenzklassen, d.h. die Relation  ~  mit  x~y <=> xH=yH  ist eine Äquivalenzrelation.

Bmk.  G  wirkt auf  (G/H)_l  durch Multiplikation von links, d.h. für  g, x in G : g(xH) = (gx)H in (G/H)_l.  

Satz. Multiplikation von links definiert einen Gruppenhomomorphismus  L_g : (G/H)_l to (G/H)_l  mit  L_g(xH) := (gx)H.  

# Nov 13. Normalteiler, Faktorgruppe

Bsp. Sei  G  Gruppe,  H ≤ G.  Dann ist  (G/H)_l := \{gH : g in G\} sse P(G)  die Menge der
**Linksnebenklassen** von  H  in  G.  Haben Äquivalenzrelation auf *G*:
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

Bsp.  overline a in ZZ/nZZ, \; 0 ≤ a ≤ n-1.  Dann  ord(overline x) = n <=> ggt(a,n) = 1.  

Kleiner Satz von Fermat. Sei  p  Primzahl und  a in ZZ  mit  p not | \; a.  Dann gilt  a^{p-1}
equiv 1 mod p.  Außerdem gilt für alle  a in ZZ : a^p equiv a mod p.  

# Nov 20. Isomorphiesatz

Prop. Seien  a, b in ZZ, d = \text{ggT}(a, b).  Dann gibt es  x, y \in ZZ,  so dass  d=xa+yb.  

Bmk. Der  ggT(a, b)  ist die kleinste natürliche Zahl, die als lineare Kombination von a und b
darstellbar ist.

Lemma. Sei  f:G \to G'  Gruppenmorphismus. Dann ist  N:=ker(f) unlhd G.  

Def.  sgn(sigma) = (-1)^{\#\{(i,j) \;:\; i<j \text{ und } sigma(i) > sigma(j)\}}.  

Lemma.  \forall sigma \in S_n : sgn(sigma) = (Produkt) \frac{sigma(j) - sigma(i)}{j-i}.  

Def.  sigma in S_n  heißt **gerade**, gdw.  sgn(sigma) = 1.  **Ungerade**, gdw.  sgn(sigma) = -1.  

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