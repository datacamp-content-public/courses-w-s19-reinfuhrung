---
title: 'Multiple Choice'
description: Basics
---

## Anwendungsbereich R-Studio

```yaml
type: PureMultipleChoiceExercise
key: 89ee3fdc94
xp: 50
```

In welchen der folgend genannten Fälle ist RStudio eine ideale Anwendung?

`@hint`
Vielleicht solltest du ganz kurz mal die Homepage von R-Studio ansehen

`@possible_answers`
- [Um R-Programme zu schreiben, den Programmablauf zu testen und projektbasiert zu arbeiten.]
- Um die Ausgabe von R-Programmen tabellarisch und graphisch darzustellen.
- Um Graphiken und Tabellen von R-Programmen APA-konform darzustellen.
- Um R-Programme in lauffähige .exe-Dateien umzuwandeln.

`@feedback`
- Nicht schlecht für den Anfang!
- Nein, dafür kann es verwendet werden, aber es ist nicht die ideale Anwendung.
- Kann man machen, aber dafür ist R-Studio nicht gedacht.
- R ist eine Interpreter-Sprache, die Programme müssen daher nicht kompiliert werden.

---

## IDE

```yaml
type: PureMultipleChoiceExercise
key: a983e56487
xp: 50
```

**Wofür steht IDE im Zusammenhang mit RStudio?**

`@hint`
RStudio ist eine IDE Anwendung, mit der R einfacher verwendet werden kann. Es integriert dabei einige hilfreiche Entwicklungsumgebungen in eine Anwendung.

`@possible_answers`
- Intensive Design Environment
- Integrated Document Environment
- Independent Developer Ecosystem
- [Integrated Development Environment]

`@feedback`
- Nope
- Fast
- Nein
- Ja, das ist es!

---

## Kompatible Programme

```yaml
type: PureMultipleChoiceExercise
key: c40bd2c4f0
xp: 50
```

Welche Statistik-Programme lassen sich nicht nur als Alternative zu R verwenden, sondern lassen sich auch in R einbinden?

`@hint`
- Ein Programm lässt sich mit dem Paket _jmv_ in R einbinden.

`@possible_answers`
- [JAMOVI und JASP]
- JPEG und GIF
- Excel und Powerpoint

`@feedback`
- Perfekt!
- Leider nein, bei JPEG geht's um Bilder. 
- Powerpoint ist nicht für Statistik gedacht.

---

## Dezimaltrennzeichen

```yaml
type: PureMultipleChoiceExercise
key: d0eb7a1a43
xp: 50
```

Welches Dezimaltrennzeichen wird in R verwendet?

`@hint`


`@possible_answers`
- Komma
- [Punkt]
- Semikolon
- Klammer

`@feedback`
- Nope
- Super, das ist es!
- Nope
- Nope

---

## Groß- und Kleinschreibung

```yaml
type: PureMultipleChoiceExercise
key: a96c7fe21d
xp: 50
```

