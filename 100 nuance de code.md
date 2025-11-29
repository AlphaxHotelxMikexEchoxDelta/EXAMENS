### **Exercice 1 — Compter les nombres pairs dans un tableau**

```c
int compterPairs(int *tab, int n);
```

* Retourne le nombre d’éléments pairs dans un tableau `tab` de taille `n`.

---

### **Exercice 2 — Somme des éléments d’un tableau**

```c
int sommeTableau(int *tab, int n);
```

* Retourne la somme de tous les éléments du tableau `tab`.

---

### **Exercice 3 — Inverser un tableau d’entiers**

```c
void inverserTableau(int *tab, int n);
```

* Inverse les éléments d’un tableau `tab` de taille `n` sans tableau supplémentaire.

---

### **Exercice 4 — Trouver le maximum dans un tableau**

```c
int maximum(int *tab, int n);
```

* Retourne la valeur maximale du tableau.

---

### **Exercice 5 — Compter les voyelles d’une chaîne**

```c
int compterVoyelles(char *str);
```

* Retourne le nombre de voyelles (`a, e, i, o, u, y`).

---

### **Exercice 6 — Convertir une chaîne en majuscules**

```c
void enMajuscules(char *str);
```

* Transforme tous les caractères minuscules de `str` en majuscules.

---

### **Exercice 7 — Copier une chaîne dans une autre**

```c
void copierChaine(char *dest, char *src);
```

* Copie la chaîne `src` dans `dest`.

---

### **Exercice 8 — Trier un tableau d’entiers (tri bulle)**

```c
void trierTableau(int *tab, int n);
```

* Trie le tableau en ordre croissant.

---

### **Exercice 9 — Compter combien de fois un chiffre apparaît dans un tableau**

```c
int compterValeur(int *tab, int n, int val);
```

* Retourne le nombre de fois que `val` apparaît.

---

### **Exercice 10 — Vérifier si un tableau est trié**

```c
int estTrie(int *tab, int n);
```

* Retourne 1 si le tableau est trié en ordre croissant, 0 sinon.

---

### **Exercice 11 — Calculer la moyenne d’un tableau**

```c
float moyenne(int *tab, int n);
```

* Retourne la moyenne des éléments.

---

### **Exercice 12 — Ajouter un entier à chaque élément du tableau**

```c
void ajouterValeur(int *tab, int n, int val);
```

* Ajoute `val` à chaque élément du tableau.

---

### **Exercice 13 — Remplir un tableau avec des carrés**

```c
void remplirCarres(int *tab, int n);
```

* Remplit le tableau avec `0^2, 1^2, 2^2, ..., (n-1)^2`.

---

### **Exercice 14 — Vérifier si un mot est palindrome**

```c
int estPalindrome(char *str);
```

* Retourne 1 si la chaîne est palindrome, 0 sinon.

---

### **Exercice 15 — Compter les mots dans une phrase**

```c
int compterMots(char *str);
```

* Retourne le nombre de mots (séparés par des espaces).

---

### **Exercice 16 — Inverser une chaîne**

```c
void inverserChaine(char *str);
```

* Inverse les caractères de la chaîne.

---

### **Exercice 17 — Mélanger aléatoirement un tableau**

```c
void melangerTableau(int *tab, int n);
```

* Mélange les éléments du tableau aléatoirement.

---

### **Exercice 18 — Extraire les chiffres d’une chaîne**

```c
int extraireChiffres(char *str, int *tab);
```

* Remplit `tab` avec les chiffres trouvés dans `str`.
* Retourne le nombre de chiffres trouvés.

---

### **Exercice 19 — Rechercher la position d’une valeur**

```c
int chercherPosition(int *tab, int n, int val);
```

* Retourne l’indice de `val` dans le tableau, -1 si non trouvé.

---

### **Exercice 20 — Supprimer toutes les occurrences d’une valeur**

```c
int supprimerValeur(int *tab, int n, int val);
```

* Supprime toutes les occurrences de `val` dans le tableau.
* Retourne la nouvelle taille du tableau.

---

### **Exercice 21 — Afficher les éléments d’un tableau**

```c
void afficherTableau(int *tab, int n);
```

* Affiche tous les éléments séparés par un espace.

---

### **Exercice 22 — Vérifier si un entier est pair**

```c
int estPair(int x);
```

