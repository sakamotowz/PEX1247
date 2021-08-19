#include <stdio.h>
#include <time.h>

float * fornecedor ( size_t n) {
    srand ( time ( NULL ));
    size_t i;
    float * solucao = (float *) malloc ( n * sizeof ( int ));
    for (  i = 0; i < n ; i ++) {
        solucao[ i] = rand () % 1000;
    }
    return solucao;
 }
float x (int n, float * V){
    float M = 0;
    int i; 
    for (i = 0; i < n; i++) {
        M += V[i];
    }
    return M/n;
}
int main () {
    float * V = fornecedor(700);
    int i;
    int n = 100;
    for (i = 0; i < n ; i ++) {
        printf ("Solução: %f \n", V[i]);
    }
    float media = x(n, V);
    printf("media: %f", media);
    return 0;
}
