---
title: Coding
description: 'easy examples u should solve without using google or anything else.'
---

## Vektoren

```yaml
type: TabExercise
key: fa3174d1ad
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375525-course-sequential-exercises. -->

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: 435c8eecd9
xp: 25
```

`@instructions`
Erzeugen Sie einen Vektor x, der aus den natürlichen Zahlen von 1 bis 10 besteht!

`@hint`
c(x:y)

`@sample_code`
```{r}

```

`@solution`
```{r}
x <- c(1:10)
```

`@sct`
```{r}

```

***

```yaml
type: NormalExercise
key: 997a713957
xp: 25
```

`@instructions`
Berechnen Sie die anschließend die Summe von x und weisen Sie das Ergebnis einem Vektor y zu.

`@hint`
sum()

`@sample_code`
```{r}
x <- c(1:10)
```

`@solution`
```{r}
y <- sum(1:10)
```

`@sct`
```{r}

```

***

```yaml
type: NormalExercise
key: 522d9b57ce
xp: 25
```

`@instructions`
Erzeugen Sie einen neuen Vektor z der x und danach y enthält.

`@hint`
c(firstVec,secondVec)

`@sample_code`
```{r}
x <- c(1:10)
y <- sum(x)
```

`@solution`
```{r}
z <- c(1:10,sum(1:10))
```

`@sct`
```{r}

```

***

```yaml
type: MultipleChoiceExercise
key: 1d89dfc5eb
xp: 25
```

`@question`
Was ist jetzt die Summe von z?

`@possible_answers`
- [605]
- 595
- 615

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@sct`
```{r}
# Check https://instructor-support.datacamp.com/en/articles/2375523-course-multiple-choice-with-console-exercises on how to write feedback messages for this exercise.
```

---

## ToothGrowth

```yaml
type: TabExercise
key: 367dd3bb12
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375525-course-sequential-exercises. -->

`@pre_exercise_code`
```{r}
ToothGrowth <- ToothGrowth
```

***

```yaml
type: NormalExercise
key: c376f2ec22
xp: 20
```

`@instructions`
Laden Sie den bereits verfügbaren Datensatz mit ToothGrowth <- ToothGrowth. Die Daten stammen von einem Experiment zum Wachstum der Zähne(gemessen durch die Länge len) bei Meerschweinchen, die eine Dosis dose an Vitamin C in einer von zwei Verabreichungsformen (supp) erhalten haben.

`@hint`
name <- dataset

`@sample_code`
```{r}

```

`@solution`
```{r}
ToothGrowth <- ToothGrowth
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 19af2611cd
xp: 20
```

`@instructions`
Berechnen Sie die mittlere Zahnlänge (len) der Meerschweinchen.

`@hint`
mean()

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
mean(ToothGrowth$len)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 05cba0be28
xp: 20
```

`@instructions`
Betrachten Sie alle Meerschweinchen mit einer Zahnlänge von mindestens 20.

`@hint`
Dataset[Dataset$variable(Bedingung),]

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
ToothGrowth[ToothGrowth$len>=20,]
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: c485fb1cae
xp: 20
```

`@instructions`
Berechnen Sie die Standardabweichung für die Zahnlänge (len)

`@hint`
sd()

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
sd(ToothGrowth$len)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 843e25104a
xp: 20
```

`@instructions`
Berechnen Sie den Korrelationskoeffizienten zwischen Dosis und Zahnlänge.

`@hint`
cor(x,y)

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
cor(ToothGrowth$dose,ToothGrowth$len)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 5b0c2d5843
```

`@instructions`
Berechnen Sie den Mittelwert der Zahnlängen nur für die Gruppe "OJ"!

`@hint`
mean(var[Bedingung])

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
mean(ToothGrowth$len[ToothGrowth$supp == "OJ"])
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```