* Retourne 1 si `x` est pair, 0 sinon.

---

### **Exercice 23 — Trouver le plus petit élément**

```c
int minimum(int *tab, int n);
```

* Retourne la valeur minimale d’un tableau.

---

### **Exercice 24 — Compter les lettres majuscules dans une chaîne**

```c
int compterMajuscules(char *str);
```

* Retourne le nombre de lettres majuscules.

---

### **Exercice 25 — Vérifier si une chaîne contient une lettre donnée**

```c
int contientLettre(char *str, char c);
```

* Retourne 1 si `c` est présent dans `str`.

---

### **Exercice 26 — Multiplier chaque élément d’un tableau par un entier**

```c
void multiplierTableau(int *tab, int n, int m);
```

* Multiplie chaque élément par `m`.

---

### **Exercice 27 — Répéter une chaîne N fois**

```c
void repeterChaine(char *str, int n);
```

* Répète la chaîne `n` fois dans la même variable (attention à la taille du tableau).

---

### **Exercice 28 — Compter les caractères spéciaux**

```c
int compterSpeciaux(char *str);
```

* Compte les caractères qui ne sont pas lettres ou chiffres.

---

### **Exercice 29 — Convertir un tableau en tableau de booléens (0 ou 1 selon si pair)**

```c
void tableauBool(int *tab, int n, int *res);
```

* `res[i] = 1` si `tab[i]` pair, 0 sinon.

---

### **Exercice 30 — Ajouter un tableau dans un autre**

```c
void additionTableaux(int *a, int *b, int *res, int n);
```

* `res[i] = a[i] + b[i]`.

---

### **Exercice 31 — Extraire les lettres d’une chaîne**

```c
int extraireLettres(char *str, char *res);
```

* Met toutes les lettres de `str` dans `res`. Retourne le nombre de lettres.

---

### **Exercice 32 — Compter combien de fois un mot apparaît dans une phrase**

```c
int compterMot(char *phrase, char *mot);
```

* Retourne le nombre d’occurrences exactes de `mot` dans `phrase`.

---

### **Exercice 33 — Trouver la valeur médiane d’un tableau**

```c
int mediane(int *tab, int n);
```

* Retourne la médiane (tri simple nécessaire).

---

### **Exercice 34 — Inverser les mots dans une phrase**

```c
void inverserMots(char *phrase);
```

* Inverse l’ordre des mots (ex: "bonjour le monde" → "monde le bonjour").

---

### **Exercice 35 — Vérifier si un tableau est symétrique**

```c
int estSymetrique(int *tab, int n);
```

* Retourne 1 si `tab[i] == tab[n-1-i]` pour tout `i`.

---

### **Exercice 36 — Compter le nombre de chiffres dans une chaîne**

```c
int compterChiffres(char *str);
```

* Retourne le nombre de caractères `0-9`.

---

### **Exercice 37 — Remplacer toutes les occurrences d’un caractère**

```c
void remplacerCaractere(char *str, char ancien, char nouveau);
```

* Remplace `ancien` par `nouveau` dans `str`.

---

### **Exercice 38 — Décaler un tableau vers la droite**

```c
void decalageDroite(int *tab, int n);
```

* Décale tous les éléments d’une position vers la droite (dernier devient premier).

---

### **Exercice 39 — Somme cumulative**

```c
void sommeCumulative(int *tab, int n, int *res);
```

* `res[i] = tab[0] + tab[1] + ... + tab[i]`.

---

### **Exercice 40 — Vérifier si une chaîne contient uniquement des lettres**

```c
int uniquementLettres(char *str);
```

* Retourne 1 si tous les caractères sont des lettres, 0 sinon.

---

### **Exercice 40 — Compter les consonnes dans une chaîne**

```c
int compterConsonnes(char *str);
```

* Retourne le nombre de lettres qui ne sont pas des voyelles.

---

### **Exercice 41 — Vérifier si un entier est multiple d’un autre**

```c
int estMultiple(int a, int b);
```

* Retourne 1 si `a` est multiple de `b`, 0 sinon.

---

### **Exercice 42 — Répéter un tableau N fois dans un autre tableau**

```c
void repeterTableau(int *tab, int n, int *res, int k);
```

* Remplit `res` avec `tab` répété `k` fois.

---

### **Exercice 43 — Convertir minuscules en majuscules et vice-versa**

