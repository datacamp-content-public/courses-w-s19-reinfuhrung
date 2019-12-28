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
Berechnen Sie anschließend die Summe von x und weisen Sie das Ergebnis einem Vektor y zu.

p.s: Führen Sie ggf. die vorherigen Befehle nochmals aus!

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
Erzeugen Sie einen neuen Vektor z, der x und danach y enthält.

p.s: Führen Sie ggf. die vorherigen Befehle nochmals aus!

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

p.s: Führen Sie ggf. die vorherigen Befehle nochmals aus!

`@possible_answers`
- [605]
- 595
- 615

`@hint`


`@sct`
```{r}
msg1 <- "Super, Weiter so!"
msg2 <- "Nope."
msg3 <- "Nein!"
ex() %>% check_mc(1, feedback_msgs = c(msg1, msg2, msg3))
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
xp: 15
```

`@instructions`
Laden Sie den bereits verfügbaren Datensatz ToothGrowth und speichern Sie ihn unter ToothGrowth. Die Daten stammen von einem Experiment zum Wachstum der Zähne (gemessen durch die Länge _len_) bei Meerschweinchen, die eine Dosis _dose_ an Vitamin C in einer von zwei Verabreichungsformen (_supp_) erhalten haben.

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
"well done"
```

***

```yaml
type: NormalExercise
key: 19af2611cd
xp: 15
```

`@instructions`
Berechnen Sie die mittlere Zahnlänge (len) der Meerschweinchen.

`@hint`
mean(dataset$variable)

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
"well done"
```

***

```yaml
type: NormalExercise
key: 05cba0be28
xp: 15
```

`@instructions`
Betrachten Sie alle Meerschweinchen mit einer Zahnlänge von mindestens 20.
Speichern Sie die Beobachtungen als "m" ab.

`@hint`
Dataset[Dataset$variable(Bedingung),]

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
m <- ToothGrowth[ToothGrowth$len>=20,]
```

`@sct`
```{r}
ex() %>% check_object("m") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: c485fb1cae
xp: 15
```

`@instructions`
Berechnen Sie die Standardabweichung für die Zahnlänge (_len_)

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
ex() %>% check_object() %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 843e25104a
xp: 15
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
xp: 15
```

`@instructions`
Berechnen Sie den Mittelwert der Zahnlängen nur für die Gruppe "OJ"!

`@hint`
mean(var[Bedingung]), "OJ" in Anführungszeichen

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

***

```yaml
type: NormalExercise
key: 88f02e6ae6
xp: 10
```

`@instructions`
Lassen Sie sich von R ein einfaches Streudiagramm der Variable _len_ ausgeben

`@hint`
plot()

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
plot(ToothGrowth$len)
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
Legen Sie eine neue Variable y an, in der Sie Folgendes speichern: 
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
Speichern Sie das Ergebnis der folgenden Aufgabe in z. Addieren Sie zu allen durch 9 teilbaren Zahlen in x den Wert 7 und ziehen Sie den Wert 1 von den ungeraden Zahlen in x ab.

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
Betrachten Sie den Datensatz _cars_ und speichern Sie ihn als _cars_ ab.

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
Mit welchem Befehl in R sieht man das am einfachsten?

`@hint`
Es ist str()

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

***

```yaml
type: NormalExercise
key: 27e55ee02b
```

`@instructions`
Bitte lassen Sie sich ein einfaches Streudiagramm von Distanz gegen Speed ausgeben!
D.h., x-Achse _speed_, y-Achse _dist_!

`@hint`
plot(y~x)

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
plot(cars$dist~cars$speed)
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
xp: 15
```

`@instructions`
Betrachten Sie den Datensatz chickwts und speichern Sie ihn auch so ab.

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
xp: 15
```

`@instructions`
Wie viele Beobachtungen und Variablen enthält der Datensatz?

