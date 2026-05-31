
⚠️ Au lieu d'un index numérique, chaque valeur a une **clé** que tu choisis toi-même. Il s'écrit avec des **accolades** `{ }`

➡️ Chaque élément est une paire **clé : valeur**
➡️ Les clés sont **uniques** — on ne peut pas avoir deux fois la même clé
➡️ Les valeurs peuvent être **n'importe quel type** (str, int, list, tuple, dict...)

#### 💡 <span style="color: cyan;">Exemple</span>

```python
joueur = {
    "nom": "Sara",
    "age": 25,
    "niveau": 3,
    "actif": True
}
```

C'est comme une **fiche d'identité** — chaque info a son étiquette.

---

### 📦 Accéder à une valeur

⚠️ On accède à une valeur via sa **clé**, pas son index

```python
joueur = {"nom": "Sara", "age": 25, "niveau": 3}

print(joueur["nom"])      # → Sara
print(joueur["niveau"])   # → 3
```


⚠️ Si la clé n'existe pas, Python lève une erreur — utilise `.get()` pour éviter ça

```python
print(joueur["ville"])           # ❌ ERREUR ! KeyError
print(joueur.get("ville"))       # ✅ → None  (pas d'erreur)
print(joueur.get("ville", "inconnue"))  # ✅ → inconnue  (valeur par défaut)
```

---

### 📦 Modifier un dictionnaire

⚠️ Modifier une valeur existante
```python
joueur["niveau"] = 5
print(joueur)   # → {"nom": "Sara", "age": 25, "niveau": 5}
```

⚠️ Ajouter une nouvelle paire clé/valeur
```python
joueur["ville"] = "Paris"
print(joueur)   # → {"nom": "Sara", "age": 25, "niveau": 5, "ville": "Paris"}
```

⚠️ Supprimer une clé
```python
del joueur["ville"]
print(joueur)   # → {"nom": "Sara", "age": 25, "niveau": 5}

joueur.pop("niveau")
print(joueur)   # → {"nom": "Sara", "age": 25}
```

⚠️ Vider un dictionnaire
```python
joueur.clear()
print(joueur)   # → {}
```

---

### 📦 Explorer un dictionnaire

⚠️ Voir toutes les clés
```python
joueur = {"nom": "Sara", "age": 25, "niveau": 3}

print(joueur.keys())    # → dict_keys(["nom", "age", "niveau"])
```

⚠️ Voir toutes les valeurs
```python
print(joueur.values())  # → dict_values(["Sara", 25, 3])
```

⚠️ Voir les paires clé/valeur ensemble
```python
print(joueur.items())   # → dict_items([("nom", "Sara"), ("age", 25), ("niveau", 3)])
```

⚠️ Est-ce qu'une clé existe ?
```python
print("nom" in joueur)      # → True
print("ville" in joueur)    # → False
```

⚠️ Combien de paires ?
```python
print(len(joueur))          # → 3
```

---

### 📦 Dictionnaire imbriqué

⚠️ Un dictionnaire peut contenir **d'autres dictionnaires** — très utilisé pour structurer des données complexes

#### 💡 <span style="color: cyan;">Exemple</span>

```python
equipe = {
    "joueur1": {"nom": "Sara", "niveau": 5},
    "joueur2": {"nom": "Lena", "niveau": 3},
}

print(equipe["joueur1"])            # → {"nom": "Sara", "niveau": 5}
print(equipe["joueur1"]["nom"])     # → Sara
print(equipe["joueur2"]["niveau"])  # → 3
```

---

#### 📦 Dict vs List vs Tuple — le tableau comparatif

⚠️ La règle simple pour choisir :

```
Tu veux...                                → Utilise

Une liste ordonnée et modifiable          → list   [1, 2, 3]
Des données fixes qui ne changent pas     → tuple  (1, 2, 3)
Des données avec des étiquettes           → dict   {"clé": valeur}
```

---

### 🔍 RECAP

```
.get(clé)              → retourne la valeur, None si inexistante
.get(clé, défaut)      → retourne la valeur, défaut si inexistante
.keys()                → retourne toutes les clés
.values()              → retourne toutes les valeurs
.items()               → retourne les paires (clé, valeur)
.pop(clé)              → supprime et retourne la valeur
.clear()               → vide le dictionnaire
del dict[clé]          → supprime la clé
clé in dict            → True si la clé existe
len(dict)              → nombre de paires clé/valeur
dict[clé] = valeur     → ajoute ou modifie une valeur
```