```c
void inverserCasse(char *str);
```

* Les lettres minuscules deviennent majuscules et inversement.

---

### **Exercice 44 — Compter combien de fois une lettre apparaît**

```c
int compterLettre(char *str, char c);
```

* Retourne le nombre de fois que `c` apparaît dans la chaîne.

---

### **Exercice 45 — Décaler un tableau vers la gauche**

```c
void decalageGauche(int *tab, int n);
```

* Décale tous les éléments d’une position vers la gauche (premier devient dernier).

---

### **Exercice 46 — Calculer la factorielle d’un entier**

```c
int factorielle(int n);
```

* Retourne `n!`.

---

### **Exercice 47 — Compter les espaces dans une chaîne**

```c
int compterEspaces(char *str);
```

* Retourne le nombre de caractères `' '`.

---

### **Exercice 48 — Vérifier si un tableau contient un doublon**

```c
int contientDoublon(int *tab, int n);
```

* Retourne 1 si au moins deux éléments sont identiques.

---

### **Exercice 49 — Remplacer tous les espaces par un caractère donné**

```c
void remplacerEspaces(char *str, char c);
```

* Remplace chaque espace `' '` par le caractère `c`.

---

### **Exercice 50 — Calculer la somme des nombres impairs**

```c
int sommeImpairs(int *tab, int n);
```

* Retourne la somme de tous les éléments impairs.

---

### **Exercice 51 — Vérifier si une chaîne commence par un mot donné**

```c
int commencePar(char *str, char *mot);
```

* Retourne 1 si `str` commence exactement par `mot`.

---

### **Exercice 52 — Trouver le deuxième maximum dans un tableau**

```c
int deuxiemeMax(int *tab, int n);
```

* Retourne le deuxième plus grand élément.

---

### **Exercice 53 — Afficher les éléments impairs d’un tableau**

```c
void afficherImpairs(int *tab, int n);
```

* Affiche uniquement les éléments impairs.

---

### **Exercice 54 — Compter combien de mots commencent par une lettre**

```c
int motsCommencentPar(char *phrase, char c);
```

* Retourne le nombre de mots dont la première lettre est `c`.

---

### **Exercice 55 — Trouver l’indice du minimum dans un tableau**

```c
int indiceMin(int *tab, int n);
```

* Retourne l’indice du plus petit élément.

---

### **Exercice 56 — Calculer le produit de tous les éléments**

```c
int produitTableau(int *tab, int n);
```

* Retourne le produit de tous les éléments du tableau.

---

### **Exercice 57 — Inverser les mots d’un tableau de chaînes**

```c
void inverserMotsTab(char tab[][20], int n);
```

* Inverse l’ordre des chaînes dans le tableau.

---

### **Exercice 58 — Vérifier si un tableau est strictement croissant**

```c
int estCroissant(int *tab, int n);
```

* Retourne 1 si `tab[i] < tab[i+1]` pour tous les `i`.

---

### **Exercice 59 — Supprimer les voyelles d’une chaîne**

```c
void supprimerVoyelles(char *str);
```

* Supprime toutes les voyelles (`a,e,i,o,u,y`) de la chaîne.

---

### **Exercice 60 — Compter les chiffres pairs dans une chaîne**

```c
int chiffresPairs(char *str);
```

* Retourne le nombre de chiffres pairs présents dans la chaîne.

---

### **Exercice 61 — Vérifier si un tableau contient un nombre donné**

```c
int contientNombre(int *tab, int n, int val);
```

* Retourne 1 si `val` est présent dans le tableau, 0 sinon.

---

### **Exercice 62 — Remplacer les minuscules par des étoiles**

```c
void remplacerMinuscules(char *str);
```

* Remplace chaque lettre minuscule par `'*'`.

---

### **Exercice 63 — Calculer la moyenne des nombres impairs d’un tableau**

```c
float moyenneImpairs(int *tab, int n);
```

* Retourne la moyenne des éléments impairs uniquement.

---

### **Exercice 64 — Trouver le premier élément supérieur à une valeur**

```c
int premierSuperieur(int *tab, int n, int val);
```

* Retourne l’indice du premier élément strictement supérieur à `val`.
* Retourne -1 si aucun.

---

### **Exercice 65 — Vérifier si un mot est contenu dans une phrase**

