#include <stdio.h>
#include <stdlib.h>

void trocar(int v[], int c, int f){
    int aux;
    if(c < f){
        aux = v[c];
        v[c] = v[f];
        v[f] = aux;
        trocar(v, c + 1, f - 1);
    }
}
void imprimir(int v[], int t){
    if(t == 1)
        printf("%d ", v[t - 1]);
    else{
        imprimir(v, t - 1);
        printf("%d ", v[t - 1]);
    }
}

int main () {

    int vet[100];
    int i, n;

    printf("escreva o numero de elementos do vetor: ");
    scanf("%d", &n);
    printf("escreva os numeros: ");
    for (i = 0; i < n; ++i)
    scanf("%d", &vet[i]);

    imprimir(vet, n);
    printf("\n");
    trocar(vet, 0, n-1);
    imprimir(vet, n);


    return 0;
}
