
⚠️ Une boucle permet de **répéter du code** plusieurs fois sans le réécrire. Il existe deux types de boucles en Python.

➡️ `for` — on sait **combien de fois** on veut répéter
➡️ `while` — on répète **tant qu'une condition est vraie**

---

## 1️⃣  La boucle `for`

⚠️ Elle **parcourt** une collection ou une séquence élément par élément
#### 💡 <span style="color: cyan;">Exemple</span>

```python
fruits = ["pomme", "banane", "cerise"]

for fruit in fruits:
    print(fruit)

# → pomme
# → banane
# → cerise
```


⚠️ Chronologie de lecture par Python 
```
tour 1 → fruit = "pomme"   → print("pomme")
tour 2 → fruit = "banane"  → print("banane")
tour 3 → fruit = "cerise"  → print("cerise")
→ plus d'éléments → la boucle s'arrête
```


---

### 📦 La fonction `range()` — boucler un nombre de fois

⚠️ `range()` génère une **séquence de nombres** — très utilisé avec `for`

```python
for i in range(5):
    print(i)

# → 0
# → 1
# → 2
# → 3
# → 4
```


⚠️ Les variantes de `range()`

```python
range(5)        # → 0, 1, 2, 3, 4          (de 0 à 4)
range(2, 6)     # → 2, 3, 4, 5             (de 2 à 5)
range(0, 10, 2) # → 0, 2, 4, 6, 8         (de 0 à 9, par pas de 2)
range(5, 0, -1) # → 5, 4, 3, 2, 1         (compte à rebours)
```


---

### 📦 Boucler avec l'index — `enumerate()`

⚠️ Quand tu veux **l'index ET la valeur** en même temps

```python
fruits = ["pomme", "banane", "cerise"]

for index, fruit in enumerate(fruits):
    print(index, fruit)

# → 0 pomme
# → 1 banane
# → 2 cerise
```


---

### 📦 Boucler sur un dictionnaire

⚠️ Par défaut, `for` parcourt les **clés**

```python
joueur = {"nom": "Sara", "age": 25, "niveau": 3}

for cle in joueur:
    print(cle)
# → nom
# → age
# → niveau
```

⚠️ Pour avoir **clé et valeur** ensemble

```python
for cle, valeur in joueur.items():
    print(cle, "→", valeur)

# → nom → Sara
# → age → 25
# → niveau → 3
```


---

## 2️⃣ La boucle `while`

⚠️ Elle répète un bloc **tant qu'une condition est vraie** — on ne sait pas forcément combien de tours elle va faire

##### 💡 <span style="color: cyan;">Exemple</span>

```python
compteur = 0

while compteur < 5:
    print(compteur)
    compteur += 1      # ⚠️ très important — sans ça, boucle infinie !

# → 0
# → 1
# → 2
# → 3
# → 4
```


---

### 📦 `break` et `continue` — contrôler une boucle

⚠️ `break` — **stoppe** la boucle immédiatement

```python
nombres = [1, 2, 3, 4, 5]

for nombre in nombres:
    if nombre == 3:
        break           # on s'arrête dès qu'on trouve 3
    print(nombre)

# → 1
# → 2
```

⚠️ `continue` — **saute** le tour en cours et passe au suivant

```python
for nombre in range(6):
    if nombre == 3:
        continue        # on saute le 3 et on continue
    print(nombre)

# → 0
# → 1
# → 2
# → 4
# → 5
```


---

### 📦 `for` vs `while` — quand choisir quoi ?

```
Tu sais combien de tours ?         → for
Tu parcours une collection ?       → for
Tu répètes jusqu'à une condition ? → while
Tu attends une action utilisateur ? → while
```


---

### 🔍 RECAP

```
for x in collection:     → parcourt chaque élément
for i in range(n):       → répète n fois
for i, x in enumerate(): → index + valeur
for k, v in dict.items(): → clé + valeur d'un dict

while condition:         → répète tant que vrai

break                    → stoppe la boucle
continue                 → saute le tour en cours

⚠️ toujours les : après for et while
⚠️ toujours indenter le bloc en dessous
⚠️ avec while, toujours modifier la variable pour éviter la boucle infinie
```