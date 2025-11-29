## **Exercice 1 — Chaînes + compteur + fichier**

```c
#include <stdio.h>

int compterCaractere(char *str, char c) {
    int nb = 0, i = 0;
    while (str[i] != '\0') {
        if (str[i] == c) nb++;
        i++;
    }
    return nb;
}

void enregistrerDansFichier(char *str, int nb) {
    FILE *f = fopen("compte.txt", "w");
    fprintf(f, "Il y a %d occurences dans : %s", nb, str);
    fclose(f);
}

void afficherSansEspaces(char *str) {
    int i = 0;
    while (str[i] != '\0') {
        if (str[i] != ' ') printf("%c", str[i]);
        i++;
    }
    printf("\n");
}

/* Exemple d'utilisation */
int main(void) {
    char s[100];
    char c;
    printf("Entrez une phrase : ");
    scanf(" %[^\n]", s); // lit la ligne avec espaces
    printf("Entrez un caractere a chercher : ");
    scanf(" %c", &c);
    int nb = compterCaractere(s, c);
    printf("Nombre de '%c' : %d\n", c, nb);
    afficherSansEspaces(s);
    enregistrerDansFichier(s, nb);
    printf("Resultat ecrit dans compte.txt\n");
    return 0;
}
```

---

## **Exercice 2 — Tableau 2D (notes) + moyennes + meilleur**

```c
#include <stdio.h>

void remplirNotes(int t[][3], int n) {
    for(int i=0;i<n;i++)
        for(int j=0;j<3;j++){
            printf("Note %d de l'etudiant %d : ", j, i);
            scanf("%d",&t[i][j]);
        }
}

float moyenne(int t[][3], int etu){
    int s=0;
    for(int j=0;j<3;j++) s+=t[etu][j];
    return s/3.0f;
}

int meilleur(int t[][3], int n){
    int best=0;
    float mbest = moyenne(t,0);
    for(int i=1;i<n;i++){
        float m = moyenne(t,i);
        if(m>mbest){ mbest=m; best=i; }
    }
    return best;
}

/* Exemple */
int main(void){
    int n;
    printf("Nombre d'etudiants : ");
    scanf("%d",&n);
    int notes[n][3];
    remplirNotes(notes,n);
    int best = meilleur(notes,n);
    printf("Etudiant avec meilleure moyenne : %d\n", best);
    return 0;
}
```

---

## **Exercice 3 — Chaînes simples : longueur, inversion, copie**

```c
#include <stdio.h>

int longueur(char *str){
    int i=0;
    while(str[i]!='\0') i++;
    return i;
}

void inverser(char *str){
    int i=0, j=longueur(str)-1;
    while(i<j){
        char tmp = str[i]; str[i]=str[j]; str[j]=tmp;
        i++; j--;
    }
}

void copier(char *dest, char *src){
    int i=0;
    while(src[i]!='\0'){ dest[i]=src[i]; i++; }
    dest[i]='\0';
}

/* Exemple */
int main(void){
    char mot[50], copie[50];
    printf("Entrez un mot : ");
    scanf("%s", mot);
    printf("Longueur : %d\n", longueur(mot));
    inverser(mot);
    printf("Inverse : %s\n", mot);
    copier(copie, mot);
    printf("Copie : %s\n", copie);
    return 0;
}
```

---

## **Exercice 4 — Pointeurs + tableau simple + fichier**

```c
#include <stdio.h>

void lireTableau(int *t, int n){
    for(int i=0;i<n;i++){
        printf("t[%d] = ", i);
        scanf("%d",&t[i]);
    }
}

int somme(int *t, int n){
    int s=0;
    for(int i=0;i<n;i++) s+=t[i];
    return s;
}

void sauvegarder(int *t, int n){
    FILE *f = fopen("tab.txt","w");
    for(int i=0;i<n;i++) fprintf(f,"%d ", t[i]);
    fclose(f);
}

/* Exemple */
int main(void){
    int n;
    printf("Taille du tableau : ");
    scanf("%d",&n);
    int t[n];
    lireTableau(t,n);
    printf("Somme = %d\n", somme(t,n));
    sauvegarder(t,n);
    printf("Tableau sauvegarde dans tab.txt\n");
    return 0;
}
```

---

## **Exercice 5 — Tableau 2D + somme ligne + recherche**

```c
#include <stdio.h>

void remplir(int t[][4], int n){
    for(int i=0;i<n;i++)
        for(int j=0;j<4;j++){
            printf("t[%d][%d] = ", i,j);
            scanf("%d",&t[i][j]);
        }
}

int sommeLigne(int t[][4], int ligne){
    int s=0;
    for(int j=0;j<4;j++) s+=t[ligne][j];
    return s;
}

int contient(int t[][4], int n, int val){
    for(int i=0;i<n;i++)
        for(int j=0;j<4;j++)
            if(t[i][j]==val) return 1;
    return 0;
}

/* Exemple */
int main(void){
    int n;
    printf("Nombre de lignes : ");
    scanf("%d",&n);
    int t[n][4];
    remplir(t,n);
    int ligne;
    printf("Somme de quelle ligne ? ");
    scanf("%d",&ligne);
    printf("Somme = %d\n", sommeLigne(t,ligne));
    int val;
    printf("Valeur a chercher : ");
    scanf("%d",&val);
    printf(contient(t,n,val) ? "Trouvee\n" : "Non trouvee\n");
    return 0;
}
```

---

## **Exercice 6 — Tableau de chaînes 2D + plus long + recherche**

