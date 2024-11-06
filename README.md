include <stdio.h>
int main() {
    int n1, n2, i, j;

    // Leer el tamaño de la primera lista
    printf("Introduce el número de elementos de la primera lista: ");
    scanf("%d", &n1);
    int lista1[n1];
    
    printf("Introduce los elementos de la primera lista:\n");
    for (i = 0; i < n1; i++) {
        scanf("%d", &lista1[i]);
    }

    // Leer el tamaño de la segunda lista
    printf("Introduce el número de elementos de la segunda lista: ");
    scanf("%d", &n2);
    int lista2[n2];

    printf("Introduce los elementos de la segunda lista:\n");
    for (i = 0; i < n2; i++) {
        scanf("%d", &lista2[i]);
    }

// Encontrar elementos en común
printf("Elementos en común:\n");
for (i = 0; i < n1; i++) {
for (j = 0; j < n2; j++) {
if (lista1[i] == lista2[j]) {
printf("%d ", lista1[i]);
break;  // Rompe el bucle interno para evitar imprimir duplicados
            }
        }
    }
    printf("\n");
    return 0;
}