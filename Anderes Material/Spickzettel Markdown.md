# Markdown Spickzettel

## Textformatierung
- **Fett**: `**Text**` oder `__Text__`
- *Kursiv*: `*Text*` oder `_Text_`
- ***Fett & Kursiv***: `***Text***`
- ~~Durchgestrichen~~: `~~Text~~`
- Unterstrichen (nur HTML): `<u>Text</u>`
- Hervorhebung (HTML): `<mark>Text</mark>`

## Überschriften
Markdown nutzt `#` für Überschriften:

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
````

## Callouts
Ich habe einige Callout-Typen hinzugefügt. Overall gibt es jetzt also folgende Callout-Typen:
### Custom
>[!CODE]

>[!EXTRA]

>[!FORMULA]

>[!GOAL]

>[!HowTo]

>[!STRENGTHS]

>[!TAG]

>[!Weaknesses]

### Native Obsidian
>[!HINT]

>[!TIP]

>[!NOTE]

>[!WARNING]

>[!DANGER]

>[!DONE]

>[!TODO]

>[!EXAMPLE]

## Listen

### Geordnete Liste

```markdown
1. Erster Punkt
2. Zweiter Punkt
   1. Unterpunkt
   2. Unterpunkt
```

### Ungeordnete Liste

```markdown
- Erster Punkt
- Zweiter Punkt
  - Unterpunkt
  - Unterpunkt
```

## Links

- `[Link-Text](https://example.com)` → [Link-Text](https://example.com/)
- Verlinkter Text mit Tooltip: `[Text](https://example.com "Tooltip")`

## Bilder

```markdown
![Alt-Text](Bild-URL "Optionaler Tooltip")
```

## Zitate

```markdown
> Dies ist ein Zitat.
```

## Code

### Inline-Code

```markdown
`Code`
```

### Code-Block

````markdown
```sprache
Dein Code hier
````
## Tabellen
```markdown

| Kopf 1  | Kopf 2  | Kopf 3  |
|---------|---------|---------|
| Wert 1  | Wert 2  | Wert 3  |
| Wert A  | Wert B  | Wert C  |
````

## Mathematische Formeln (MathJax)

### Inline-Formel

```markdown
\( E = mc^2 \)
```

### Block-Formel

```markdown
$$
\int_a^b f(x) \, dx = F(b) - F(a)
$$
```

### Beispiele

- Inline: `\( a^2 + b^2 = c^2 \)` → a2+b2=c2a^2 + b^2 = c^2
- Block:
    
    ```markdown
    $$
    \lim_{x \to \infty} f(x) = L
    $$
    ```
    

## Tiefgestellt und Hochgestellt

### Tiefgestellt

```markdown
H<sub>2</sub>O
```

Ergebnis: H2O

### Hochgestellt

```markdown
x<sup>2</sup>
```

Ergebnis: x2

## Horizontale Linie

```markdown
---
```

## Faltbare Callouts (Obsidian)

```markdown
> [!INFO]+ **Titel**
Inhalt des Callouts hier.
```

## Zusätzliche Tipps

- **HTML funktioniert in Markdown**, z. B.: `<span style="color: red;">Text</span>`
- **Emojis**: `:smile:` → 😄
- **Checkboxen**:

```markdown
- [ ] To-Do
- [x] Erledigt
```