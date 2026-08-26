#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    char buffer[40];
    int vikt;
    int reps;
    int rm;

    printf("STYRKELYFT - TEORETISKT 1RM\n");
    printf("--------------------------\n");

    printf("Ange vikt i kg: ");
    fgets(buffer, sizeof(buffer), stdin);
    vikt = atoi(buffer);

    printf("Ange antal repetitioner: ");
    fgets(buffer, sizeof(buffer), stdin);
    reps = atoi(buffer);

    rm = vikt + (vikt * reps) / 30;

    printf("\nTeoretiskt 1RM: %d kg\n", rm);

    return 0;
}

