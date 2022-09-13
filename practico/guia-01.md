# 1
Determine si la relación dada es una relación de equivalencia sobre $\{1, 2, 3, 4, 5\}$. Si la relación es de equivalencia, indique las clases de equivalencia.

$$
A = \{1, 2, 3, 4, 5\}
$$

## (a)
$$
\{(1, 1), (2, 2), (3, 3), (4, 4), (5, 5), (1, 3), (3, 1)\}
$$

- Es `reflexiva` ya que $\forall a  \in A, aRa$.
- Para $\forall a,b \in A$ si
    - $a = b, aRb \land bRa$ por ser `reflexivo`,
    - para $a \ne b$, solo están relacionados $1R3$ y $3R1$,
    - y para $a,b \not \in \{1, 3\}, a \ne b$, entonces $a\not R b$.
    - Luego $\forall a,b \in A, aRb \Rightarrow bRa$, por ende, es `simétrico`.
- Para $\forall a,b,c \in A$ si
    - Solo se tienen $a = c = 1, b = 3$ o $a = c = 3, b = 1$ tal que $aRb \land bRc$ y estos sí cumplen que $aRc$
    - para el resto de casos, no existen $a,b,c \in A$ tal que $aRb \land bRc$.
    - Por ende, $\forall a,b,c \in A, aRb \land bRc \Rightarrow aRc$, es decir, es `transitivo`.
- Como es `reflexivo`, `simétrico` y `transitivo`, es `equivalencia`.
$$
\begin{array}{c}
[1] &=& \{1, 3\} \\
[2] &=& \{2\} \\
[4] &=& \{4\} \\
[5] &=& \{5\} \\
\end{array}
$$
Entonces
$$
A/_R = \{[1], [2], [4], [5]\} = \{\{1, 3\}, \{2\}, \{4\}, \{5\}\}
$$

## (b)
$$
\{(1, 1), (2, 2), (3, 3), (4, 4)\}
$$

- No es `reflexiva` ya que $5 \not{R} 5$ y $5 \in A$, por ende, no es `equivalente`.

## (c)
$$
\{(x, y)\ |\ 1 ≤ x ≤ 5, 1 ≤ y ≤ 5\}
$$

Tenemos que $\forall x, \exist (x, 1), (x, 2), (x, 3), (x, 4), (x, 5)$ y $\forall y, \exist (1, y), (2, y), (3, y), (4, y), (5, y)$.

- Es `reflexiva` ya que $\forall a  \in A, aRa$, pues existen $(a, a)$,
- es `simétrica` ya que $\forall a,b \in A, \exist (a, b), (b, a) \in R$,
- es `transitiva` ya que $\forall a,b,c \in A, \exist (a, b), (b, c) \in R$, por ende, $aRb \land bRc$, y además, se tiene para todo $a \in A$ existen $(a, 1), (a, 2), (a, 3), (a, 4), (a, 5)$, por ende $aRc$.
- Como es `reflexiva`, `simétrica` y `transitiva`, es `equivalencia`.
$$
\begin{array}{c}
[1] &=& \{1, 2, 3, 4, 5\} \\
\end{array}
$$

Entonces

$$
A/_R = \{[1]\} = \{\{1, 2, 3, 4, 5\}\}
$$

# 2
Determine si las siguientes relaciones sobre $\Z$ son `reflexivas`, `simétricas`, `antisimétricas` o `transitivas`:

## (a)
$$
(x, y) ∈ \R \text{ sii } x^2 = y^2
$$

Tenemos que para todo $x$, existen solamente $(x, -x), (x, x) \in R$.

- Es `reflexiva`, pues $a^2 = a^2, \forall a \in \Z$.
- Es `simétrica`, pues $a^2 = b^2 \Leftrightarrow b^2 = a^2, \forall a,b \in \Z$.
- No es `antisimétrica`, pues $1^2 = -1^2 \land -1^2 = 1^2$, pero $1 \ne 1$.
- Es `transitiva`, pues solo hay dos casos para todo $x$, y ambos son triviales.

## (b)
$$
(x, y) ∈ \R \text{ sii } x > y
$$

- No es `reflexiva`, pues no puede existir el par $(a, a), \forall a \in \Z$, ya que $a \not > a$.
- No es `simétrica`, pues no pueden existir los pares $(a, b), (b, a), \forall a \in \Z$, ya que implicaría que $a > b \land b > a$, y sabemos que siempre va a existir un $n \in \Z$ tal que $a > n$, por ser $a \in \Z$.
- Es `antisimétrica`, ya que para $a,b \in \Z$, de existir $aRb$, no puede existir $bRa$.
- Es `transitiva`, pues $\forall a,b,c \in \Z, a > b \land b > c \Rightarrow a > c$.

## (c)
$$
(x, y) ∈ \R \text{ sii } x ≥ y
$$

