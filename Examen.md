# 📘 **EXAMEN DE PROGRAMMATION C — Version Finale**

---

# **PARTIE 1 — Questions de cours (15 questions)**

1. Quelle est la différence entre `scanf()` et `fgets()` pour la saisie utilisateur ?
2. Que représente le caractère `\0` dans une chaîne de caractères en C ?
3. Comment déclare-t-on un tableau 2D de 5 lignes et 3 colonnes contenant des `int` ?
4. Qu’est-ce qu’un pointeur et pourquoi l’utilise-t-on ?
5. Écrire la syntaxe permettant de déclarer un pointeur vers un `float`.
6. Dans un fichier, quelle est la différence entre `fgets()` et `fprintf()` ?
7. Pourquoi utilise-t-on `&` avec `scanf()` ?
8. Que permet l'opérateur `*` lorsqu'il est utilisé devant un pointeur ?
9. Comment initialise-t-on une chaîne de caractères vide en C ?
10. Qu’est-ce qu’une fonction `void` en langage C ?
11. Comment passe-t-on un tableau en paramètre à une fonction ?
12. Que se passe-t-il si une chaîne n’a pas de caractère `\0` ?
13. Comment ouvre-t-on un fichier en mode écriture ?
14. À quoi sert la fonction `fclose()` ?
15. Quelle est la différence entre un tableau et une variable simple ?

---

# **PARTIE 2 — Exercices pratiques**

---

# ⭐ **Exercice 1 : Chaînes et pointeurs**

### **1. `int compteLongueur(char *str)`**

Écrire une fonction qui retourne le nombre de caractères dans la chaîne (jusqu’au `\0`).

---

### **2. `void inverserPremierEtDernier(char *str)`**

Écrire une fonction qui inverse le premier et le dernier caractère d’une chaîne si elle contient au moins 2 caractères.
Exemples :

* `"papa"` → `"aapp"`
* `"ab"` → `"ba"`
* `"x"` → `"x"` (inchangé)

---

### **3. `int contientVoyelle(char *str)`**

Écrire une fonction qui retourne `1` si la chaîne contient une voyelle (`a, e, i, o, u, y`), sinon `0`.

---

# ⭐ **Exercice 2 : Tableaux 2D — Statistiques**

### **1. `void remplirNotes(int notes[][], int n)`**

L’utilisateur remplit les notes de **n étudiants**, chacun ayant **5 notes** (avec `scanf`).

---

### **2. `float moyenneEtudiant(int notes[][], int index)`**

Calcule et retourne la moyenne des 5 notes de l’étudiant numéro `index`.

---

### **3. `int meilleurEtudiant(int notes[][], int n)`**

Retourne l’indice de l’étudiant ayant la meilleure moyenne générale.

---

# **PARTIE 3 — Analyse de code (5 questions)**

Pour chaque code :

1. expliquer la ligne demandée
2. décrire ce que le programme affiche ou calcule.

---

## **Question 1**

```c
char s[20] = "bonjour";
int i = 0;

while (s[i] != '\0') {
    if (s[i] == 'o') {
        printf("O trouve a la position %d\n", i);
    }
    i++;
}
```

➡ **Ligne à expliquer :** `s[i] != '\0'`
➡ **Dire ce que le code affiche.**

---

## **Question 2**

```c
int a = 5;
int b = 12;
int *p = &a;
int *q = &b;

a = *q - *p;
*q = a + b;

printf("%d %d %d %d\n", a, b, *p, *q);
```

➡ **Ligne à expliquer :** `a = *q - *p;`
➡ **Dire ce que le programme affiche.**

---

## **Question 3**

```c
int t[2][3] = {{1,2,3},{4,5,6}};
int somme = 0;

for (int i = 0; i < 2; i++) {
    for (int j = 0; j < 3; j++) {
        somme += t[i][j];
    }
}

printf("Somme : %d\n", somme);
```

➡ **Ligne à expliquer :** `somme += t[i][j];`
➡ **Donner la somme finale.**

---

## **Question 4**

```c
char mot[20] = "orange";
char copie[20];
int i = 0;

while (mot[i] != '\0') {
    copie[i] = mot[i];
    i++;
}
copie[i] = '\0';

printf("Copie = %s\n", copie);
```

➡ **Ligne à expliquer :** `copie[i] = mot[i];`
➡ **Dire ce que le programme affiche.**

---

## **Question 5**

```c
char entree[30];
printf("Entrez un mot : ");
fgets(entree, 30, stdin);

int count = 0;
for (int i = 0; entree[i] != '\0'; i++) {
    if (entree[i] >= '0' && entree[i] <= '9') {
        count++;
    }
}

printf("Il y a %d chiffres dans la saisie.\n", count);
```

➡ **Ligne à expliquer :** `if (entree[i] >= '0' && entree[i] <= '9')`
➡ **Dire ce que calcule le programme.**
