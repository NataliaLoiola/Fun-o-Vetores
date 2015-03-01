# Fun-o-Vetores
Vet-Soma Maior e Menor

#include <stdio.h>
#include <stdlib.h>
void matriz_teste(int matriz[5][5]);
main ()
{
    int mat[5][5],i,j;
    for (i=0;i<5;i++)
    {
        printf ("\nDIGITE CINCO ELEMENTOS DA LINHA %d DA MATRIZ.\n",i);
        for (j=0;j<5;j++)
        scanf ("%d",&mat[i][j]);
    }
    matriz_teste(mat);
    return 0;
    system("pause");
}
void matriz_teste(int matriz[5][5])
{
    int i,j,s=0,maior,menor=maior=matriz[0][0];
    for (i=0;i<5;i++)
    for (j=0;j<5;j++)
    {
        s=s+matriz[i][j];
        if (matriz[i][j]>maior)
        maior=matriz[i][j];
        else if (matriz[i][j]<menor)
        menor=matriz[i][j];
    }
    printf ("\nA SOMA DOS ELEMENTOS DA MATRIZ E: %d.\nO MAIOR ELEMENTO DA MATRIZ E: %d.\nO MENOR ELEMENTO DA MATRIZ E: %d.\n\n",s,maior,menor);
}
