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
Vielleicht sollten Sie kurz die Homepage von RStudio ansehen.

`@possible_answers`
- [Um R-Programme zu schreiben, den Programmablauf zu testen und projektbasiert zu arbeiten.]
- Um die Ausgabe von R-Programmen tabellarisch und graphisch darzustellen.
- Um Graphiken und Tabellen von R-Programmen APA-konform darzustellen.
- Um R-Programme in lauffähige .exe-Dateien umzuwandeln.

`@feedback`
- Nicht schlecht für den Anfang!
- Nein, dafür kann es verwendet werden, aber es ist nicht die ideale Anwendung.
- Kann man machen, aber dafür ist RStudio nicht gedacht.
- R ist eine Interpreter-Sprache, die Programme müssen daher nicht kompiliert werden.

---

## IDE

```yaml
type: PureMultipleChoiceExercise
key: a983e56487
xp: 50
```

Wofür steht _IDE_ im Zusammenhang mit RStudio?

`@hint`
RStudio ist eine IDE-Anwendung, mit der R einfacher verwendet werden kann. Es integriert dabei einige hilfreiche Entwicklungsumgebungen in eine Anwendung.

`@possible_answers`
- Intensive Design Environment
- Integrated Document Environment
- Independent Developer Ecosystem
- [Integrated Development Environment]

`@feedback`
- Nein
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
- Nein
- Super, das ist es!
- Nein
- Nein

---

## Groß- und Kleinschreibung

```yaml
type: PureMultipleChoiceExercise
key: a96c7fe21d
xp: 50
```

In R wird zwischen Groß- und Kleinschreibung unterschieden, richtig oder falsch?

`@hint`


`@possible_answers`
- [richtig]
- falsch

`@feedback`
- Genau, nur weiter so!
- Nein, leider ist die Antwort _falsch_ wirklich falsch.

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
- [vergleicht, ob das Ergebnis 8 * 3 gleich 6 * 4 ist und liefert den logischen Wert TRUE als Ergebnis]
- vergleicht, ob das Ergebnis 8 * 3 gleich 6 * 4 ist und liefert den logischen Wert FALSE als Ergebnis

`@feedback`
- Das stimmt leider nicht.
- Doch, der Ausdruck ist sehr wohl erlaubt.
- Ja, das Symbol prüft auf logische Äquivalenz.
- Es handelt sich um einen Vergleich, aber mit anderem Ergebnis.

---

## Small Exercise

```yaml
type: MultipleChoiceExercise
key: 0319dccb8d
xp: 50
```

Berechnen Sie den Mittelwert des Vektors **vector1** (der Vektor wurde bereits in den Arbeitsspeicher geladen und ist mit eben diesem Namen verfügbar). Wenn Sie in der Konsole _vector1_ und _Eingabe_ eingeben, sehen Sie die Werte, die in diesem Vektor gespeichtert sind.

Verwenden Sie die Tab-completion von RStudio sowohl beim Funktionsnamen wie auch innerhalb der Funktion.

`@possible_answers`
- 5.4
- [7.6]
- 10.45
- 12.23

`@hint`
Verwenden Sie die Funktion _mean()_ und die Tab-completion-Funktion von RStudio

`@pre_exercise_code`
```{r}
vector1 <- c(3, 12, 13, 4, 6)
```

`@sct`
```{r}
msg1 <- "Leider falsch."
msg2 <- "Super, weiter so!"
msg3 <- "Leider falsch."
msg4 <- "Leider falsch."
ex() %>% check_mc(1, feedback_msgs = c(msg1, msg2, msg3, msg4))
```

---

## Small Exercise II

```yaml
type: NormalExercise
key: a5759445de
xp: 100
```

Bei dieser Aufgabe geht es darum, die Konsole von RStudio als einfachen Taschenrechner zu verwenden.

`@instructions`
Berechnen Sie die Summe aus 2 und 28.

`@hint`
Das Ergebnis sollte 30 sein, wenn etwas anderes herauskommt, dann passt etwas nicht. Haben Sie auf _Run Code_ und _Submit Answer_ gedrückt?

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

Wofür wird in RStudio das Konsolenfenster verwendet?

`@hint`
www.google.at

`@possible_answers`
- [Um direkte R-Befehle abzusenden.]
- Um die R-Dateien zu verwalten.
- Um den Ablauf von R-Programmen zu kontrollieren.
- Um R-Programme zu schreiben und diese in einem Programmfile abzuspeichern.

`@feedback`
- Super!
- Das kann man besser im Dateimanager machen.
- Dazu verwendet man den Debugger.
- Dazu verwendet man das Source-Fenster.

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
- Sie bewegen den Cursor in ein anderes Fenster von RStudio.
- Sie bewirken nichts Spezielles.
- [Sie blättern durch die bereits eingegebenen Befehle (Historie)]

`@feedback`
- Nein, das tun sie nicht.
- Sie bewirken schon etwas - probieren Sie es einfach mal aus!
- Ja, die Historie der bereits eingegeben Befehle wird damit durchblättert.

---

## Small Exercise III

```yaml
type: NormalExercise
key: 07a3a95b59
xp: 100
```

Rechnen und vergleichen.

`@instructions`
Prüfen Sie in einer Codezeile, ob 3 * 4 gleich 2 * 6 UND 5 * 12 gleich 60 ist.

`@hint`
Zuerst die ersten beiden Produkte vergleichen, dann Und-Zeichen, dann die beiden anderen Zahlen vergleichen

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

Wozu dient die Extract-Function?

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