```c
int contientMot(char *phrase, char *mot);
```

* Retourne 1 si `mot` apparaît exactement dans `phrase`, 0 sinon.

---

### **Exercice 66 — Ajouter une valeur à tous les éléments d’un tableau**

```c
void ajouterTous(int *tab, int n, int val);
```

* Ajoute `val` à chaque élément.

---

### **Exercice 67 — Vérifier si un tableau contient uniquement des nombres positifs**

```c
int uniquementPositifs(int *tab, int n);
```

* Retourne 1 si tous les éléments sont ≥ 0, 0 sinon.

---

### **Exercice 68 — Compter les lettres minuscules**

```c
int compterMinuscules(char *str);
```

* Retourne le nombre de lettres minuscules dans la chaîne.

---

### **Exercice 69 — Décaler une chaîne de caractères vers la droite**

```c
void decalageDroiteChaine(char *str);
```

* Décale tous les caractères d’une position vers la droite (dernier devient premier).

---

### **Exercice 70 — Trouver le troisième maximum dans un tableau**

```c
int troisiemeMax(int *tab, int n);
```

* Retourne le troisième plus grand élément.

---

### **Exercice 71 — Vérifier si un tableau est palindrome**

```c
int tableauPalindrome(int *tab, int n);
```

* Retourne 1 si le tableau se lit pareil de gauche à droite et droite à gauche.

---

### **Exercice 72 — Multiplier les éléments impairs d’un tableau**

```c
void multiplierImpairs(int *tab, int n, int val);
```

* Multiplie uniquement les éléments impairs par `val`.

---

### **Exercice 73 — Compter le nombre de mots dans une phrase**

```c
int compterMotsPhrase(char *str);
```

* Retourne le nombre de mots séparés par des espaces.

---

### **Exercice 74 — Extraire les voyelles dans un tableau de caractères**

```c
int extraireVoyelles(char *str, char *res);
```

* Remplit `res` avec les voyelles de `str`. Retourne le nombre de voyelles.

---

### **Exercice 75 — Inverser les voyelles dans une chaîne**

```c
void inverserVoyelles(char *str);
```

* Inverse uniquement les voyelles, les autres lettres restent à leur place.

---

### **Exercice 76 — Supprimer les doublons dans un tableau**

```c
int supprimerDoublons(int *tab, int n);
```

* Supprime tous les doublons. Retourne la nouvelle taille du tableau.

---

### **Exercice 77 — Vérifier si deux chaînes sont identiques**

```c
int chainesEgales(char *s1, char *s2);
```

* Retourne 1 si `s1` et `s2` sont identiques, 0 sinon.

---

### **Exercice 78 — Calculer le carré de chaque élément d’un tableau**

```c
void carreTableau(int *tab, int n);
```

* Remplace chaque élément par son carré.

---

### **Exercice 79 — Compter le nombre de mots commençant par une voyelle**

```c
int motsVoyelles(char *str);
```

* Retourne le nombre de mots dont la première lettre est une voyelle.

---

### **Exercice 80 — Vérifier si un tableau contient un nombre impair**

```c
int contientImpair(int *tab, int n);
```

* Retourne 1 si au moins un élément est impair, 0 sinon.

---

### **Exercice 81 — Remplacer toutes les lettres majuscules par un caractère**

```c
void remplacerMajuscules(char *str, char c);
```

* Remplace chaque lettre majuscule par le caractère `c`.

---

### **Exercice 82 — Calculer la moyenne pondérée d’un tableau**

```c
float moyennePonderee(int *tab, int *poids, int n);
```

* Retourne `(tab[0]*poids[0] + ... + tab[n-1]*poids[n-1]) / somme(poids)`.

---

### **Exercice 83 — Retourner l’indice du plus grand élément pair**

```c
int indiceMaxPair(int *tab, int n);
```

* Retourne l’indice du plus grand élément pair, -1 si aucun.

---

### **Exercice 84 — Compter les caractères alphabétiques**

```c
int compterAlphabets(char *str);
```

* Retourne le nombre de lettres (maj et min).

---

### **Exercice 85 — Vérifier si un tableau est strictement décroissant**

```c
int estDecroissant(int *tab, int n);
```

* Retourne 1 si `tab[i] > tab[i+1]` pour tous les `i`.

---