In R wird zwischen Groß- und Kleinschreibung unterschieden, richtig oder falsch?

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@possible_answers`
- [richtig]
- falsch

`@feedback`
- Genau, nur weiter so!
- Nein, leider ist die Antwort _falsch_ wirklich falsch

---

## Ausdrücke in R

```yaml
type: PureMultipleChoiceExercise
key: 94f441c570
xp: 50
```

Welche Bedeutung hat in R das folgende Symbol == im Ausdruck 8 * 3 == 6 * 4?

`@hint`


`@possible_answers`
- weist der Variablen _8 * 3_ das Ergebnis der Multiplikation _6 * 4_ zu.
- hat gar keine Bedeutung, da dieser Ausdruck in R gar nicht erlaubt ist.
- [Vergleicht, ob das Ergebnis 8 * 3 gleich 6 * 4 ist und liefert den logischen Wert TRUE als Ergebnis]
- Vergleicht, ob das Ergebnis 8 * 3 gleich 6 * 4 ist und liefert den logischen Wert FALSE als Ergebnis

`@feedback`
- Sorry, total daneben. Vielleicht solltest du das Skript nochmals von vorne zu lesen beginnen.
- Nein, der Ausdruck ist sehr wohl erlaubt.
- Ja, er prüft auf logische Äquivalenz.
- Der Vergleich liefert aber ein anderes Ergebnis, oder?

---

## Small Exercise

```yaml
type: MultipleChoiceExercise
key: 0319dccb8d
xp: 50
```

Berechne den Mittelwert des Vektors **vector1** (der Vektor wurde bereits in den Arbeitsspeicher geladen und ist mit eben diesem Namen verfügbar). Wenn du in der Konsole _vector1_ und _Eingabe_ eingibst, siehst du die Werte, die in diesem Vektor gespeichtert sind.

Verwende die Tab-completion von RStudio sowohl beim Funktionsnamen wie auch innerhalb der Funktion.

`@possible_answers`
- 5.4
- [7.6]
- 10.45
- 12.23

`@hint`
Verwende die Funktion mean() und die Tab-completion-Funktion von R-Studio

`@pre_exercise_code`
```{r}
vector1 <- c(3, 12, 13, 4, 6)
```

`@sct`
```{r}
# Check https://instructor-support.datacamp.com/en/articles/2375523-course-multiple-choice-with-console-exercises on how to write feedback messages for this exercise.
```

---

## Small Exercise II

```yaml
type: NormalExercise
key: a5759445de
xp: 100
```



`@instructions`
Bei dieser Aufgabe geht es darum, die Konsole von R-Studio als einfachen Taschenrechner zu verwenden.

`@hint`
Ergebnis sollte 30 sein, wenn du was anderes heraus bekommst, dann passt was nicht

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
2+28
```

`@sct`
```{r}

```

---

## Konsolenfenster

```yaml
type: PureMultipleChoiceExercise
key: 86ac8a0eb1
xp: 50
```

Wofür wird in R-Studio das Konsolenfenster verwendet?

`@hint`
www.google.at

`@possible_answers`
- [Um direkte R-Befehle abzusenden.]
- Um die R-Dateien zu verwalten.
- Um den Ablauf von R-Programmen zu kontrollieren.
- Um R-Programme zu schreiben und diese in einem Programmfile abzuspeichern.

`@feedback`
- Super!
- Das kann man besser im Dateimanager machen
- Dazu verwendet man den Debugger
- Dazu verwendet man das "Source-Fenster"

---

## Pfeiltasten

```yaml
type: PureMultipleChoiceExercise
key: 0bc971d82e
xp: 50
```

Welche Auswirkung haben die Pfeiltasten (nach oben, nach unten) in der Konsole?

`@hint`


`@possible_answers`
- Bewegen den Cursor in ein anderes Fenster von RStudio.
- Bewirken nichts Spezielles.
- [Blättern durch die bereits eingegebenen Befehle (Historie)]

`@feedback`
- Nein, tun sie nicht.
- Bewirken schon etwas, denk mal nach oder probiers einfach mal aus!
- Ja, die Historie der bereits eingegeben Befehle wird damit durchblättert.

---

## Small Exercise III

```yaml
type: NormalExercise
key: 07a3a95b59
xp: 100
```



`@instructions`
Prüfe in einer Codezeile, ob 3 * 4 gleich 2 * 6 UND 5 * 12 gleich 60 ist.

`@hint`
a == b & c == d

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
3*4 == 2*6 & 5*12 == 60
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

---

## R-Markdown

```yaml
type: PureMultipleChoiceExercise
key: 1b771d7f4a
xp: 50
```

Was ermöglicht R-Markdown?

`@hint`
- R-Markdown ist an HTML angelehnt.

`@possible_answers`
- [Man kann damit Dokumente erstellen, die sowohl R-Code als auch Text enthalten.]
- Es ermöglicht das einfache Erstellen von Bilddateien.
- Es handelt sich um ein Paket zur Notengebung.

`@feedback`
- Richtig. 
- Leider nein. 
- Nein, um "marks" geht es hier nicht :)

---

## Extract Function

```yaml
type: PureMultipleChoiceExercise
key: 230d7c6510
xp: 50
```

Wozu dient die Extract Function?

`@hint`
- Sie ist praktisch für sich wiederholende Aufgaben.

`@possible_answers`
- Damit kann man Variablen aus dem Code wiederverwenden. 
- Damit lässt sich das Speichern von Daten vereinfachen. 
- [Damit lässt sich selbst geschriebener Code in eine Funktion umwandeln.]

`@feedback`
- Nein, darum geht es leider nicht.
- Leider nein.
- Richtig.
