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

Es geht hier um Berechnungen mit Vektoren.

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
ex() %>% check_object("x") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 997a713957
xp: 25
```

`@instructions`
Berechnen Sie anschließend die Summe der Zahlen von 1 bis 10 und weisen Sie das Ergebnis einem Vektor y zu.

P.S.: Führen Sie ggf. die vorherigen Befehle nochmals aus!

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
ex() %>% check_object("y") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 522d9b57ce
xp: 25
```

`@instructions`
Erzeugen Sie einen neuen Vektor z, der x und danach y enthält.
Geben Sie die Vektoren als 1:10 und sum(1:10) an!

`@hint`
Es ist **nicht** c(x&y) gemeint, sondern verwenden Sie bitte die in der Instruktion angegebene Form. Dann: c(firstVec,secondVec)

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
ex() %>% check_object("z") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: MultipleChoiceExercise
key: 1d89dfc5eb
xp: 25
```

`@question`
Was ist jetzt die Summe von z?

P.S.: Führen Sie ggf. die vorherigen Befehle nochmals aus!

`@possible_answers`
- [110]
- 95
- 105

`@hint`


`@sct`
```{r}
msg1 <- "Super, weiter so!"
msg2 <- "Leider falsch."
msg3 <- "Leider falsch."
ex() %>% check_mc(1, feedback_msgs = c(msg1, msg2, msg3))
```

---

## ToothGrowth

```yaml
type: TabExercise
key: 367dd3bb12
xp: 100
```

Die Daten dieser Übung stammen von einem Experiment zum Wachstum der Zähne (gemessen durch die Länge _len_) bei Meerschweinchen, die eine Dosis _dose_ an Vitamin C in einer von zwei Verabreichungsformen (_supp_) erhalten haben.

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
Laden Sie den bereits verfügbaren Datensatz _ToothGrowth_ und speichern Sie ihn in der Variable _ToothGrowth_.

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
Berechnen Sie die mittlere Zahnlänge (_len_) der Meerschweinchen und speichern Sie die Lösung bitte in der Variable _m_.

`@hint`
mean(dataset$variable)

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
m <- mean(ToothGrowth$len)
```

`@sct`
```{r}
ex() %>% check_object("m") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 05cba0be28
xp: 15
```

`@instructions`
Betrachten Sie alle Meerschweinchen mit einer Zahnlänge von mindestens 20.
Speichern Sie die Beobachtungen als _m_ ab.

`@hint`
Dataset[Dataset$variableBedingung,]

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
Berechnen Sie die Standardabweichung für die Zahnlänge (_len_) und speichern Sie die Lösung bitte in der Variable _sa_.

`@hint`
sd()

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
sa <- sd(ToothGrowth$len)
```

`@sct`
```{r}
ex() %>% check_object("sa") %>% check_equal()
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
Legen Sie die Lösung bitte als Variable _corr_ an.

`@hint`
cor(x,y)

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
corr <- cor(ToothGrowth$dose,ToothGrowth$len)
```

`@sct`
```{r}
ex() %>% check_object("corr") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 5b0c2d5843
xp: 15
```

`@instructions`
Berechnen Sie den Mittelwert der Zahnlängen nur für die Gruppe "OJ"! Speichern Sie das Ergebnis als Variable _oj_!

`@hint`
mean(var[Bedingung]), "OJ" in Anführungszeichen

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
oj <- mean(ToothGrowth$len[ToothGrowth$supp == "OJ"])
```

`@sct`
```{r}
ex() %>% check_object("oj") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 88f02e6ae6
xp: 10
```

`@instructions`
Lassen Sie sich von R ein einfaches Streudiagramm der Variable _len_ ausgeben.
Speichern Sie den Befehl bitte als _plotlen_!

`@hint`
plot()

`@sample_code`
```{r}
ToothGrowth <- ToothGrowth
```

`@solution`
```{r}
plotlen <- plot(ToothGrowth$len)
```

`@sct`
```{r}
ex() %>% check_object("plotlen") %>% check_equal()
success_msg("Well done!")
```

---

## Vektoren again

