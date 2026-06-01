## 📦 int

⚠️  Ce sont les **nombres sans virgule**, positifs ou négatifs.

#### 💡 <span style="color: cyan;">Exemple</span>

``` python
age = 25          # positif
temperature = -3     # negatif
```


---

## 📦 float

⚠️  Les nombres **avec une virgule** (notée `.` en Python comme en anglais).

### 💡 <span style="color: cyan;">Exemple</span>

``` python
PI = 3.14159
```


---

## 📦 str

⚠️  Du texte, toujours entre **guillemets** (simples `'` ou doubles `"`).

### 💡 <span style="color: cyan;">Exemple</span>

``` python
prenom = "Sara" # "Sara" est un objet de type str
```


---

## 📦 bool

⚠️  Le type le plus simple : seulement **deux valeurs possibles**.

### 💡 <span style="color: cyan;">Exemple</span>

``` python
est_connecte = True 
a_gagne = False
```


---

## 🔍 Comment connaître le type d'une variable ?

```python

age = 25
print(type(age))        # → <class 'int'>

taille = 1.75
print(type(taille))     # → <class 'float'>

prenom = "Sara"
print(type(prenom))     # → <class 'str'>

actif = True
print(type(actif))      # → <class 'bool'>
```