- Es `reflexiva`, pues existe $(x,x) \in R$, para todo $x$, por ser $x = y \lor x < y$.
- No es `simétrica`, pues no existen $(x,y) \in R$, tal que para todo $x \ge y \land y \ge x$, salvo el caso trivial de la reflexividad.
- Es `antisimétrica`, pues para todo par $(x,y) \in R$, tal que para todo $x \ge y \land y \ge x$, se cumple que $x = y$.
- Es `transitiva`, pues para todo $a,b,c \in \R$ se cumple que si $a \ge b \land b \ge c$, entonces $a \le c$.

## (d)
$$
(x, y) ∈ \R \text{ sii } x \ne y
$$

- No es `reflexiva` por definición de la relación.
- Es `simétrica`, pues si existe $(x,y) \in R$, entonces como $x \ne y \land y \ne x$, entonces $(y,x) \in R$.
- No es `antisimétrica`, pues es `simétrica` pero no `reflexiva`, entonces se cumple $(x,y), (y,x) \in R$, pero no $x = y$.
- No es `transitiva`, pues para si tomamos $(x,y) \in R$ se cumple que $x \ne y \land y \ne x$ pero es falso que $x \ne x$.

# 3
Utilizando las respuestas del ejercicio $(2)$ determine para cada caso si la relación es de equivalencia y/o de orden. Recuerde que una relación de orden debe ser reflexiva, antisimétrica, y transitiva.

- $(a)$ es de `equivalencia`.
- $(b)$ no es nada.
- $(c)$ es de `order`.
- $(d)$ no es nada.

# 4
Sea $A$ un conjunto y $f$ una función definida en $A$. Probar que la relación $\{⟨x, y⟩ ∈ A × A : f (x) = f (y)\}$ es una relación de equivalencia sobre $A$. Comparar con $2a$.

- Es `reflexiva`, pues $f(x) = f(x), \forall x \in A$.
- Es `simétrica`, pues $f(x) = f(y) \Leftrightarrow f(y) = f(x), \forall x,y \in A$.
- Es `transitiva`, pues $\forall a,b,c \in A, f(a) = f(b) \land f(b) = f(c) \Rightarrow f(a) = f(c)$.

> $$
> f^\prime (x) = x^2 \sube \{⟨x, y⟩ ∈ A × A : f (x) = f (y)\}
> $$

# 5
Utilizando como motivación con los ejercicios $2b$ y $2c$, responda:

## (a) 
Sea $R$ una relación irreflexiva y transitiva (“relación de orden parcial estricto”) sobre un conjunto $A$. Probar que $R ∪ Igualdad_A$ es una relación de orden parcial sobre $A$.

> Al añadirle a $R$ la relación $Igualdad_A$, le estamos dando la propiedad de `reflexividad`, por ende, va a existir la relación $xRx$, para algún $x \in A$, y como $x$ no puede ser mayor ni menor a sí mismo, la relación de orden deja de ser estricta.

## (b)
¿Cómo se podrá obtener una relación de orden parcial estricto a partir de una relación de orden parcial?

- Sea $R$ relación de orden parcial, 
$$
Q = \{⟨x, y⟩ ∈ A × A : xRy \land x \ne y\}
$$
- Por ende, $Q$ es de orden parcial y estricto.

# 6
Liste los pares de la relación de equivalencia sobre $\{1, 2, 3, 4\}$ definida por la partición dada. También señale las clases de equivalencia $[1], [2], [3]$ y $[4]$.

## (a)
$\{1, 2\}, \{3, 4\}$ 

$$
\begin{array}{c}
R_{\{1, 2\}} = \{(1,1),(2,2),(1,2),(2,1)\} = \{[1]\} \\
R_{\{3, 4\}} = \{(3,3),(4,4),(3,4),(4,3)\} = \{[3]\} \\
\\
R = \{[1], [3]\}
\end{array}
$$

## (b)
$\{1\}, \{2\}, \{3\}, \{4\}$

$$
\begin{array}{c}
R_{\{1\}} = \{(1,1)\} = \{[1]\} \\
R_{\{2\}} = \{(2,2)\} = \{[2]\} \\
R_{\{3\}} = \{(3,3)\} = \{[3]\} \\
R_{\{4\}} = \{(4,4)\} = \{[4]\} \\
\\
R = \{[1], [2], [3], [4]\}
\end{array}
$$

# 7
Sea $R$ la relación “Fulano no es más viejo que Mengano” sobre un conjunto de personas $A$.

## (a) 
De un ejemplo, puede ser ficticio, de un conjunto $A$ de personas en los cuales esa relación no sea un orden parcial.

> Llamemos a “Fulano no es más viejo que Mengano” como $R$, tomamos $a,b \in A$ tales que $a,b$ son gemelos.

## (b) 
Explique qué propiedad falla para que sea un orden parcial.

> Es claro que $aRb \land bRa$, y como no son la misma persona, $R$ no es antisimétrica y se rompe así, la relación de orden parcial