```yaml
type: TabExercise
key: 4766f57a23
xp: 100
```

Diese Aufgabe erfolgt wieder mit Vektoren.

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
Erzeugen Sie einen Vektor x, der die Zahlen von 1 bis 100 enthält.

`@hint`
Das haben Sie in einer früheren Übung schon gemacht. Vektoren erzeugt man mit _c()_.

`@sample_code`
```{r}

```

`@solution`
```{r}
x <- c(1:100)
```

`@sct`
```{r}
ex() %>% check_object("x") %>% check_equal()
success_msg("Well done!")
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
ex() %>% check_object("y") %>% check_equal()
success_msg("Well done!")
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
c(((x[Bedingung])+7),((x[Bedingung])-1)); _ungerade_ lässt sich als _x%%2==1_ ausdrücken

`@sample_code`
```{r}
x <- c(1:100)
```

`@solution`
```{r}
x <- c(1:100)
z <- c((x[x%%9==0])+7,(x[x%%2==1])-1)
```

`@sct`
```{r}
ex() %>% check_object("z") %>% check_equal()
success_msg("Well done!")
```

---

## Cars

```yaml
type: TabExercise
key: 57ba32e6f6
xp: 100
```

Im Datensatz _cars_ finden Sie Angaben zu verschiedenen Autos.

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
ex() %>% check_object("cars") %>% check_equal()
success_msg("Well done!")
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
Es ist _str()_

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
Geben Sie die 3., 10. und 12. Beobachtung aus und speichern Sie diese in die Variable x!

`@hint`
dataset[c(.,.,.),]

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
cars <- cars
x <- cars[c(3,10,12),]
```

`@sct`
```{r}
ex() %>% check_object("x") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 9867c3f436
xp: 20
```

`@instructions`
Extrahieren Sie die zweite Variable und speichern Sie diese in der Variable _two_!

`@hint`
dataset[,2]

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
two <- cars[,2]
```

`@sct`
```{r}
ex() %>% check_object("two") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 4e706c2c5c
xp: 20
```

`@instructions`
Extrahieren Sie die Variable _dist_ für die ersten 3 Beobachtungen und speichern Sie diese in der Variable _firstthree_!

`@hint`
dataset$var[x:y]

`@sample_code`
```{r}
cars <- cars
```

`@solution`
```{r}
firstthree <- cars$dist[1:3]
```

`@sct`
```{r}
ex() %>% check_object("firstthree") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 27e55ee02b
```

`@instructions`
Bitte lassen Sie sich ein einfaches Streudiagramm von Distanz gegen Speed ausgeben!
D.h., auf der x-Achse soll _speed_, auf der y-Achse _dist_ abgetragen werden!

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

Der hier verwendete Datensatz enthält Futter- und Gewichtsdaten von Hühnern.

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
Betrachten Sie den Datensatz _chickwts_ und speichern Sie ihn als _chickw_ ab!

`@hint`


`@sample_code`
```{r}

```

`@solution`
```{r}
chickw <- chickwts
```

`@sct`
```{r}
ex() %>% check_object("chickw") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 11a12d6a03
xp: 15
```

`@instructions`
Wie viele Beobachtungen und Variablen enthält der Datensatz? Speichern Sie die Antwort als _ch_ ab!

`@hint`
Verwenden Sie _str()_

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
ch <- str(chickwts)
```

`@sct`
```{r}
ex() %>% check_object("ch") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 92db60f74f
xp: 15
```

`@instructions`
Extrahieren Sie einen neuen Datensatz, der nur jene Beobachtungen enthält, wo die Hühner mit horsebean oder linseed gefüttert wurden.
Speichern Sie diesen Datensatz unter dem Namen _sol_!