### **Exercice 86 — Décaler un tableau circulairement vers la gauche**

```c
void decalageCirculaireGauche(int *tab, int n, int k);
```

* Décale `k` positions vers la gauche.

---

### **Exercice 87 — Supprimer tous les chiffres d’une chaîne**

```c
void supprimerChiffres(char *str);
```

* Supprime les caractères `0–9` de la chaîne.

---

### **Exercice 88 — Calculer la somme des carrés**

```c
int sommeCarres(int *tab, int n);
```

* Retourne `tab[0]^2 + tab[1]^2 + ... + tab[n-1]^2`.

---

### **Exercice 89 — Vérifier si une chaîne est composée uniquement de chiffres**

```c
int uniquementChiffres(char *str);
```

* Retourne 1 si tous les caractères sont `0–9`, 0 sinon.

---

### **Exercice 90 — Rechercher le caractère le plus fréquent dans une chaîne**

```c
char caractereFrequent(char *str);
```

* Retourne le caractère apparaissant le plus souvent.

---

### **Exercice 91 — Compter le nombre de mots de longueur ≥ N**

```c
int motsLongueurN(char *str, int n);
```

* Retourne le nombre de mots dont la longueur ≥ `n`.

---

### **Exercice 92 — Ajouter 1 à tous les éléments d’un tableau**

```c
void incrementerTableau(int *tab, int n);
```

* Ajoute 1 à chaque élément.

---

### **Exercice 93 — Vérifier si une chaîne contient uniquement des lettres et espaces**

```c
int lettresEtEspaces(char *str);
```

* Retourne 1 si tous les caractères sont lettres ou espaces.

---

### **Exercice 94 — Multiplier tous les éléments d’un tableau par un tableau de coefficients**

```c
void multiplierParCoefficients(int *tab, int *coef, int n);
```

* Chaque élément devient `tab[i] *= coef[i]`.

---

### **Exercice 95 — Extraire les majuscules dans une chaîne**

```c
int extraireMajuscules(char *str, char *res);
```

* Met dans `res` toutes les majuscules. Retourne le nombre de majuscules.

---

### **Exercice 96 — Inverser un tableau de caractères**

```c
void inverserTableauChar(char *tab, int n);
```

* Inverse tous les caractères dans le tableau `tab` de taille `n`.

---

### **Exercice 97 — Compter les lettres après un certain indice**

```c
int compterApresIndice(char *str, int indice);
```

* Retourne le nombre de lettres après la position `indice` dans la chaîne.

---

### **Exercice 98 — Calculer la différence entre max et min**

```c
int differenceMaxMin(int *tab, int n);
```

* Retourne `max(tab) - min(tab)`.

---

### **Exercice 99 — Vérifier si un mot est présent au début ou à la fin d’une phrase**

```c
int debutFin(char *phrase, char *mot);
```

* Retourne 1 si `mot` est au début ou à la fin de `phrase`, 0 sinon.

---


# **Exercice 100 — Matrice 4D 5×5×5×5 avec valeurs entre 0 et 1**

**Objectif :**

1. Générer une matrice 4D `mat[5][5][5][5]` avec des valeurs aléatoires entre -0.5 et 1.5.
2. Parcourir la matrice et **repérer toutes les valeurs qui ne sont pas entre 0 et 1**.
3. Corriger ces valeurs : `<0` → `0`, `>1` → `1`.
4. Afficher un résumé du nombre de corrections.

---

## **Prototype des fonctions**

### 1. `void genererMatrice(float mat[5][5][5][5]);`

* Remplit la matrice avec des valeurs aléatoires entre -0.5 et 1.5.

### 2. `int corrigerMatrice(float mat[5][5][5][5]);`

* Parcourt la matrice, corrige les valeurs hors [0,1], et retourne le nombre de corrections.

### 3. `void afficherMatrice(float mat[5][5][5][5]);`

* Affiche toutes les valeurs.

---

## **Exemple de main**

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    float mat[5][5][5][5];
    srand(time(NULL));

    genererMatrice(mat);

    printf("Matrice avant correction :\n");
    afficherMatrice(mat);

    int nbCorrige = corrigerMatrice(mat);
    printf("\nNombre de valeurs corrigées : %d\n", nbCorrige);

    printf("\nMatrice apres correction :\n");
    afficherMatrice(mat);

    return 0;
}
```
