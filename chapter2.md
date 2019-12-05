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

---

## Vektoren again

```yaml
type: TabExercise
key: 4766f57a23
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375525-course-sequential-exercises. -->

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: b5f5e76442
xp: 35
```

`@instructions`
Erzeugen Sie einen Vektor x, der die Zahlen von 1 bis 100 enthält

`@hint`
Sollten Sie mittlerweile schon wissen ;)

`@sample_code`
```{r}

```

`@solution`
```{r}
x <- c(1:100)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 48f2446fd1
xp: 35
```

`@instructions`
Legen Sie eine neue Variable y an in der Sie Folgendes speichern: 
Dividieren Sie alle in x enthaltenen Vielfachen von 6 durch 3.

`@hint`
x%%6==0

`@sample_code`
```{r}
x <- c(1:100)
```

`@solution`
```{r}
x <- c(1:100)
y <- (x[x%%6==0])/3
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: c363c8c5b7
xp: 30
```

`@instructions`
Speichern Sie in z -> Addieren Sie zu allen durch 9 teilbaren Zahlen in x den Wert 7 und ziehen Sie den Wert 1 von den ungeraden
ab.

`@hint`
c(((x[x%%Bedingung])+7),((x[x%%Bedingung])-1))

`@sample_code`
```{r}
x <- c(1:100)
```

`@solution`
```{r}
x <- c(1:100)
z<- c((x[x%%9==0])+7,(x[x%%2==1])-1)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

---

## Cars

```yaml
type: TabExercise
key: 57ba32e6f6
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375525-course-sequential-exercises. -->

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: a4afb6dddf
xp: 20
```

`@instructions`
Betrachten Sie den Datensatz cars und speichern Sie ihn als cars ab.

`@hint`
var <- dataset

`@sample_code`
```{r}

```

`@solution`
```{r}
cars <- cars
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 413263920e
xp: 20
```

`@instructions`
Wie viele Beobachtungen und Variablen enthält der Datensatz?
Mit welchem Befehl in R sieht man das am Einfachsten?

`@hint`
Es ist nicht view(),head()!

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
str(cars)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: a259c8f3cc
xp: 20
```

`@instructions`
Geben Sie die 3., 10. und 12. Beobachtung aus.

`@hint`
name[c(.,.,.),]

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
cars <- cars
cars[c(3,10,12),]
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 9867c3f436
xp: 20
```

`@instructions`
Extrahieren Sie die zweite Variable.

`@hint`
dataset[,2]

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
cars[,2]
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 4e706c2c5c
xp: 20
```

`@instructions`
Extrahieren Sie die Variable dist fuer die ersten 3 Beobachtungen.

`@hint`
dataset$var[x:y]

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
cars$dist[1:3]
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

---

## chickwts

```yaml
type: TabExercise
key: 486e9fe2e3
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375525-course-sequential-exercises. -->

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: 4f837cc9b7
xp: 20
```

`@instructions`
Betrachten Sie den Datensatz chickwts und speichern sie Ihn auch so ab.

`@hint`
Schaffst du auch so ;)

`@sample_code`
```{r}

```

`@solution`
```{r}
chickwts <- chickwts
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 11a12d6a03
xp: 20
```

`@instructions`
Wie viele Beobachtungen und Variablen enthält der Datensatz?

`@hint`
Weißt du doch schon ;)

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
str(chickwts)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 92db60f74f
xp: 20
```

`@instructions`
Extrahieren Sie einen neuen Datensatz, der nur jene Beobachtungen enthält, wo die Hühner mit horsebean oder linseed gefüttert wurden.

`@hint`
google wird dir helfen :p

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: da85b204f4
xp: 20
```

`@instructions`
Was ist das minimale, maximale und durchschnittliche Gewicht für alle Beobachtungen?
Mit 3 Befehlen nacheinander bitte, angefangen mit minmial, dann maximal und im Anschluss durchschnittlich!

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
min(chickwts$weight)
max(chickwts$weight)
mean(chickwts$weight)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: 1b91385a8e
xp: 20
```

`@instructions`
Wie sind diese Werte,wenn nur jene Huehner betrachtet werden, die mit horsebean oder linseed gefuettert wurden.

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@sample_code`
```{r}
chickwts <- chickwts

```

`@solution`
```{r}
min(chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]$weight)
max(chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]$weight)
mean(chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]$weight)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```
