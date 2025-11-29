# 🎓 **10 EXERCICES à FAIRE**

---

# ⭐ **Exercice 1 — Chaînes + compteur + fichier**

Écrire **3 fonctions** :

1. `int compterCaractere(char *str, char c);`

   * Retourne le nombre de fois où la lettre `c` apparaît dans la chaîne `str`.
   * Utiliser une boucle simple `while`.

2. `void enregistrerDansFichier(char *str, int nb);`

   * Ouvre le fichier **compte.txt** en mode écriture.
   * Écrit le nombre de caractères trouvés + la chaîne.
   * Ferme le fichier.

3. `void afficherSansEspaces(char *str);`

   * Affiche la chaîne sans afficher les espaces.
   * Garder les autres caractères.

---

# ⭐ **Exercice 2 — Tableau 2D (notes) + moyennes + recherche**

Écrire **3 fonctions** sur un tableau `int t[][3]` où chaque ligne représente un étudiant :

1. `void remplirNotes(int t[][3], int n);`

   * Lit les 3 notes de chaque étudiant via `scanf`.

2. `float moyenne(int t[][3], int etu);`

   * Calcule la moyenne des 3 notes d’un étudiant.

3. `int meilleur(int t[][3], int n);`

   * Retourne l’indice de l’étudiant ayant la meilleure moyenne.

---

# ⭐ **Exercice 3 — Chaînes simples : inversion + longueur + copie**

Écrire **3 fonctions** :

1. `int longueur(char *str);`

   * Calcule la longueur d’une chaîne (sans `strlen`).

2. `void inverser(char *str);`

   * Inverse la chaîne (ex : "papa" → "apap").

3. `void copier(char *dest, char *src);`

   * Copie `src` dans `dest`.
   * Sans utiliser `strcpy`.

---

# ⭐ **Exercice 4 — Pointeurs + tableau simple + écriture fichier**

Écrire **3 fonctions** :

1. `void lireTableau(int *t, int n);`

   * Lit les `n` valeurs du tableau avec `scanf`.

2. `int somme(int *t, int n);`

   * Retourne la somme du tableau.

3. `void sauvegarder(int *t, int n);`

   * Écrit les valeurs du tableau dans **tab.txt**.
   * Une seule ligne avec les nombres séparés par espaces.

---

# ⭐ **Exercice 5 — Tableau 2D + sommes + recherche d’une valeur**

Écrire **3 fonctions** :

1. `void remplir(int t[][4], int n);`

   * Lit un tableau 2D de `n` lignes et 4 colonnes.

2. `int sommeLigne(int t[][4], int ligne);`

   * Retourne la somme des 4 valeurs de la ligne.

3. `int contient(int t[][4], int n, int val);`

   * Retourne 1 si la valeur existe quelque part dans le tableau.

---

# ⭐ **Exercice 6 — Tableau de chaînes 2D + recherche + taille**

Écrire **3 fonctions** sur un tableau de mots `char mots[][20]` :

1. `void lireMots(char mots[][20], int n);`

   * Lit `n` mots avec `scanf("%19s")`.

2. `int plusLong(char mots[][20], int n);`

   * Retourne l’indice du mot le plus long.

3. `int existe(char mots[][20], int n, char *recherche);`

   * Retourne 1 si le mot recherché existe dans la liste.

---

# ⭐ **Exercice 7 — Fichier simple + tableau + calcul**

Créer un fichier texte nommé `nombres.txt` contenant **au moins 8 entiers**.

Écrire **3 fonctions** :

1. `void lireFichier(int *t, int n);`

   * Ouvre `nombres.txt` en lecture.
   * Lit les `n` premiers entiers du fichier dans le tableau.

2. `int max(int *t, int n);`

   * Retourne la plus grande valeur du tableau.

3. `void doubler(int *t, int n);`

   * Multiplie toutes les valeurs du tableau par 2.

---

# ⭐ **Exercice 8 — Tri + concaténation + chaînes**

Écrire **3 fonctions** :

1. `int taille(char *str);`

   * Calcule la longueur de la chaîne (sans `strlen`).

2. `void trierString(char *str);`

   * Trie tous les caractères de la chaîne par ordre alphabétique.

3. `void concatenation(char *dest, char *src);`

   * Ajoute `src` à la fin de `dest`.

---

# ⭐ **Exercice 9 — Tableau 2D + multiplication + affichage**

Écrire **3 fonctions** :

1. `void remplir2D(int t[][], int n);`

   * Lit un tableau 2D de `n` lignes et `j` colonnes.

2. `void multiplierLigne(int t[][], int ligne, int v);`

   * Multiplie chaque valeur de la ligne par `v`.

3. `void afficher(int t[][], int n);`

   * Affiche le tableau sous forme de grille.

---

# ⭐ **Exercice 10 — Chaîne + fichier + majuscules**

Écrire **3 fonctions** :

1. `int compterVoyelles(char *str);`

   * Retourne le nombre total de voyelles (a,e,i,o,u,y en MAJ ou min).

2. `void enregistrerPhrase(char *str);`

   * Écrit la chaîne dans un fichier **phrase.txt**.

3. `void mettreMaj(char *str);`

   * Transforme toutes les lettres minuscules en majuscules.
