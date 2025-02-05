# <font color = "orange">Pfeildiagramm</font>
>[!INFO] Definition
>Pfeildiagramme erlauben die Darstellung von [[DM II - Relation|Relationen]] in einer visuellen Form. [[DM II - Relation|Relationen]] werden dabei als Pfeile vom ersten Element zum zweiten Element gezogen. Es können dabei auch mehrere Pfeile zum selben Element oder vom selben Element wegführen. Diese Diagramme sind normalerweise von links nach rechts ausgerichtet, doch Mermaid erlaubt dies nicht anders.
>Dies könnte dann beispielsweise so aussehen:
>>[!EXAMPLE] 
>>```mermaid
>>graph TD
>>1 --> a
>>2 --> a
>>2 --> b
>>2 --> c
>>3 --> c
>>3 --> d
>>3 --> e
>>```