```c
#include <stdio.h>

void lireMots(char mots[][20], int n){
    for(int i=0;i<n;i++){
        printf("Mot %d : ", i);
        scanf("%19s", mots[i]);
    }
}

int plusLong(char mots[][20], int n){
    int best=0, max=0;
    for(int i=0;i<n;i++){
        int j=0; while(mots[i][j]!='\0') j++;
        if(j>max){ max=j; best=i; }
    }
    return best;
}

int existe(char mots[][20], int n, char *recherche){
    for(int i=0;i<n;i++){
        int j=0; 
        while(mots[i][j]!='\0' && recherche[j]!='\0' && mots[i][j]==recherche[j]) j++;
        if(mots[i][j]=='\0' && recherche[j]=='\0') return 1;
    }
    return 0;
}

/* Exemple */
int main(void){
    int n=4;
    char mots[4][20];
    lireMots(mots,n);
    printf("Mot le plus long : %s\n", mots[plusLong(mots,n)]);
    char r[20];
    printf("Mot a chercher : ");
    scanf("%s", r);
    printf(existe(mots,n,r) ? "Trouve\n" : "Pas trouve\n");
    return 0;
}
```

---

## **Exercice 7 — Fichier simple + tableau + calcul**

```c
#include <stdio.h>

void lireFichier(int *t, int n){
    FILE *f = fopen("nombres.txt","r");
    for(int i=0;i<n;i++) fscanf(f,"%d",&t[i]);
    fclose(f);
}

int max(int *t, int n){
    int m = t[0];
    for(int i=1;i<n;i++) if(t[i]>m) m=t[i];
    return m;
}

void doubler(int *t, int n){
    for(int i=0;i<n;i++) t[i]*=2;
}

/* Exemple */
int main(void){
    int n=8, t[8];
    lireFichier(t,n);
    printf("Max = %d\n", max(t,n));
    doubler(t,n);
    for(int i=0;i<n;i++) printf("%d ", t[i]);
    printf("\n");
    return 0;
}
```

---

## **Exercice 8 — Tri + concaténation + chaînes**

```c
#include <stdio.h>

int taille(char *str){
    int i=0; while(str[i]!='\0') i++;
    return i;
}

void trierString(char *str){
    int l = taille(str);
    for(int i=0;i<l-1;i++)
        for(int j=i+1;j<l;j++)
            if(str[j]<str[i]){
                char tmp=str[i]; str[i]=str[j]; str[j]=tmp;
            }
}

void concatenation(char *dest, char *src){
    int i=0; while(dest[i]!='\0') i++;
    int j=0; while(src[j]!='\0'){ dest[i]=src[j]; i++; j++; }
    dest[i]='\0';
}

/* Exemple */
int main(void){
    char s1[50], s2[50];
    printf("Entrez 1ere chaine : "); scanf("%s", s1);
    printf("Entrez 2eme chaine : "); scanf("%s", s2);
    trierString(s1); printf("Triee s1 : %s\n", s1);
    concatenation(s1,s2); printf("Concatenee : %s\n", s1);
    return 0;
}
```

---

## **Exercice 9 — Tableau 2D + multiplication + affichage**

```c
#include <stdio.h>

void remplir2D(int t[][5], int n){
    for(int i=0;i<n;i++)
        for(int j=0;j<5;j++){
            printf("t[%d][%d] = ", i,j);
            scanf("%d",&t[i][j]);
        }
}

void multiplierLigne(int t[][5], int ligne, int v){
    for(int j=0;j<5;j++) t[ligne][j]*=v;
}

void afficher(int t[][5], int n){
    for(int i=0;i<n;i++){
        for(int j=0;j<5;j++) printf("%d ", t[i][j]);
        printf("\n");
    }
}

/* Exemple */
int main(void){
    int n;
    printf("Nombre de lignes : ");
    scanf("%d",&n);
    int t[n][5];
    remplir2D(t,n);
    afficher(t,n);
    int ligne, val;
    printf("Quelle ligne multiplier ? "); scanf("%d",&ligne);
    printf("Multiplier par ? "); scanf("%d",&val);
    multiplierLigne(t,ligne,val);
    printf("Tableau apres multiplication :\n");
    afficher(t,n);
    return 0;
}
```

---

## **Exercice 10 — Chaîne + fichier + majuscules**

```c
#include <stdio.h>

int compterVoyelles(char *str){
    int i=0, c=0;
    while(str[i]!='\0'){
        char x = str[i];
        if(x=='a'||x=='e'||x=='i'||x=='o'||x=='u'||x=='y'||
           x=='A'||x=='E'||x=='I'||x=='O'||x=='U'||x=='Y') c++;
        i++;
    }
    return c;
}

void enregistrerPhrase(char *str){
    FILE *f = fopen("phrase.txt","w");
    fprintf(f,"%s",str);
    fclose(f);
}

void mettreMaj(char *str){
    int i=0;
    while(str[i]!='\0'){
        if(str[i]>='a' && str[i]<='z') str[i]-=32;
        i++;
    }
}

/* Exemple */
int main(void){
    char s[100];
    printf("Entrez une phrase : "); scanf(" %[^\n]", s);
    printf("Nombre de voyelles : %d\n", compterVoyelles(s));
    mettreMaj(s); printf("En majuscules : %s\n", s);
    enregistrerPhrase(s);
    printf("Phrase en majuscules sauvegardee dans phrase.txt\n");
    return 0;
}
```