`@hint`
Wir brauchen eine Bedingung [], einen Vergleich == und ein Oder |
Tipp: Beistrich am Ende nicht vergessen!

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
sol <- chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]
```

`@sct`
```{r}
ex() %>% check_object("sol") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: da85b204f4
xp: 15
```

`@instructions`
Was ist das minimale, maximale und durchschnittliche Gewicht für alle Beobachtungen?
Bitte bearbeiten Sie diese Aufgabe mit 3 Befehlen nacheinander, angefangen mit minimal, dann maximal und im Anschluss durchschnittlich!

Speichern Sie die Ergebnisse in _mi,ma_ und _mea_!

`@hint`
Befehl(chickwts$weight)

`@sample_code`
```{r}
chickwts <- chickwts
```

`@solution`
```{r}
mi <- min(chickwts$weight)
ma <- max(chickwts$weight)
mea <- mean(chickwts$weight)
```

`@sct`
```{r}
ex() %>% check_object("mi","ma","mea") %>% check_equal()
success_msg("Well done!")
```

***

```yaml
type: NormalExercise
key: 1b91385a8e
xp: 15
```

`@instructions`
Berechnen Sie die Gewichts-Werte _min, max_ und _mean_, wenn nur jene Hühner betrachtet werden, die mit horsebean oder linseed gefüttert wurden.

Speichern Sie diese in _mihl, mahl_ und _meahl_!

`@hint`
Befehl(dataset[dataset$var == "horsebean" | dataset$var == "linseed", ]$weight)

`@sample_code`
```{r}
chickwts <- chickwts

```

`@solution`
```{r}
mihl <- min(chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]$weight)
mahl <- max(chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]$weight)
meahl <- mean(chickwts[chickwts$feed == "horsebean" | chickwts$feed == "linseed", ]$weight)
```

`@sct`
```{r}
ex() %>% check_object("mihl","mahl","meahl") %>% check_equal()
success_msg("Well done!")
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

`@possible_answers`
- [Ja]
- Nein

`@hint`
Sehen Sie sich das Ergebnis von _PR_ an!

`@sct`
```{r}
msg1 <- "Perfekt"
msg2 <- "Das stimmt leider nicht. Bitte noch einmal genau nachsehen!"
ex() %>% check_mc(1, feedback_msgs = c(msg1, msg2))
```

---

## If , If-else

```yaml
type: NormalExercise
key: a33e66c617
xp: 100
```

Bei dieser Übung arbeiten Sie mit Bedingungen (if).

`@instructions`
x <- -5

Schreiben Sie eine einfache If-Bedingung, sodass R anhand des Wertes in x für eine positive Zahl den Text "Non-negative number" bzw. für eine negative Zahl "Negative number" ausgibt!

Weiter soll in dieser Bedingung, sobald eine negative Zahl gefunden wurde, ein Vektor y mit dem Wert 0 angelegt werden, sowie bei nicht-negativen Zahlen ein Vektor y mit dem Wert 1!

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
  y <- 1
} else {
print("Negative number")
  y <- 0
}





```

`@sct`
```{r}
ex() %>% check_object("y") %>% check_equal()
success_msg("Well done!")
```

---

## Show me your Skills!

```yaml
type: NormalExercise
key: 9cf1fc2eb2
xp: 100
```

Die Fibonacci-Folge ist eine unendliche Folge von Zahlen (den Fibonacci-Zahlen), bei der sich die jeweils folgende Zahl durch Addition der beiden vorherigen Zahlen

fn = fn-1 + fn+2

mit den Anfangswerten f0 = 0 und f1 = 1 ergibt. Also, 0; 1; 1; 2; 3; 5; 8; 13; : : :. 

`@instructions`
Schreiben Sie eine for-Schleife, welche in einem Vektor _fib_ die ersten 30 Fibonacci-Zahlen abspeichert.	

Am Ende vom Code bitte die Folge ausgeben lassen. Also _print(fib)_.

Bitte am Ende dann die Summe der Fibonacci-Folge von 1:30 als Variable y abspeichern!

`@hint`
for (i in 3:30) { ......}

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
fib <- c(0,1)
for (i in 3:30) { 
  fn <- fib[i-1] + fib[i-2]
  fib <- c(fib, fn)
}
print(fib)
y <- sum(fib)

```

`@sct`
```{r}
ex() %>% check_object("y") %>% check_equal()
success_msg("Super, alles gut gemeistert!")


```
