# <font color = "orange">Branch</font>
>[!INFO] Definition
>Ein Branch ist ein Entwicklungszweig, der die parallele Entwicklung eines Repositories in zwei verschiedene Richtungen erlaubt. Diese Änderungen stören einander nicht und können schließlich verglichen oder zusammengeführt werden.

>[!TIP] Tipp
>Es wird empfohlen, den Main-Branch immer lauffähig zu halten und parallel dazu Feature-Branches anzulegen, auf denen Features entwickelt werden. Diese kann schließlich, nach fertiger Entwicklung, auf den Main-Branch gemerged werden.
## Befehle
>[!HOWTO] Einen neuen Branch anlegen
>Der Befehl `git branch [branchName]` legt einen neuen Branch an.

>[!HOWTO] Zu einem Branch wechseln
>Der Befehl `git checkout [branchName]` wechselt zu einem anderen Branch. Dieser wird ausgecheckt, sodass auf ihm gearbeitet werden kann.

>[!HOWTO] Branches anzeigen
>Der Befehl `git branch` ohne weitere Argumente führt alle vorhandenen Branches auf.

>[!HOWTO] Zwei Branches mergen - Fast Forward
>Zunächst einmal muss der Branch ausgecheckt werden, in den gemerged werden soll. Dafür wird der Befehl `git checkout [branchName]` genutzt. Anschließend wird dann `git merge [branchToMerge]` genutzt, mit dem Branch als Argument, der auf den anderen gemerged werden soll.
>**Per Default wird der *Fast Forward*-Merge** genutzt.
