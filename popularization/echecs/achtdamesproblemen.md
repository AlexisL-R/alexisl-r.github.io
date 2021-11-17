# 8 Dames en één (bijzonder) schaakbord

In deze problemen zal je de vele facetten van het schaakbord kunnen ontdekken. Je moet niet weten schaken om ervan te kunnen genieten, maar je moet wel weten hoe je de schaakstukken moet zetten. In schaak wordt de koningin "dame" genoemd.

![mouv_toren_dames.png](attachment:mouv_toren_dames.png)

## Probleem 1: 8-koninginnenprobleem en meer

### a) Het klassieke 8-koninginnenprobleem
Hoeveel manieren zijn er om 8 dames op een 8×8
schaakbord te zetten zodat geen enkele dame een andere dame aanvalt?

### b) Symmetrie van de 8
Hoeveel oplossingen zijn er op symmetrie na?

### c) Veralgemening voor kleine $n$
Vind alle oplossingen voor alle $n\times n$ schaakborden voor $n\leq 10$.

### d)  Grotere $n$
Vind één oplossing voor een $29\times 29$ schaakbord

### e) Grote $n$
Vind één oplossing voor een $14\times 14$ schaakbord.


```python
### De oplossing van Gauss in SageMath/Python voor een n×n schaakbord
n=8 
de_Permutaties = Permutations(n) 
sol = []
#Diagonalen
for perm in de_Permutaties:
    if n == len(set(perm[i]+i for i in range(n))) and n == len(set(perm[i]-i for i in range(n))):
        sol.append(perm)

print(len(sol))


```

## Probleem 2: een torus schaakbord

![diag_tore_dame.PNG](attachment:diag_tore_dame.PNG)

### a) 8 dames op een Torus
Hoeveel manieren zijn er om 8 dames op een $8\times 8$ torusschaakbord te zetten zodat geen enkele dame een andere dame aanvalt?

### b) Kleinere tori
Geef het aantal oplossingen voor elk $n\times n$ torusschaakbord voor $n<8$.

### c) Voldoende voorwaarde
Voor welke $n$ is er ten minste één oplossing? Geef zo'n positie. 

### d) Nodige voorwaarde
Zijn er $n$ waarvoor er géén oplossing is? 


```python
### De oplossing van Gauss-Pólya in SageMath/Python voor een n×n schaakbord
n=8 
de_Permutaties = Permutations(n) 
sol = []
#Diagonalen
for perm in de_Permutaties:
    if n == len(set(mod(perm[i]+i, n) for i in range(n))) and n == len(set(mod(perm[i]-i,n) for i in range(n))):
        sol.append(perm)

print(len(sol))
```

    28


## Probleem 3: Dominantie
Een dominantie koninginnenprobleem vraagt het minimum aantal dames dat nodig is om een schaakbord volledig te beschermen met dames. (Het is wel een NP-moelijke probleem.)

### a) Koninginnen op een gewoon schaakbord
Wat is het dominantienummer van het $8\times 8$ schaakbord? Geef een voorbeeld.


### b) Niet-aanvallende Koninginnen op een gewoon schaakbord
Wat is het dominantienummer van het $8\times 8$ schaakbord voor niet aanvallende dames? Geef een voorbeeld

### c) Grenzen
Geef je beste boven- en ondergrenzen voor het dominantieprobleem voor het $n\times n$ dominantienummer. (Waarschuwing, het is een open probleem om sherpe grenzen te vinden.)

## Probleem 4: Schaakkunstgalerieën
Een kunstgalerieprobleem vraagt het minimum aantal bewakers dat nodig is om een galerie gemaakt van polyomino, dus samenhangende velden (zoals een schaakbord in 2D of tetrisstukken) te beschermen. Een schaakkunstgalerieprobleem heeft schaakstukken als bewakers. Bijvoorbeeld op een $n\times n$ zijn er altijd $n$ torenbewakers nodig.

Zij $N$ het aantal velden in het schaakkunstgalerieprobleem. 

### a) Torenbewakers bovengrens
Geef een bovengrens in functie van $N$ met torens als bewakers. 

### b) Torenbewaker supremum
Geen de kleinste bovengrens voor het schaakkunstgalerieprobleem met torens als bewakers en bouw een voorbeeld voor elke $N$.

### c) Damesbewakers bovengrens
Geef een bovengrens in functie van $N$  met dames als bewakers. 

### d) Damesbewaker supremum

Geen de kleinste bovengrens voor het schaakkunstgalerieprobleem met dames als bewakers en bouw een voorbeeld voor elke $N$.

### Het is een 3D wereld

Zijn de resultaten hierboven geldig voor 3D polyominos?

### f) Dimensie $d$

Zijn de resultaten hierboven geldig in dimensie $d\geq 2$?

## Probleem 5: Springende Paarden en varia
Paarden, het meest geliefde stuk van het spel kunnen springen over andere stukken. Twee in een richting en dan links of rechts.

![Paarden.png](attachment:Paarden.png)

### a) Een klassiek schaak-domino probleem

Stel dat twee tegenover tegenoverstaande uiterste hoeken van het schaakbord weggehaald zijn. Kan je het resterende bord met $2\times 1$ domino's betegelen?

### b) Guarini's probleem

Verwissel de witte met de zwarte paarden in dit $3\times 3$ schaakbord

![guriani.png](attachment:guriani.png)

### c) Graaf

Geef de graaf van Guarini's probleem. 

### d) Mega Guarini

Verwissel de witte met de zwarte paarden in dit $3\times 4$ schaakbord

![megapaarden.png](attachment:megapaarden.png)

### e) Torentour
Bezoek elke velden van een schaakbord met een toren slechts een keer een kom terug naar de initiële positie.

### f) De stelling van Gomory

Bewijs de stelling van Gomory: als je een wit veld en een zwart veld van het $8\times 8$ schaakbord verwijdert, kan je het met $2\times 1$ domino's betegelen. 

### g) Paardentour

Een paardentour gebeurt als een paard alle velden van het bord bezoekt. Hij is gesloten als het paard teruggaat naar zijn initiële positie en open indien niet.

Vind een paardentour voor een $8\times 8$ schaakbord.

### h) Onmogelijke paardentouren

Bewijs dat de $3\times 4$ en $4\times 4$ schaakborden geen paardentour hebben. Is er een $n$ waarvoor een $4\times n$ schaakbord wél een paardentour heeft?

### i) Algoritmen van Schwenk

Vind een algoritme om op een $n\times m$ schaakbord een paardentour te maken, indien mogelijk. Geef dan alle borden waarvoor het mogelijk is. 


```python

```


```python

```


```python

```


```python

```


```python

```
