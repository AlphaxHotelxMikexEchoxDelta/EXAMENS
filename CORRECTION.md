# ✅ **CORRECTION — EXAMEN DE PROGRAMMATION C**

---

# **PARTIE 1 — Correction des questions de cours**

1. **`scanf()` lit jusqu’au premier espace**, ne lit pas les espaces.
   **`fgets()` lit toute la ligne**, y compris les espaces, jusqu’au `\n`.

2. `\0` est **le caractère de fin de chaîne**. Il marque où s’arrête le texte.

3. `int t[5][3];`

4. Un pointeur est **une variable qui contient l’adresse d’une autre variable**.
   On l’utilise pour modifier des valeurs, gérer tableaux, chaînes, fonctions…

5. `float *p;`

6. * `fgets()` : lit une ligne depuis un fichier.
   * `fprintf()` : écrit dans un fichier.

7. Parce que `scanf()` a besoin de **l’adresse** où stocker la donnée.

8. `*` permet **d’accéder à la valeur pointée** (déréférencement).

9. `char nom[20] = "";` → chaîne vide.

10. Une fonction `void` **ne retourne rien**.

11. En passant son **nom**, ex : `maFonction(tableau);`
    (le nom représente une adresse)

12. La chaîne est **invalide** : risques de crash, lecture hors limites, affichage bizarre.

13. `FILE *f = fopen("fichier.txt", "w");`

14. `fclose()` **ferme le fichier** et libère les ressources.

15. Une variable simple stocke **une seule valeur**.
    Un tableau stocke **plusieurs valeurs** de même type.

---

# **PARTIE 2 — Correction des exercices**

---

# ⭐ Exercice 1

## **1. compteLongueur**

```c
int compteLongueur(char *str) {
    int i = 0;
    while (str[i] != '\0') {
        i++;
    }
    return i;
}
```

---

## **2. inverserPremierEtDernier**

```c
void inverserPremierEtDernier(char *str) {
    int len = compteLongueur(str);
    if (len < 2) return;

    char tmp = str[0];
    str[0] = str[len - 1];
    str[len - 1] = tmp;
}
```

---

## **3. contientVoyelle**

```c
int contientVoyelle(char *str) {
    for (int i = 0; str[i] != '\0'; i++) {
        char c = str[i];
        if (c=='a' || c=='e' || c=='i' || c=='o' || c=='u' || c=='y' ||
            c=='A' || c=='E' || c=='I' || c=='O' || c=='U' || c=='Y') {
            return 1;
        }
    }
    return 0;
}
```

---

# ⭐ Exercice 2 — Tableaux de notes

## **1. remplirNotes**

```c
void remplirNotes(int notes[][], int n) {
    for (int i = 0; i < n; i++) {
        printf("Etudiant %d :\n", i);
        for (int j = 0; j < 5; j++) {
            printf("  Note %d : ", j);
            scanf("%d", &notes[i][j]);
        }
    }
}
```

---

## **2. moyenneEtudiant**

```c
float moyenneEtudiant(int notes[][], int index) {
    int somme = 0;
    for (int j = 0; j < 5; j++) {
        somme += notes[index][j];
    }
    return somme / 5.0;
}
```

---

## **3. meilleurEtudiant**

```c
int meilleurEtudiant(int notes[][], int n) {
    int best = 0;
    float bestMoy = moyenneEtudiant(notes, 0);

    for (int i = 1; i < n; i++) {
        float m = moyenneEtudiant(notes, i);
        if (m > bestMoy) {
            bestMoy = m;
            best = i;
        }
    }
    return best;
}
```

---

# **PARTIE 3 — Analyse de code (correction)**

---

## **Question 1**

### Ligne expliquée :

`s[i] != '\0'`
→ On continue la boucle **tant que la chaîne n’est pas terminée**.

### Résultat du code :

Dans `"bonjour"`, les `'o'` sont aux positions 1 et 3.

Affichage :

```
O trouve a la position 1
O trouve a la position 3
```

---

## **Question 2**

### Ligne expliquée :

`a = *q - *p;`
→ `*q` vaut `12`, `*p` vaut `5`, donc `a = 12 - 5 = 7`.

### Calcul complet :

* `a` devient 7
* `*q = a + b = 7 + 12 = 19` → donc `b = 19`
* `*p` lit la valeur de `a` → 7
* `*q` lit la valeur de `b` → 19

### Affichage :

```
7 19 7 19
```

---

## **Question 3**

Somme =
1 + 2 + 3 + 4 + 5 + 6 = **21**

### Ligne expliquée :

`somme += t[i][j];`
→ On ajoute chaque élément du tableau à la variable somme.

### Affichage :

```
Somme : 21
```

---

## **Question 4**

### Ligne expliquée :

`copie[i] = mot[i];`
→ On copie chaque caractère de `mot` dans `copie`.

### Résultat :

`copie` devient `"orange"`

### Affichage :

```
Copie = orange
```

---

## **Question 5**

### Ligne expliquée :

`if (entree[i] >= '0' && entree[i] <= '9')`
→ Teste si le caractère est un **chiffre ASCII** entre 0 et 9.

### Fonction du programme :

Il **compte combien de chiffres** l’utilisateur a saisis.

Exemple : entrée `"ab12cd5"` → affiche :

```
Il y a 3 chiffres dans la saisie.
```
