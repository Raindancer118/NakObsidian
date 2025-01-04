#### <font color = "orange">Was ist RSA?</font>
**RSA** ist ein nach seinen Erfindern benanntes Kryptosystem. Seine #Verschlüsselung ist sicher und es wird häufig eingesetzt.

>[!Formeln]
>$c = m$<sup>e</sup> mod $n$
>$m = c$<sup>d</sup> mod $n$
>
>$n = p * q$
>
>$Phi(n) = (p-1) * (q-1)$
>
>$d =$ *[[Erweiterter Euklid]]*$(Phi(n),e) = t$

>[!HINT]
>**Public Key:**
>$(n,e)$
>
>**Private Key:**
>$(n,d)$

#### <font color = "orange">Was bedeuten die [[Variablen]]?</font>
$c$ ist die **verschlüsselte Nachricht**, während $m$ die **entschlüsselte Nachricht** ist. $e$ ist eine **teilerfremde Zahl** von **Phi($n$)**. Meist ist $e$ allerdings gegeben.

>[!Definition]
>Eine Teilerfremde Zahl $e$ von einer Zahl $a$ ist eine Zahl, für die der ggT($a,e$) $= 1$ ist.

$d$ ist das Ergebnis des Erweiterten Euklid von Phi$(n)$ und $e$. $d$ ist ein Teil des **private keys**.

>[!HINT]
>Für gewöhnlich sind $p,q,e$ gegeben.

#crypto