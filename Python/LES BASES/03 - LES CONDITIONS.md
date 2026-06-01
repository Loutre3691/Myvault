
⚠️ Une condition permet d'**exécuter du code uniquement si quelque chose est vrai**. Python évalue une expression et choisit quel bloc exécuter.

➡️ Le bloc exécuté est **indenté** (décalé de 4 espaces) — c'est obligatoire en Python !
➡️ Python lit les conditions **dans l'ordre** et s'arrête à la première vraie
➡️ `else` est le **cas par défaut** — il s'exécute si aucune condition n'est vraie

#### 💡 <span style="color: cyan;">Exemple</span>
 
```python
age = 20

if age >= 18:
    print("Tu es majeur")   # ✅ cette ligne s'exécute
else:
    print("Tu es mineur")   # ignorée
```

---

### 📦 Structure complète — if / elif / else

⚠️ `elif` = "sinon si" — permet de tester **plusieurs conditions à la suite**

```python
note = 14

if note >= 16:
    print("Très bien")
elif note >= 12:
    print("Bien")        # ✅ cette ligne s'exécute
elif note >= 10:
    print("Passable")
else:
    print("Insuffisant")
```


⚠️ Chronologie de lecture par Python 
```
1. note >= 16 ?  → 14 >= 16 ? Non  → on passe
2. note >= 12 ?  → 14 >= 12 ? Oui  → on exécute "Bien" et on STOP
```


---

### 📦 Les opérateurs de comparaison

⚠️ Ce sont eux qui créent les conditions — ils retournent toujours `True` ou `False`

```python
10 == 10    # → True   égal à
10 != 5     # → True   différent de
10 > 5      # → True   supérieur à
10 < 5      # → False  inférieur à
10 >= 10    # → True   supérieur ou égal à
10 <= 9     # → False  inférieur ou égal à
```


---

### 📦 Combiner des conditions — and / or / not

⚠️ `and` — les deux conditions doivent être vraies
```python
age = 20
argent = 50

if age >= 18 and argent >= 10:
    print("Tu peux entrer")    # ✅ les deux sont vrais
```

⚠️ `or` — au moins une condition doit être vraie
```python
jour = "samedi"

if jour == "samedi" or jour == "dimanche":
    print("C'est le week-end !")   # ✅ samedi est vrai
```

⚠️ `not` — inverse la condition
```python
connecte = False

if not connecte:
    print("Merci de te connecter")   # ✅ not False = True
```


---

### 📦 Condition sur une liste / set / dict

⚠️ On peut tester si une valeur est dans une collection avec `in`

```python
fruits = ["pomme", "banane", "cerise"]

if "banane" in fruits:
    print("La banane est dans la liste")   # ✅

joueur = {"nom": "Sara", "niveau": 3}

if "niveau" in joueur:
    print("La clé niveau existe")          # ✅
```


---

### 📦 La condition ternaire — version courte

⚠️ Une condition sur **une seule ligne** — utile pour les cas simples

```python
# syntaxe : valeur_si_vrai  if  condition  else  valeur_si_faux

age = 20
statut = "majeur" if age >= 18 else "mineur"
print(statut)   # → majeur
```

---

### 🔍 RECAP

```
if condition:          → si la condition est vraie
elif condition:        → sinon si (autant de elif que nécessaire)
else:                  → sinon (cas par défaut)

==    égal à
!=    différent de
>     supérieur à
<     inférieur à
>=    supérieur ou égal à
<=    inférieur ou égal à

and   les deux conditions vraies
or    au moins une condition vraie
not   inverse la condition

x in collection     → True si x est dans la collection
```