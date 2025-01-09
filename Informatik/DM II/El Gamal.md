>[!QUOTE]
>*"Können wir nochmal Gagamel an der Tafel machen?"*
>    ~ J. Voß, 2024
#### <font color = "orange">Wie funktioniert El Gamal?</font>
El Gamal arbeitet mit dem [[Diffie-Hellmann-Key-Exchange-Verfahren]], das es erlaubt, Schlüssel auszutauschen, theoretisch ohne, dass ein Mithörer diese nutzen könnte, um Nachrichten zu entschlüsseln.

>[!Formeln]
>**Schlüssel:**
>$x = g$<sup>a</sup> mod $p$
>$y = g$<sup>b</sup> mod $p$
>$z = y$<sup>a</sup> mod $p$
>$z = x$<sup>b</sup> mod $p$
>$z = g$<sup>a*b</sup> mod $p$  <- Diese Formel benutzt Eve, wenn sie an sowohl $a$ als auch $b$ kommt.

Zunächst wird das [[Diffie-Hellmann-Key-Exchange-Verfahren]] angewendet. Aus diesem entstehen die privaten und öffentlichen Schlüssel, die in El Gamal verwendet werden können.

>[!HINT]
>**Verschlüsselung:**
>$c = m*$public key<sup>private key</sup> mod $p$
>$m = y$<sup> p-1-a</sup> $* c$ mod $p$

>[!Example]
>Die Nachricht $m$ soll von Bob verschlüsselt werden. Dafür nutzen wir Alice' Public Key $x$ und Bobs Private Key $b$. So kommt zustande:
>$c =m*x$<sup>b</sup> mod $p$
>Diese Nachricht soll nun auch von Alice entschlüsselt werden. Sie nutzt dafür ihren Private Key $a$ und Bob's Public Key $y$. So kommt zustande:
>$m = y$<sup>p-1-a</sup> $*c$ mod $p$