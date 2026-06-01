

➡️ Fonctions déjà intégrées dans Python — pas besoin de les importer

---

## 1️⃣ Affichage / saisie

|Fonction|Utilité|Exemple|
|---|---|---|
|`print()`|Afficher dans le terminal|`print("Bonjour")` → `Bonjour`|
|`input()`|Demander une saisie|`input("Ton prénom ?")` → retourne un string|

---

## 2️⃣ Conversion de types

|Fonction|Utilité|Exemple|
|---|---|---|
|`int()`|Convertir en entier|`int("42")` → `42`|
|`float()`|Convertir en décimal|`float("3.14")` → `3.14`|
|`str()`|Convertir en texte|`str(42)` → `"42"`|
|`bool()`|Convertir en booléen|`bool(0)` → `False`|

---

## 3️⃣ Infos sur un objet

|Fonction|Utilité|Exemple|
|---|---|---|
|`type()`|Connaître le type|`type(42)` → `<class 'int'>`|
|`len()`|Connaître la longueur|`len([1, 2, 3])` → `3`|
|`id()`|Adresse mémoire|`id(a)` → `140234567891`|

---

## 4️⃣ Maths

|Fonction|Utilité|Exemple|
|---|---|---|
|`abs()`|Valeur absolue|`abs(-5)` → `5`|
|`round()`|Arrondir|`round(3.14159, 2)` → `3.14`|
|`max()`|Le plus grand|`max([3, 7, 2])` → `7`|
|`min()`|Le plus petit|`min([3, 7, 2])` → `2`|
|`sum()`|Additionner tout|`sum([1, 2, 3])` → `6`|

---

## 5️⃣ Listes / boucles

|Fonction|Utilité|Exemple|
|---|---|---|
|`range()`|Séquence de nombres|`range(5)` → `0, 1, 2, 3, 4`|
|`enumerate()`|Index + valeur|`enumerate(["a", "b"])` → `(0, "a"), (1, "b")`|
|`zip()`|Deux listes en parallèle|`zip([1,2], ["a","b"])` → `(1,"a"), (2,"b")`|

---

## 6️⃣ Tri / ordre

|Fonction|Utilité|Exemple|
|---|---|---|
|`sorted()`|Trier (nouvelle liste)|`sorted([3,1,2])` → `[1, 2, 3]`|
|`reversed()`|Inverser|`reversed([1,2,3])` → `3, 2, 1`|

---

## 7️⃣ Conditions avancées

|Fonction|Utilité|Exemple|
|---|---|---|
|`any()`|Au moins un vrai ?|`any([False, True])` → `True`|
|`all()`|Tous vrais ?|`all([True, False])` → `False`|

---

## 8️⃣ Fichiers

|Fonction|Utilité|Exemple|
|---|---|---|
|`open()`|Ouvrir un fichier|`open("fichier.txt", "r")`|
