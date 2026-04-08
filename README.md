#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main(int argc, char *argv[]) {

    if (argc!= 3) {
        printf("Voce precisa informar os limites para geracao do numero\n");
        return 0;
    }

    int min = atoi(argv[1]);
    int max = atoi(argv[2]);

    srand(time(NULL));
    int numero = min + rand() % (max - min + 1);

    printf("O numero aleatorio e %d\n", numero);

    return 0;
}# numeroaleatori0
