
## 📦 Les Variables

⚠️  Une variable, c'est un nom qu'on crée pour stocker une valeur. Ce nom peut ensuite être passé à une fonction ou méthode pour utiliser le contenu qu'il représente. Le type de la variable dépend de la valeur qu'on lui assigne.


➡️  **Modifiable** à tout moment
➡️ Est **typée dynamiquement** — Python trouve le type tout seul
➡️ Peut **changer de type** en cours de programme 

### 💡 <span style="color: cyan;">Exemple</span>

``` python
age = 25          # Python voit un entier → int
taille = 1.70     # Python voit un décimal → float
prenom = "Sara"   # Python voit des guillemets → str

```


---

## 📦 Les Constantes

⚠️  Une constante, c'est comme une variable mais dont la valeur **ne doit pas être modifiée** pendant le programme. En Python, on l'écrit en **MAJUSCULES** pour signaler aux autres développeurs de ne pas y toucher

➡️  **Non modifiable par convention**
➡️ En MAJUSCULES_AVEC_UNDERSCORE
➡️  Est définie **une seule fois** au début du programme

### 💡 <span style="color: cyan;">Exemple</span>

``` python
PI = 3.14159
MAX_JOUEURS = 10
COULEUR_FOND = "noir"

# Mauvaise pratique même si Python l'autorise :
PI = 5  # non !
```


---

## 📦 Les Objets

⚠️  Un objet, c'est ce que la variable pointe. En Python tout est objet — un str, un int, une liste... Chaque objet a un type, une valeur, et des méthodes intégrées qu'on peut utiliser.

### 💡 <span style="color: cyan;">Exemple</span>

``` python
prenom = "Sara" # "Sara" est un objet de type str
```


