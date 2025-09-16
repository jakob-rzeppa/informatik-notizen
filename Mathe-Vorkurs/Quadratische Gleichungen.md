## Lösen von Quadratischen Gleichungen

### PQ-Formel

$$
x^2+px+q = 0
$$

$$
x_{1,2} = -\Big(\frac{p}{2}\Big) \pm \sqrt{\Big(\frac{p}{2}\Big)^2 - q}
$$

### Reelle Lösungen bei Quadratischen Gleichungen

Die Lösungen hängen vom Radikanten (der Ausdruck unter dem Wurzelzeichen), der sogenannten Diskriminante, also p und q ab.

Mit $x^2+px+q = 0$ gilt:

Die Lösungen hängen von dem Radikanten (Ausdruck unter der Wurzel), auch Diskriminante genannt, ab.

1. $(\frac{p}{2})^2 - q > 0$: zwei reelle Lösungen
2. $(\frac{p}{2})^2 - q = 0$: eine reelle Lösung
3. $(\frac{p}{2})^2 - q < 0$: keine reelle Lösung

### Nullprodukt

Q: Was besagt der Satz des Nullprodukts?
A: Ein Produkt wird null, wenn mindestens ein Faktor null ist.
<!--ID: 1757918644971-->

Kann genutzt werden, um Quadratische Gleichungen zu lösen:

$$
\begin{align}
x^2 - 49 &= 0\\
(x + 7)(x - 7) &= 0\\
\\
\Rightarrow x_1 &= 7\\
x_2 &= -7
\end{align}
$$

### Substitution

$$
x^4 - x^2 - 6 = 0
$$

Substitution mit $x^2 := z$

$$
\begin{align}
z^2 - z - 6 &= 0\\
z_{1,2} &= -\Big(\frac{1}{2}\Big) \pm \sqrt{\Big(\frac{1}{2}\Big)^2 + 6}\\
z_{1,2} &= -\Big(\frac{1}{2}\Big) \pm \sqrt{\frac{1}{4} + \frac{24}{4}}\\
z_{1,2} &= -\Big(\frac{1}{2}\Big) \pm \sqrt{\frac{25}{4}}\\
\Rightarrow z_1 &= 3\\
z_2 &= -2
\end{align}
$$

Resubstitution:

$$
\begin{align}
z_1 &= 3\\
z_2 &= -2\\
\\
z_1 = x^2 = 3\\
\Rightarrow x_{1} &= \sqrt{3}; x_{2} = -\sqrt{3}\\
\\
z_2 &= x^2 = -2\\
\Rightarrow &\text{keine weiteren reellen Nullstellen}
\end{align}
$$