`@hint`
Verwenden Sie str()

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
xp: 15
```

`@instructions`
Extrahieren Sie einen neuen Datensatz, der nur jene Beobachtungen enthält, wo die Hühner mit horsebean oder linseed gefüttert wurden.

`@hint`
Wir brauchen eine Bedingung [], einen Vergleich == und ein Oder |

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
xp: 15
```

`@instructions`
Was ist das minimale, maximale und durchschnittliche Gewicht für alle Beobachtungen?
Mit 3 Befehlen nacheinander bitte, angefangen mit minmial, dann maximal und im Anschluss durchschnittlich!

`@hint`
Befehl(chickwts$weight)

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
xp: 15
```

`@instructions`
Berechnen Sie die Werte _min, max_ und _mean_,wenn nur jene Huehner betrachtet werden, die mit horsebean oder linseed gefuettert wurden.

`@hint`
Befehl(dataset[dataset$var == "horsebean" | dataset$var == "linseed", ]$weight)

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

***

```yaml
type: NormalExercise
key: 5f7e723596
xp: 15
```

`@instructions`
Bitte lassen Sie sich von R ein Balkendiagramm ausgeben, wobei auf der X-Achse die unterschiedlichen Sorten (_feed_) aufgetragen sind und auf der Y-Achse das Gewicht!

`@hint`
boxplot(y ~ x, data = ...)

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
boxplot(weight ~ feed, data = chickwts)
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: NormalExercise
key: d73e70505d
xp: 15
```

`@instructions`
Unterscheiden sich die Feed-Gruppen signifikant voneinander? Berechnen Sie bitte eine ANOVA!

`@hint`
anova(lm(y~x,data = ...))

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
anova(lm(weight ~ feed, data = chickwts))
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

***

```yaml
type: MultipleChoiceExercise
key: 1be020f4d1
xp: -5
```

`@question`
Unterscheiden sich die Gruppen signifikant voneinander?
Laut ANOVA Step 7.

`@possible_answers`
- [Ja]
- Nein

`@hint`


`@sct`
```{r}
msg1 <- "Perfect ;)"
msg2 <- "Nope!? Bitte nochmal genau nachsehen!"
ex() %>% check_mc(1, feedback_msgs = c(msg1, msg2))
```

---

## If , If-else

```yaml
type: NormalExercise
key: a33e66c617
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
x <- -5

Schreiben Sie eine einfache If-Bedingung, sodass R anhand des Wertes in x für eine positive Zahl  "Non-negative number" bzw. für eine negative Zahl "Negative number" ausgibt!

`@hint`
if(...){
print(...)
} else {
print(...)
}

`@pre_exercise_code`
```{r}
x <- -5
```

`@sample_code`
```{r}
x <- -5
```

`@solution`
```{r}
if(x > 0){
print("Non-negative number")
} else {
print("Negative number")
}
```

`@sct`
```{r}
# Examples of good success messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.
```

---

## Show me your Skills!

```yaml
type: NormalExercise
key: 9cf1fc2eb2
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
Die Fibonacci-Folge ist eine unendliche Folge von Zahlen (den Fibonacci-Zahlen), bei der sich die jeweils folgende Zahl durch Addition der beiden vorherigen Zahlen


fn = fn-1 + fn+2

mit den Anfangswerten f0 = 0 und f1 = 1 ergibt. Also, 0; 1; 1; 2; 3; 5; 8; 13; : : :. Schreiben Sie eine for-Schleife, welche in einem Vektor fib die ersten 30 Fibonacci-Zahlen abspeichert.	

Am Ende vom Code bitte die Folge ausgeben lassen. Also print(fib)

`@hint`
for (i in 3:30) { ......}

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
fib <- c(0,1)
```

`@solution`
```{r}
fib <- c(0,1)
for (i in 3:30) { 
  fn <- fib[i-1] + fib[i-2]
  fib <- c(fib, fn)
}
print(fib)

```

`@sct`
```{r}
"Super, alles gut gemeistert!"
```
